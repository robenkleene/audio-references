# Logic File Management

The "Save As..." dialog has two options: "Organize my project as a:" `Package` or `Folder`.

- **Package**: Will save the project as a single bundle with a `logicx` extension.
- **Folder**: Saves the project as a folder, with a `logicx` project file inside the folder. By default it creates two other folders: "Audio Files" and "Freeze Files".

## Strategy

Use the `Folder` method because this allows you to save many `.logicx` files with different variations in the same directory that can access the same assets. With the package method, each time you want to save a variation, that requires duplicating the entire project.
