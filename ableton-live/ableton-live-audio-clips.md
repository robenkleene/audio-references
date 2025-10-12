# Ableton Live Audio Clips

- Double-click to create a warp marker
- `⇧Drag` on the audio to move the audio under the warp marker
- If all the clip slots are filled, use `Create > Insert Scene` (`⌘I`) to add another scene
- `⇧Z`: Zoom in on current time selection (zooms into the whole clip if nothing is selected)
- `⇧X`: Zoom in on the entire clip (the `⇧Z` and `⇧X` shortcuts require `⇧` even though that isn't labeled in the menu item)

## Start & End

The `Start` and `End` of the clip, always the absolute boundary for playback (the `Loop` can't extend beyond the `Start` and `End`), and determines the played section if the `Loop` is off.

The upper lower set of braces in the `Clip` view is for the `Start` and `End`.

## Loop

The loop section has a `Position` and `Length` which determine the looped section. If looping is disabled, the clip will just play once and end.

A good workflow to temporarily focus on just a section of a clip is to set the `Loop` to just repeat the section being worked on.

The upper set of braces in the `Clip` view is for the `Loop` (note that moving the `Loop` while both the `Loop` and `Start` and `End` braces are at the same spot *will move both the `Loop` and the `Start` and `End`).

## Scrubbing

You can scrub audio by turning off quantization (`⌘0`) and moving the cursor above the waveform until it becomes a cursor icon.

## Extending Length

To extend the length of an audio clip (this does not bake in audio):

1. Drag it into the arrange view
2. Either loop the clip and select it, or to add silence, select an area spanning beyond the clips start or end
3. Choose `Edit > Consolidate` (`⌘J`)
4. The consolidated clip can then be dragged back to a slot on the `Session` view

## Packs

- To add a sample from a pack to a project, just right-click a clip and choose `Show in Browser`, then drag the audio clip into `Current Project` in the sidebar
