# Max Parameters

To set a value from an inspector via a message:

1. In the inspector select the value to set and copy it (`⌘C`)
2. Get the parameter name and value from the clipboard, and set it via a message (e.g., `_parameter_unitstyle 8`)

## Troubleshooting

Max stores a lot of state about child `bpatcher` parameters that it's unclear how to refresh (e.g., in GUI menus like the `live.banks` UI that opens when you double-click the object, it references old parameter names in child `bpatcher` that have already been updated).

To force these parameters to refresh, open the `.maxpat` file that contains the `bpatcher` and cut the entire contents (`⌘A` `⌘X`), save, then undo (`⌘Z`) to get the contents back.
