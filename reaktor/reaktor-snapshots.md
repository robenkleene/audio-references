# Reaktor Snapshots

- Snapshots are embedded in the Ensemble file, whereas Presets are external files.
- Since Snapshots are written into the Ensemble file, the Ensemble must be in edit mode before writing presets.

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

### External Snapshot Banks

You can save a Snapshot Bank to an external `.ssf` file, in practice this isn't that useful though, because loading a `.ssf`

### Add a Snapshot

1. Turn on edit mode, by clicking the "Edit" button.
2. With the Preset browser selected (`F2`), right-click on "Embedded" and choose "New Bank".