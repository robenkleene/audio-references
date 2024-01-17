# Max `bpatcher`

## Arguments

- In the Inspector, for the `bpatcher` object (e.g., in the patcher *containing* the `bpatcher`), set the `Argument(s)` field.
- In the `bpatcher` the arguments can then be used as `#1`, e.g., in messages, but also for `Short Name`, `Long Name`, and `Scripting Name`, but *only* at the beginning (e.g., `#1-foo`)
- The `#1` can also be used in the arguments list, e.g., so a parent `bpatcher` can pass its argument to a child `bpatcher`

## Troubleshooting

Max stores a lot of state about child `bpatcher` parameters that it's unclear how to refresh (e.g., in GUI menus like choosing `View > Parameters` or the `live.banks` UI that opens when you double-click the object, it references old parameter names in child `bpatcher` that have already been updated).

To force these parameters to refresh, open the `.maxpat` file that contains the `bpatcher` and cut the entire contents (`⌘A` `⌘X`), save, then undo (`⌘Z`) to get the contents back.
