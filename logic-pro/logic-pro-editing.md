# Logic Pro Editing

- `⇧D` / `Edit > Deselect All`: Deselect all.
- `⇧F`: Select following
- `⌃⇧F`: Select following of same track pitch (only select following for tracks with a region already selected)

## Ripple Delete

It's called "ripple" because the effect of the edit "ripples" to affect other clips.

Use `⌘-drag` to select an area (regardless of whether it contains regions) and then select `Edit > Delete and Move` to delete the selection and move everything from the right to fill the space (ripple delete).

There's no default key binding for `Delete and Move`, but `⇧⌫` makes a nice custom binding from Adobe Premiere Pro.

Note that this is affected by snap, so for finer-grained control toggle off snap (`⌘G`).

## Silence

To insert silence, put the locators where you want the silence to be inserted and select `Edit > Cut/Insert Time > Insert Silence at Locators` (`⌃⌘Z`).
