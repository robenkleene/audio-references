# Logic Files

The "Save As..." dialog has two options: "Organize my project as a:" `Package` or `Folder`.

- **Package**: Will save the project as a single bundle with a `logicx` extension.
- **Folder**: Saves the project as a folder, with a `logicx` project file inside the folder. By default it creates two other folders: "Audio Files" and "Freeze Files".

## Strategy

Always use the package format instead of folder. The package format only really encapsulates files that are automatically managed by Logic, so the package format provides nice encapsulation of everything that's managed by Logic.

### External Assets

If you do have external assets, like additional presets that you want to store with a project but that aren't managed by logic, just create a folder and move the `logicx` package into it, and then add the assets to that folder.

For example:

- `Reaktor Sequencer Triggering`
    - `Reaktor Sequencer Triggering.logicx`
    - `Blue Matrix Edited.ens`
