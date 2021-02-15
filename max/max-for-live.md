# Max for Live

- **Device Height**: `342px`

## Distribution

- Freeze the device by opening it from Ableton Live and clicking the freeze icon and then saving again.

## Frozen Devices

Working on frozen devices that use `bpatcher` is somewhat tedious, here's the process:

1. Optionally start by create a `git` branch
2. Open the device in Ableton Live and unfreeze it, this should be done before editing any dependencies, otherwise duplicates of the files will be created.
3. Make changes
4. Open the device in Live again and freeze again
5. Merge the branch

- When preparing Max packages for release: Move the source folder out of the Max Project Search Path first to test all dependencies.

## Presets

When restoring presets, if there's a problem with loading garbage values that's usually because the `pattr` variables, e.g., not being set as `blob`.
