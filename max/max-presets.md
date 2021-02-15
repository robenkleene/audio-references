# Max Presets

The strategy for presets with Max for Live:

1. Have the `pattrstorage` system only read and write JSON files
2. Store the current state with Ableton Live

## Alternatives

There is a way to have the current status of `pattrstorage` be stored with a Live set, this is done by toggling on all of the following options in the Info panel of `pattrstorage`:

1. **Parameter Mode Enabled**: Exposes `pattrstorage` to Live presets
2. **Initial Enabled**: Store `pattrstorage` values in the patch file automatically
3. **Auto-Update Parameter Initial Value**: Automatically store changes into the patch file

It appears that for a compiled Max for Live device, storing in the patch file becomes storing as an Live preset. If option two is not enabled, then Live will ask for a path to save the presets at when quitting.

The above is useful behavior, but it also creates a problem: Once those options are turned on, it becomes impossible to use a `loadbang` to load a `pattrstorage` preset on startup, for some reason the preset just doesn't load.
