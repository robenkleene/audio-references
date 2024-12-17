# Ableton Live Tasks Racks Rack Variations

Creating device chains:

1. Multiple device chains by dragging devices to the far left drop area
2. Choose the `Chain` tab in the rack interface
3. For each device chain, move the little blue zone selectors so they don't overlap
4. Set a `Macro` to the `Chain Selector` (the little tab at the top of the chain view), moving this `Macro` dial will then change which chain is active
5. Use MIDI automation to change the Chain Selector based on clips

## Toggling `Device On` in `MIDI Effect Rack`. 

The chain zones only determine which devices MIDI gets routed to, to toggle on and off MIDI devices that output, regardless of MIDI input (e.g., for devices that generate MIDI), also map the on status of the device to the same `Chain Selector` macro dial:

1. Toggle on `Map` for the macros
2. Choose the device on button
3. In the `Marco Mappings` sidebar that pops up, set the `Device: On` `Min` and `Max` to the same zone range that the chain is active from