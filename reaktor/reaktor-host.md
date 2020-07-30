# Reaktor Host

When running Reaktor within a host, the state of parameters is automatically saved with the host, but snapshots, properties, and changing the structure are not saved. To save these kinds of changes, you'll have to make a separate copy of your ensemble.

There are two methods of managing a separate copy:

1. Saving edited Ensembles manually
2. Saving edited Ensembles automatically

Factory Ensembles are write protected, so neither of these methods will ever overwrite a factory ensemble.

## Manual

To save an Ensemble manually, make a change that requires saving, then click the red "Save Ensemble" button in the upper left. If this is the first time you've clicked that button, you'll be prompted for a location to save the Ensemble. If you click the button again later, it will overwrite the current save location.

To access the save again to a new location, click the triangle to the right of the Reaktor logo to access a menu that has a "File > Save As…" option.

Note: It's unclear if a *User Library* ensemble is loaded, whether the first click to the "Save" icon will prompt for a save location or whether that's only for the Factory Library? As a convention, it's probably a good idea to always save to a new location the first time?

## Automatic

## Notes

As a convention, always save the Ensemble in the same folder as the hosts project file. You'll usually want to make a container directory with both the hosts project file and the Ensemble inside, for example:

- `My Song`
    - `My Song.logicx`
    - `My Edited Ensemble.ens`