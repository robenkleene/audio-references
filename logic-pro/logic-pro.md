# Logic Pro

## Basic

- `x`: Toggle mixer
- `y`: Toggle library
- `v`: Hide/show all plugin windows
- `c`: Toggle loop
- `e`: Toggle editor
- `⌘k`: Toggle musical typing
- `⌘⌫`: Delete track
- `⌘G`: Toggle snap, you can also hold `⌃` while dragging to temporarily turn off snapping

## Tips

- To set the song length drag the `End Marker` at the far right. (For some reason, if Logic Pro's window is flush with the edge of the screen it can be impossible to drag the `End Marker` any farther right, in this case move the window to the left so it's not flush and it should be possible to drag the marker.)

## Tools

- `T`: Show tools menu
- Hold `⌃⌥` for zoom tool

### Tools Menu

`T`: Pointer
`Z`: Zoom

## Regions

- `⌃M`: Mute Region
- Rename a region in the inspector on the left when a region is selected.
- To select all regions in a track, click the track's header (name). (Note that if the "Cycle" is active, only the regions in the Cycle will be selected.)
- To select a track, but not the regions, `⌥click` the track

### Tips

- For some reason you can only drag to loop regions when automation isn't visible (Toggle automation with `a`).

## Snap

By default Logic Pro snaps to relative values, e.g., if you move a region that's X number of ticks from a bar line, to another bar, it will maintain the distance of X from the new bar line. To switch this behavior, and snap to the bar line itself, under the `Snap` dropdown, select `Snap Regions to Absolute Values`.

## Cycle

- `C`: Toggle Cycle

### Tips

- To set the cycle length to the selection, `^click` the Cycle button. (Turn on "Auto Set Locators")

### Removing Clicks

#### Fade Out

- Select the audio
- In the inspector on the left (toggle with `I`), under "More", enter a "Fade Out" of `1` (for `1ms`).

## Plugins

- `[` / `]`: Next and previous preset

## Mixer

If the Solo button `s` has a red line through it that means it's in solo safe mode, to turn that off `⌃click` it.

## ReWire

- **Playback Mode**: Less CPU, use when not playing an instrument over ReWire (e.g., when you're only using audio routing).
- **Live Mode**: More CPU, use when playing an instrument over ReWire
- To receive audio over ReWire, "Mixer" -> "Options" -> "Create New Auxiliary Channel Strip" (`⌃n` with the Mixer visible), then choose your ReWire source as the input.

## Library Content

- The library content can be deleted from "About this Mac" -> "Storage" -> "Manage" -> "Music Creation"

## Frequency

The Channel EQ and MultiMeter (note you can scroll the MultiMeter!) both have a frequency analyzer.

## MIDI

- `⌥↑` / `⌥↓`: Move the selected MIDI notes up or down.

### Importing

- To import MIDI with the time signature and tempo information, use "File > Open" and select the MIDI file, this will create a new project.
- To just import the MIDI tracks, use "File > Import".
