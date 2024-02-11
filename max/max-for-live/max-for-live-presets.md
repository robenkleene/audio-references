# Max for Live Presets

1. Add a `pattrstorage` and a linked `preset` object to save and restore presets, this allows saving and restoring from a JSON file
2. Use an `autopattr` in every `maxpat` that has parameters to automatically get them added to the `pattr` system

## Unique Names

When using `bpatcher`, to make sure objects have unique parameter names when using multiple instances, name each parameter (usually `Long Name` and `Scripting Name` starting with a `#1`). Then in the patcher containing the `bpatcher` set the `Argument(s)` field with a value for `#1`.

## Presets on Load

Don't try and load a preset on startup (instead start with an init patch), because there doesn't seem to be a solution to this that satisfies these conditions:

1. Keeps the Ableton Push interface in sync with the patch parameter settings
2. Doesn't interfere with Live's regular set state restoration (e.g., keeps loading the preset on startup from overwriting Live's device state restoration for the loaded Live set)
