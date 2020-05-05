# Logic Pro

## Basic

- `x`: Toggle mixer
- `y`: Toggle library
- `v`: Hide/show all plugin windows
- `c`: Toggle loop
- `e`: Toggle editor
- `⌘k`: Toggle musical typing
- `⌘⌫`: Delete track
- `⌘G`: Toggle snap

## Zoom

- `⌘←` / `⌘→`: Zoom in and out horizontally
- `⌘↓` / `⌘↑`: Zoom in and out vertically
- `⌃⌥-drag`: Drag to zoom
- `⌃⌥-two-finger-drag`: Zoom in both X and Y
- `Z`: Toggle zoom to selection

General zoom strategy, put the playhead where you want to zoom in and then use `⌃⌥-two-finger-drag`.

## Tools

- `T`: Show tools menu
- Hold `⌃⌥` for zoom tool

### Tools Menu

`T`: Pointer
`Z`: Zoom

## Track Headers

- Click the divider to resize a tracker header
- `⇧click` to divider to resize all track headers to the same height
- `⌥drag` to resize all headers simultaneously

## Regions

- `⌃M`: Mute Region
- To select all regions in a track, click the track's header (name).
- To select a track, but not the regions, `⌥click` the track

### Tips

- For some reason you can only drag to loop regions when automation isn't visible (Toggle automation with `a`).

## Automation

- `⌃⌘⌫`: Delete visible automation for region
- Double-click an automation point to delete it.

## Transport

- `↩`: Go to beginning
- `␣`: Play

## Cycle

- `C`: Toggle Cycle

### Tips

- To set the cycle length to the selection, `^click` the Cycle button. (Turn on "Auto Set Locators")

### Removing Clicks

#### Fade Out

- Select the audio
- In the inspector on the left (toggle with `I`), under "More", enter a "Fade Out" of `1` (for `1ms`).

## MIDI Editing

- `⌘4`: Open the MIDI editor in a new window
- Clicking a key, selects all notes in that key
- `⌥↓` / `⌥↑`: Move note up or down
- `⇧⌥↓` / `⇧⌥↑`: Move note up or down
- `⌥o`: Toggle playing MIDI notes when they are selected (or click the symbol that looks like a MIDI cable above the piano roll)

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
