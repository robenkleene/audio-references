# Max for Live MIDI Tools

There are two types of MIDI tools: `Generator` and `Transformation`.

## Generator

- Clicking the `Apply` button (or toggling the `Generate` button from the `Generate` section in the Live clip settings) triggers outputting *an empty `notes` dictionary* from `live.miditool.in` (this means you don't need a separate button in Max patch to trigger the patch)

## Transformation

- Clicking the `Apply` button (or toggling the `Transform` button from the `Transform` section in the Live clip settings) triggers outputting *the current `notes` as a dictionary* from `live.miditool.in` (this means you don't need a separate button in Max patch to trigger the patch)

## Opening & Testing

Max for Live MIDI tools cannot be dragged and dropped into the UI the way regular Max for Live devices can. As a workaround, to quickly test a device, in the Ableton Live file tree click `Add Folder...` then add the folder for the Max for Live MIDI tool. It will then be available under the `Generate` drop-down menu.

## `live.miditool.in`

Outputs dictionaries of the current MIDI notes.

## `live.miditool.out`

Takes input of dictionaries to set the MIDI notes.

## Dictionary Format

A `notes` key.

- `pitch`
- `start_time`
- `duration`

### Optional Keys

- `velocity`
- `mute`
- `probability`
- `release_velocity`

### Examples

- `pitch: 56`
- `start_time: 0.`
- `duration: 0.25`
- `velocity: 100`
- `probability: 1`

Duration is relative to the current bar, so `0.25` is a quarter note.
