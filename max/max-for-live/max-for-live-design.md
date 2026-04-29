# Max for Live Live Design

## Device Dimensions

- New Max for Live projects insert a comment with a Y origin of `170px`, indicating the real device height is `169px` (i.e., the device height ends `1px` before the comment)
- This is reinforced by the pixel measurements on macOS, accounting for Retina displays, the drawable device height in Max is `338px / 2px = 169px` (i.e., `338px` measured pixels results in `169px` usable pixels in Max)
- To prevent borders around the device, e.g., to make sure Live doesn't add extra padding to the right of the device, set the `Initial Window Size` to the exact width and height of the device (set the origin to `0. 0.`)

## Control Spacing

- `2px`: The horizontal and vertical spacing between control groups (i.e., groups of controls with a background panel behind them)
- `5px`: The horizontal and vertical padding between the edge of a panel or the device edge and the controls it contains
- `4px`: The horizontal and vertical spacing between controls (e.g., a `live.numbox` positioned next to or above another)
- `4px`: When a label is position to the left of a control (e.g., a label for a `live.numbox`)

### Math

The following algorithm can be used to calculate where controls should be positioned.

- `3px` is to start after `2px` spacing
- `maxVisualControlWidth` is the size of the largest control that can fit in this column (`44px` is a good default for this, in this case `live.text` buttons would be `44px` [note that a `live.text` button appears to have an extra pixel of spacing on each side, so a `46px` button has a visual width of `44px`])
- `visualControlWidth` is to account for spacing controls that are smaller than `maxVisualControlWidth` (e.g., `live.dial` are locked at `41px`)

`(maxVisualControlWidth + 3) × col + 3 + (maxVisualControlWidth − visualControlWidth) / 2`

Or simplified:

`3 + (44 + 3) × col`

Or simplified further:

Start from `3px` and add `47px` for each column.

This gives the following values for the first eight columns:

1. `3px`
2. `50px`
3. `97px`
4. `144px`
5. `191px`
6. `238px`
7. `285px`
8. `332px`

The spacing of the end of a panel is the same as the next control, so for a single column panel:

- The panel itself would have an origin of `0px`
- The first control would have an origin of `3px`
- The panel width would be `50px`

## Black Background Panels

For visual content, like graphs, use a black background (graphical controls [e.g., like dials] never go on the black background, but number controls, toggles, and pull-down menus do)

- The black background section for visual content typically extends all the way to bottom of the device (with the standard `2px` margin at the bottom, but that's not in the drawable area)
- When tabs use a black background then the selected tab visually connects to the black content area below it (i.e., the tab bar and the visual area appear as one continuous black region)

## Color

- Set panels to group controls to `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Device Background` to match the default that Live devices use for these panels
- Since `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Control Header` is the same color as the default Max background, it's a good idea to set the project `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Control Header`, which will show the default Live background color when the device is locked. To also use this color when unlocked, also set `Unlocked Patcher Background Color`
