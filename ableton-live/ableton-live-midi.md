# Ableton Live MIDI

- `⌘B`: Turn on editing mode
- `⌘1` / `⌘2`: Narrow / widen grid
- To preview (play) notes when the MIDI editor is clicked on, turn on "MIDI Editor Preview" with the headphones icon above the piano roll notes.
- To give multiple notes the same velocity, select the notes then drag their velocity to the maximum, then to the desired value.
- To select all notes in a key, click the note in the piano roll.
- Use `⇧` click to select multiple non-continuous MIDI notes

## MIDI Editor

- To make a section play faster or slower, just select the MIDI notes and drag the handles above it squash or expand that section

## Presets

The `Pgm` and `Bank` settings to change external instrument presets are at the bottom of a MIDI clip's expanded options.

## Routing

To route MIDI from one track to another, just create a MIDI track (`⇧⌘T`) and set `MIDI To` to the other track (you may also have to select the specific instrument to route to in from the second drop down).

## MIDI Effects

Ableton Live seems not to support third-party MIDI effects, e.g., when inserting a plugin, Reaktor lists `Reaktor 6` and `Reaktor 6 FX`, for the instrument and audio effects, but not `Reaktor 6 MIDIFX`, for the MIDI effect.

### Recording

To record the MIDI output from a MIDI effect:

1. Setup a new MIDI track (`⌘⇧T`)
2. Set the `MIDI From` to the track with the MIDI effect
3. Click the `ARM Recording` button at the bottom of the new MIDI track
4. Click the record button for an empty clip slot on the new MIDI track

## MIDI Export

Ableton Live can import multi-track or single-track MIDI files but it can only export single track. To export MIDI, right-click the MIDI clip and select "Export MIDI Clip..."
