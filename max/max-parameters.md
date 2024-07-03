# Max Parameters

- `View > Parameters`: List all parameters
- To initially assign parameter values, if we're using `pattrstorage` with `preset`, first load a preset, then show the parameters list (`View > Parameters`), then toggle all of the `Initial Value Enabled` checkboxes on (it will automatically populate the `Initial Value` field with the `Value`).
- Parameters work the same whether using Max or Max for Live, parameters are stored in the `.maxpat` for Max (e.g., for the topmost patch) and in the `.amxd` for Max for Live

## Setting

To set a value from an inspector via a message:

1. In the inspector select the value to set and copy it (`⌘C`)
2. Get the parameter name and value from the clipboard, and set it via a message (e.g., `_parameter_unitstyle 8`)

## Troubleshooting

- A common problem for a parameter not loading is because the value gets overwritten by a `loadmess`
- Parameters seem to work well in `.amxd` but not great in `.maxpat`

### `bpatcher`

Max stores a lot of state about child `bpatcher` parameters that it's unclear how to refresh (e.g., in GUI menus like choosing `View > Parameters` or the `live.banks` UI that opens when you double-click the object, it references old parameter names in child `bpatcher` that have already been updated).

To force these parameters to refresh, open the `.maxpat` file that contains the `bpatcher` and cut the entire contents (`⌘A` `⌘X`), save, then undo (`⌘Z`) to get the contents back.
