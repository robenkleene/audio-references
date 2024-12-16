# Ableton Live Racks

- A chain is a path from MIDI to signal to output
- Each Drum Rack chain receives input from a single assigned MIDI note
- Macro Controls are a bank of eight knobs each capable of adding any number of parameters from any device in a Rack.

## Types

- `MIDI Effect Rack`: Only MIDI effects, only on MIDI tracks
- `Audio Effect Rack`: Only audio effects, on audio or MIDI tracks
- `Instrument Racks`: Instruments, MIDI and audio effects. MIDI effects must be first, then an instrument, then audio effects.
- `Drum Racks`: Similar to Instrument Racks. Instruments, MIDI, and Audio effects, with the same signal flow rules.

## Macro Controls

- To put a control on the Macro Control panel, just right-click it and choose `Map to Macro`.
- Use `⌘R` to rename macro controls
- To add a third-party instrument's parameters, click `Configure` then move a parameter, it will appear in the Ableton Live panel for that instrument, then can be right-clicked to map to a macro.

## Toggling Devices

1. Group effects into an `Audio Effect Rack` (select the devices and `⌘G`)
2. Toggle on `Map` for a macro dial
3. Click the `Device On` button on the first effect
4. Click the `Map` button for the first dial
5. Now setting the dial to `64>` will have the device off, and `63<` will have the device on
