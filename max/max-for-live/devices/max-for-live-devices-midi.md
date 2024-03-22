# Max for Live Devices MIDI

There are two types, `Generator` and `Transformation`.

## Generator

- Pressing the `Generate` button from the `Generate` section in the Live clip settings, triggers outputting *an empty `notes` dictionary* from `live.miditool.in` (this means you don't need a separate button in Max patch to trigger the patch)

## Transformation

- Pressing the `Transform` button from the `Transform` section in the Live clip settings, triggers outputting *the current `notes` as a dictionary* from `live.miditool.in` (this means you don't need a separate button in Max patch to trigger the patch)

## `live.miditool.in`

Outputs dictionaries of the current MIDI notes.

## `live.miditool.out`

Takes input of dictionaries to set the MIDI notes.

## Dictionary Examples
