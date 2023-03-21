# Max Commands

## Mouse

- `⌘-double-click` object: Open `bpatcher`
- `⌥-click` object: Open help
- `⌘-click` white space: Unlock/Lock Window
- `⌥-drag`: To select patch cords
- `⌥-drag` from any object: To duplicate it
- `⌘-drag` object: Manipulate it as if the window were locked
- `⌘-double-click patcher`: Open it in a new window, even if the window is locked
- `⌘-double-click send` (or `receive`): See menu with all instances of the pair (the `⌘` isn't necessary in a locked window.)
- `⌥-click` any object: Help
- `Double-Click loadmess`: Fire message

### Keyboard

#### Palettes

- `⇧⌘I`: Open inspector in a separate window
- `⌘I`: Open inspector in sidebar
- `⇧⌘M`: Open console in a separate window
- `⌘M`: Open console in sidebar

#### Canvas

- `⌘Y`: Auto-align
- `⌘J`: Fix width (e.g., a comment)
- `⌃⌘O`: Show object explorer

#### Editing

- `⇧↩` / `⇥`: End editing
- `⌘'` / `Object > Name...`: Edit scripting name

## Presets

Using `presets` object with the mouse:

- `⇧-click`: Save current preset
- `click`: Restore preset
- `⇧⌥-click`: Delete preset

## Templates

Default values that are changed for a template (to be similar to Max for Live). All of these values can be changed under the "Inspector Window" ( `⇧⌘I` and click the background to see the patcher settings):

- **Grid Size**: `8. 8.`
- **Default Font Name**: `Arial Bold`
- **Default Font Size**: `10`
- **Snap to Grid on Open**: On
- **Snap to Objects on Open**: Off

The default template can be changed in "Preferences" -> "Default Patcher Template".

## Initial Window Size

To set the window size and position, select "Definite Initial Window Location".

## Special

- In messages `$1`, `$2`, etc... get replaced by arguments in an incoming list.
- Using `#0` at the start of a variable name gets replaced by a unique identifier at runtime. E.g., to use multiple copies of the same patch that use `send` and `receive`. (Note that this is only `#0`, `#1`, `#2`, etc... behave differently).
