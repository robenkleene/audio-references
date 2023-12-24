# Max for Live Freeze

Working on frozen devices that use `bpatcher` is somewhat tedious, here's the process:

1. Optionally start by create a `git` branch
2. Open the device in Ableton Live and unfreeze it (just drag it to a new project, then click the `Edit` button), this should be done before editing any dependencies, otherwise duplicates of the files will be created.
3. Make changes
4. Open the device in Live again and freeze again
5. Merge the branch
