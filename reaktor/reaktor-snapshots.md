# Reaktor Snapshots

The most reliable method is to save Snapshots for each Instrument first, then use the Ensemble to save Snapshots of combinations of Instrument Snapshots.

## Setup

1. Turn on edit mode for the ensemble by clicking the `Edit` button.
2. Make sure all the Instruments have `Include in Snapshots` toggled on by going to `Properties` (`F5`) and toggling on `Function > Snapshots > Include in Snapshots`.
3. Go to the `Preset Browser` (`F2`)
4. In the `Select Instrument` pop-up menu (drop-down menu at the top of the `Preset Browser`) toggle on `Follow instrument selection`
5. Click the `Reaktor` menu, and choose `File > Save As` to save the Ensemble to a new location along with the current project

## Creating Presets

### Instrument

Use Instrument Snapshots to save control changes.

1. Under the `Preset Browser`, right-click the `Embedded` header and select `New Bank` (or use the existing bank if it's empty)
2. Make some control changes
3. With the bank to add to selected, create a Snapshot by clicking the `Add` button at the bottom the `Preset Browser` sidebar
4. Click the red save icon again to save the Instrument

### Ensemble

Use Ensemble Snapshots to save combinations of Instrument Snapshots.

1. Under the `Preset Browser`, right-click the `Embedded` header and select `New Bank` (or use the existing bank if it's empty)
2. With the bank to add to selected, create a Snapshot by clicking the `Add` button at the bottom the `Preset Browser` sidebar
3. Choose some instrument presets
4. Click the red save icon again to save the Ensemble
