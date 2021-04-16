# Logic Pro Podcast

- Male voice should be high in the 85 to 200 range, use EQ to boost the that range if necessary, and lower other ranges.
- To make music and voice sound good together, use EQ to lower the music where it's clashing with the voice.

## Tips

- In the "Editor", run "Functions > Remove Silence..."

## Effects

`Noise Gate > EQ > Compressor > Limiter`.

Use one of the voice presets for the compressor.

## Podcast

- Right-click the HUD and select `Customize Control Bar and Display...`, and add `Varispeed`. Varispeed lets you double the speed of playback for faster editing. The `-+` button in the toolbar toggles it on and off.

### Remove Silence

To remove silence (cutting the audio into many small clips), right-click the region and choose `Split > Remove Silence from Audio Region...`.

Good settings are:

- `Threshold: -22`
- `Minimum Time to accept as Silence: 0.1`
- `Pre Attack-Time: 0.05`
- `Post Release-Time: 0.03`
- `Search Zero Crossing: On`

After removing silence, select all the regions and using the inspector to apply a `10` `Fade In` and `Fade Out`.

### Process

1. Line up the tracks.
2. Make duplicates of each track, and mute the second copy. This is so we always have a reference of the original audio which can assist in re-aligning if we make a mistake.
3. Add effects to each track, listen to parts of each track where someone speaks a lot and make sure it sounds natural.
4. Run remove silence and add fade in and fade outs, listen to parts of each track where someone speaks a lot and make sure it sounds natural.
5. Listen and make small edits of two types:
    1. Delete little bits of irrelevant noise.
    2. Close gaps of silence.
    - For performing these edits, using `⌘-drag` to select across all three tracks and then doing a ripple delete with `Delete and Move` (`⇧⌫`) is helpful. To get finer-grained control with `⌘-drag`, toggle off snap with `⌘G`.

### Tips

- To remove silence in a track, or all tracks, use ripple delete.
- To add silence, to one track use `⇧F` to select forward and drag the regions.
- To add silence to multiple tracks, select a region in each track and use `⌃⇧F` to select forward for all selected regions, and drag the regions.

## Export

- Just use a regular bounce (`⌘B`), with `160 kbps` bit rate. Set `Normalize: Off`. Make sure `Variable Bit Rate` is off.
