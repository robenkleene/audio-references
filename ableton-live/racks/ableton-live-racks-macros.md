# Ableton Live Racks Macros

Macros allow you to take map a knob to control a parameter inside the rack. Multiple parameters can be mapped to the same macro knob.

## Mappings

- To put a control on the Macro Control panel, just right-click it and choose `Map to Macro`.
- Use `⌘R` to rename macro controls
- To add a third-party instrument's parameters, click `Configure` then move a parameter, it will appear in the Ableton Live panel for that instrument, then can be right-clicked to map to a macro.

## The Map Button

1. Toggle on `Show/Hide Macro Controls`, and click the `Map` button on the rack's title bar.
2. After clicking the `Map` button, the `Macro Mappings` sidebar will appear that shows all the parameters mapped to that macro knob
3. Click a control and an outline will highlight that control
4. Click the map button on the macro knob
5. When you're done mapping parameters to macros, click the `Map` button in the rack's title bar again to exit mapping mode

### Notes

Multiple parameters can be mapped to a single macro dial, if `Map` is active in the rack's title bar, then clicking a device parameter will activate the `Map` button on the macro dial's, if that parameter is already mapped to the device parameter, then it will be an `Unmap` button to unmap that parameter from that dial. (Note that unmapping parameters never changes the name of the macro dial, like `Map` does when adding the first parameter, so macro dial names need to be renamed manually after unmapping.)

## Macro Variations

- Show by toggling the `Show/Hide Macro Variations` button
- The `New` button stores a new `Macro Variation` with the current settings
- Double-click the variation name, or single click the play button, to restore a variation
- If a parameter changes with a variation selected, then a asterisk (`*`) appears next to its name to indicate it was edited. To update an edited variation click the `Overwrite` button (looks like the top a battery with a `+` icon on it) for the variation
- There isn't an easy built-in way to toggle variations based on clips, the best approach is to control the variation with an external control (e.g., using Max for Live with the Live API), and then control that control.

## `MIDI Effect Rack` `Chain`

1. Group multiple devices into a rack by selecting them, right clicking, and choosing `Group` (`⌘G`). (If there's only one device so far, only group it.)
2. Show the `Chain List` by toggling on the `Show/Hide Chain List` button. Drag devices to the `Drop MIDI Effects Here` section.
3. Select the `Chain` tab in the rack interface, for each device chain, move the little blue zone selectors so they don't overlap (i.e., drag the zone selector one key over so `0` is the first chain, and `1` is the second chain).
4. Map a `Macro` dial to the `Chain Selector` (the little tab at the top of the chain view) by toggling on the `Map` button at the top of the `MIDI Effect Rack`, then clicking the `Chain Selector` tab, then clicking the `Map` button on one of the `Macro` dials.

### Toggling `Device On` in a `MIDI Effect Rack`

The chain zones only determine which devices MIDI gets routed to, to toggle on and off MIDI devices that output, regardless of MIDI input (e.g., for devices that generate MIDI), also map `Device On` for the device to the same `Chain Selector` `Macro` dial.

1. Toggle on `Map` for the `MIDI Effect Rack`
2. Click the `Device On` button
3. Click the `Map` button for a `Macro` dial
3. In the `Marco Mappings` sidebar in the upper left, set the `Device: On` `Min` and `Max` to the same zone range that the chain is active from (e.g., for the the zone that's only `Chain Selector: 0`, set `Min: 0` and `Max: 0`)
