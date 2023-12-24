# Max for Live Troubleshooting

### Deleting Duplicate Files

If the device is opened and unfrozen in Ableton Live after dependencies have already been edited, duplicate files will be created. To clean these up:

1. Open the project in Max
2. Right-click the `bpacher` and choose `Object > Open Original <...>`
3. Delete those duplicated files
4. Close and re-open the project

#### Troubleshooting

Sometimes duplicate files get created even if nothing has been modified (which means they'll get re-created every time we unfreeze) in this case, deleting the files after unfreezing, then closing the project and re-opening it should work to get it referencing the right files.
