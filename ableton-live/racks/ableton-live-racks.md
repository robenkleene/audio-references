# Ableton Live Racks

There are four types of racks:

- `Audio Effect Rack`
- `Drum Rack`
- `Instrument Rack`
- `MIDI Effect Rack`

## Macros

Macros allow you to take map a knob to control a parameter inside the rack. Multiple parameters can be mapped to the same macro knob.

### Mapping

To map a control to a macro:

1. Click the `Map` button on the rack's title bar while the rack's `Macro Controls` are visible
2. After clicking the `Map` button, the `Macro Mappings` sidebar will appear that shows all the parameters mapped to that macro knob
3. Click a control and an outline will highlight that control
4. Click the map button on the macro knob
5. When you're done mapping parameters to macros, click the `Map` button in the rack's title bar again to exit mapping mode

## Chain Selector

The chain selector only determines where MIDI is routed, that means that it doesn't disable audio or MIDI output for devices that aren't in that chain. This means for example that instruments and MIDI effects that don't need MIDI input will continue to output sound or MIDI even if they aren't on a selected chain. As a workaround, these devices can be toggled on and off with the same macro as the `Chain Selector`.

- Show it by choosing the `Chain` tab, then move the zone to choose when the chain active. If the chain is active MIDI will be sent to that chain (note that if a chain outputs audio without MIDI input, e.g., if it has a MIDI device on it that outputs MIDI, then that will continue to be active, the chain selector only controls which chain has MIDI routed to it)

### Toggle Devices With the Chain Selector

- To toggle devices on and off based on their zone (e.g., so MIDI devices don't output when the chain isn't selected), map the device on to the Chain Selector macro, under the `Macro Mappings` sidebar that pops up when mappings are active, there's an option to set the `Min` and `Max` for device on, if that's set to only the zones where the chain is active, then it will toggle off and on depending on whether the `Chain Selector` macro is set to an active zone.
