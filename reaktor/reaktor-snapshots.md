# Reaktor Snapshots

- Use Snapshots saved in the Ensemble, not Presets, and not Snapshot Banks (Presets can't use the morph functionality, and Snapshot Banks aren't automatically loaded).

## Editing & Saving Snapshots

1. Turn on edit mode for the ensemble by clicking the `Edit` button.
2. Make sure all the Instruments have `Include in Snapshots` toggled on by going to `Properties` (`F5`) and toggling on `Function > Snapshots > Include in Snapshots`.
3. Go to the `Preset Browser` (`F2`)
4. Select the select the Ensemble (prefixed with `Ens -`) in the `Select Instrument` pop-up menu (drop-down menu at the top of the `Preset Browser`) and disable `Follow instrument selection` (also under the `Select Instrument` dropdown)
5. Click the `Reaktor` menu, and choose `File > Save As` to save the Ensemble to a new location along with the current project
6. Under the `Preset Browser`, right-click the `Embedded` header and select `New Bank` (or use the existing bank if it's empty for the Ensemble)
7. Make some changes you are ready to save. The save icon should turn red, click the save icon (if you haven't already saved you can choose a location to save a copy of the Ensemble here)
8. With the bank to add to selected, create a Snapshot by clicking the `Add` button at the bottom the `Preset Browser` sidebar.
9. Click the red save icon again to save the Ensemble.

## Tips

- The snapshots shown in the Reaktor window title bar is determined by the `Snapshot Master`, choose the `Snapshot Master` by selecting the Ensemble (click the background), under `Function > Snapshots > Select Master`
