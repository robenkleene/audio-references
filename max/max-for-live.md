# Max for Live

- **Device Height**: `342px`

## Distribution

- Freeze the device by opening it from Ableton Live and clicking the freeze icon and then saving again.

## Frozen Devices

Working on frozen devices that use `bpatcher` is somewhat tedious, here's the process:

1. Optionally start by create a `git` branch
2. Open the device in Ableton Live and unfreeze it (just drag it to a new project, then click the `Edit` button), this should be done before editing any dependencies, otherwise duplicates of the files will be created.
3. Make changes
4. Open the device in Live again and freeze again
5. Merge the branch

### Deleting Duplicate Files

If the device is opened and unfrozen in Ableton Live after dependencies have already been edited, duplicate files will be created. To clean these up:

1. Open the project in Max
2. Right-click the `bpacher` and choose `Object > Open Original <...>`
3. Delete those duplicated files
4. Close and re-open the project

#### Troubleshooting

Sometimes duplicate files get created even if nothing has been modified (which means they'll get re-created every time we unfreeze) in this case, deleting the files after unfreezing, then closing the project and re-opening it should work to get it referencing the right files.

### Isolated Testing

When preparing Max packages for release: Make sure to test without the source folder for the patch in Max's Search Paths, otherwise it may pick up a dependency that isn't actually in the bundle.

## Presets

When restoring presets, if there's a problem with loading garbage values that's usually because the `pattr` variables, e.g., not being set as `blob`.
