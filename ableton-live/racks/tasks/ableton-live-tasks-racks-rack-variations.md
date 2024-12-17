# Ableton Live Tasks Racks Rack Variations

## `MIDI Effect Rack` `Chain`

1. Group multiple devices into a rack by selecting them, right clicking, and choosing `Group` (`⌘G`). (If there's only one device so far, only group it.)
2. Show the `Chain List` by toggling on the `Show/Hide Chain List` button. Drag devices to the `Drop MIDI Effects Here` section.
3. Select the `Chain` tab in the rack interface, for each device chain, move the little blue zone selectors so they don't overlap (i.e., drag the zone selector one key over so `0` is the first chain, and `1` is the second chain).
4. Map a `Macro` dial to the `Chain Selector` (the little tab at the top of the chain view) by toggling on the `Map` button at the top of the `MIDI Effect Rack`, then clicking the `Chain Selector` tab, then clicking the `Map` button on one of the `Macro` dials.

## Toggling `Device On` in a `MIDI Effect Rack` 

The chain zones only determine which devices MIDI gets routed to, to toggle on and off MIDI devices that output, regardless of MIDI input (e.g., for devices that generate MIDI), also map `Device On` for the device to the same `Chain Selector` `Macro` dial.

1. Toggle on `Map` for the macros
2. Click the `Device On` button
3. In the `Marco Mappings` sidebar that pops up in the upper right, set the `Device: On` `Min` and `Max` to the same zone range that the chain is active from (e.g., for the the zone that's only `Chain Selector: 0`, set `Min: 0` and `Max: 0`)