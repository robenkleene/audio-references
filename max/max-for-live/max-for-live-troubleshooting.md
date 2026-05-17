# Max for Live Troubleshooting

- In Max for Live, for `send` / `receive` to have unique identifiers, prefix the identifier with `---` (instead of `#0`). `---` is a unique device-wide identifier (`#0` is for each patcher). It's unclear whether `---` and `#0` can be combined into `---#0`.

## Deleting Duplicate Files

If the device is opened and unfrozen in Ableton Live after dependencies have already been edited, duplicate files will be created. To clean these up:

1. Open the project in Max
2. Right-click the `bpacher` and choose `Object > Open Original <...>`
3. Delete those duplicated files
4. Close and re-open the project

### Problems With Duplicate Files

Sometimes duplicate files get created even if nothing has been modified (which means they'll get re-created every time we unfreeze) in this case, deleting the files after unfreezing, then closing the project and re-opening it should work to get it referencing the right files.

## Device Prompts for a Save Path on Every Save

If editing a `.amxd` device in Ableton Live prompts for a save location every time (instead of saving in place at the default path), the device's embedded Max project is flagged read-only.

A `.amxd` file is a small binary header followed by the patcher JSON. That JSON contains an embedded project object (`"project": { ... }`) listing the device's dependencies. If that project has `"readonly": 1`, Max refuses to write into it and falls back to "Save As" on every save.

This typically happens when the device was once part of a Max *package* — package contents are read-only by design, and the flag gets baked into the device's embedded project and persists even after the package is removed.

To fix it, change `"readonly": 1` to `"readonly": 0` in the patcher JSON:

1. The value lives in the JSON after the 32-byte binary header — search for `"readonly"`.
2. It is a length-preserving single-character edit, so the `ptch` chunk size in the header does not need updating.
3. Reload the device in Live (remove and re-add so Live re-reads the file) and confirm saves no longer prompt.

There is no Max UI toggle for this flag — it is internal state Max derives from context. The UI-only alternative is to rebuild the device: create a fresh device of the same type in Live, copy all objects into it, and save (a freshly created device gets a writable project).