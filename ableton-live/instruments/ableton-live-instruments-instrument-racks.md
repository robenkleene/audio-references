# Ableton Live Instruments Instrument Racks

## Chain Selector

- Show it by choosing the `Chain` tab, then move the zone to choose when the chain active. If the chain is active MIDI will be sent to that chain (note that if a chain outputs audio without MIDI input, e.g., if it has a MIDI device on it that outputs MIDI, then that will continue to be active, the chain selector only controls which chain has MIDI routed to it)

### Toggle Devices With the Chain Selector

- To toggle devices on and off based on their zone (e.g., so MIDI devices don't output when the chain isn't selected), map the device on to the Chain Selector macro, under the `Macro Mappings` sidebar that pops up when mappings are active, there's an option to set the `Min` and `Max` for device on, if that's set to only the zones where the chain is active, then it will toggle off and on depending on whether the `Chain Selector` macro is set to an active zone.

## Macros

To map a `Macro` control to a parameter, use the `Map` button in the title bar of the `Instrument Rack`.