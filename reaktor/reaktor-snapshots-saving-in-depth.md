# Reaktor Snapshots

## Keyboard Shortcuts

- `F2`: Show `Preset Browser`
- `↓` / `↑`: When the `Preset Browser` has focus, go to the next / previous preset

## Basics

These issues you need to deal with if you're using Reaktor no matter what.

- If the save button is red, it means you will lose data if you quit (regardless whether you are using Snapshots or other Ensemble changes or not).
- Making any edit to graph-style UI elements will make the button red and require saving as a separate file. Changing knobs and sliders generally will not.
- If you're using an Ensemble saved to a file, and you move the Ensemble (e.g., if you're keeping it with a project, and you move the project), then you'll need to re-locate the file the next time you open the project.

## Notes

- Snapshots are embedded in the Ensemble file, whereas Presets are external files.
- Since Snapshots are written into the Ensemble file, the Ensemble must be in edit mode before writing presets.

## Quick Start

How to quickly save and reload Snapshots.

1. Turn on edit mode for the ensemble by clicking the `Edit` button.
2. In the sidebar, in the `Select Instrument` pop-up menu, select the Ensemble (prefixed with `Ens -`), and disable `Follow instrument selection`.
3. Make some changes you are ready to save. The save icon should turn red, click the save icon and choose a location to save a copy of the Ensemble (by convention, put it next to the host project file).
4. Under the `Preset Browser` (`F2`), right-click the `Embedded` header and select `New Bank`.
5. With the bank to add to selected, create a Snapshot by clicking the `Add` button at the bottom the `Preset Browser` sidebar.
6. Click the red save icon again to save the Ensemble.

## Instruments vs. Ensembles

- Snapshots or Presets can either be saved in Instruments or Ensembles. If an Ensemble has at least one Instrument, when the "Preset Browser" (`F2`) is selected, a dropdown menu will appear at the top. The Ensemble is always at the top and is the name of the Ensemble prefixed with `Ens -`. The list of Instruments in the Ensemble are listed below.

If the Ensemble does not contain any instruments, than the dropdown menu will not be visible because the only possible selection is the Ensemble.

## Tips

- Generally consensus seems to be to avoid presets because they're a bit of an afterthought technology that exists because Reaktor Player cannot edit ensemble files.

## Presets

- Presets cannot be recalled by MIDI via Bank and Program Change Messages, and do not support the "Morph + Randomize" functionality.

### Files

Presets are stored in your "Native Instruments > User Content" folder.

It's unclear if a preset file can be stored in another location (such as next to a host project file), presets just aren't used very much so there isn't much information on them, for this reason, we'll stick with snapshots.

## Snapshots

### Snapshot Banks as Files

Snapshot banks can be stored as external `.ssf` files. In practice this isn't that useful though, because loading a `.ssf` doesn't persist across host re-launches.

#### Saving

To save a Snapshot Bank as a `.ssf` file, turn on edit mode,  right-click the bank and select "Save Bank".

#### Loading

To load a Snapshot Bank from an `.ssf` file, turn on edit mode, right-click an existing bank (or the `Embedded` header) and select "Load Bank".

### Embedded Snapshot Banks

The only reliable way to add banks appears to be to embed banks in the ensemble.

#### Creating a Bank

1. Turn on edit mode, by clicking the "Edit" button.
2. With the `Preset Browser` selected (`F2`), right-click on "Embedded" and choose "New Bank".

#### Creating a Snapshot

When creating Snapshots, you probably want to first select the Ensemble (prefixed with `Ens -`) from the `Select Instrument` pop-up menu, and disable `Follow instrument selection`. Otherwise it's to easy to add the Snapshot to the wrong instrument. If you're having trouble saving and restoring a snapshot, this is probably the problem.

1. With the bank to add to selected, create a Snapshot by clicking the `Add` button at the bottom the `Preset Browser` sidebar.

#### Deleting a Snapshot

Right-click the snapshot and select `Delete`.

## Troubleshooting

- In `Properties` (`F5`), make sure `Recall by MIDI` is turned on, and that `Select Master` is set to the main ensemble.

### Unreliable

Snapshots seem to be completely unreliable: Sometimes they only partially restore, sometimes they don't restore at all, particularly when triggered by program change MIDI messages. When having trouble changing Snapshots via MIDI messages, the best approach I've found is to simply take the Snapshot that isn't working and click the `Add` button to create a duplicate in a later slot. The new Snapshot tends to work. Note that using `Store` to overwrite the snapshot, does not seem to work.
