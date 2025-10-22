# Ableton Live Arrangement

- `HOME` / `END`: Move the Insert Marker to the beginning or end of the track
- `F10`: Back to arrangement

## Loop

- `⌘L`: Toggle loop (the loop marker must be selected)
- `⌘←` / `⌘→`: Shorten / lengthen loop

### Loop Whole Song

1. `⌘A`: To select whole song
2. `⌘L`: To loop selection

## Looping Clips

- To loop a clip, make sure `Loop` is toggled on when the clip is selected, and then just drag the right edge of the clip to the loop duration.

## Session to Arrangement

- Note that clip-based automation in the Session View is converted to "track-based" automation in the Arrangement View. This is because clip-based automation in Session View sets the value directly, whereas clip-based automation in the Arrangement View is *modulation*, it changes the base value. So in order to preserve the session view's clip-based automation values, it needs to set the base value, which can only be done as track-based automation in the Arrangement View, so the automation is converted to track-based automation. (This is also why boolean values like `Device On`, can't be set in the clip-based automation in the Arrangement View, because boolean values can't be modulated.)

### Drag & Drop

- Start dragging a clip, hit `⇥` to switch to `Arrangement`, drop the clip

## Troubleshooting

- When an audio in the arrange view can't be heard, click `Return to Arrangement` in the upper right of the tracks
- Clicking `Return to Arrangement` will also prevent an audio track from being recorded over by clips

## Splitting

To split a clip:

1. Click in the clip to place the `Insert Marker`
2. `Edit > Split` (`⌘E`)
