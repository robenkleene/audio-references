# Max for Live Live Design

## Device Height

### Pixel Measurements

When viewing a device in Ableton Live on macOS, the height of a device is `342px` measured from the bottom of the `Device Title Bar` to the divider line below devices. But the last `4px` are not actually drawable by a device, so the drawable device height is `338px`.

Live devices also have a `4px` border between groupings of controls.

### Max Dimensions

- New Max for Live projects insert a comment with a Y origin of `170px`, indicating the real device height is `169px` (i.e., the device height ends `1px` before the comment)
- This is reinforced by the pixel measurements on macOS, accounting for Retina displays, the drawable device height in Max is `338px / 2px = 169px`
- Similarly, after accounting for Retina displays, the border width between control groups should be `4px / 2px = 2px`
- To prevent borders around the device, e.g., to make sure Live doesn't add extra padding to the right of the device, set the `Initial Window Size` to the exact width and height of the device (set the origin to `0. 0.`)

## Device Spacing

- `2px` separate colored sections (including from the border)
- The black background section for visual content typically extends all the way to bottom of the device (with the standard `2px` margin at the bottom, but that's not in the drawable area)
- Tabs use a black background, and the selected tab visually connects to the black content area below it (i.e., the tab bar and the visual area appear as one continuous black region)

## Control Spacing

- When a Live device has a single column of full size controls, the panel behind the controls should be `53px` (resulting in a Retina Display width of `106px`)
- Two columns of controls is `113px` (`226px` Retina Display width)

## Color

- For visual content, like graphs, use a black background (graphical controls [e.g., like dials] never go on the black background, but number controls, toggles, and pull-down menus do)
- Groups of related controls (e.g., a few dials that belong together) have their own background panel, and `2px` gaps separate these groupings from each other and from adjacent sections
- Set panels to group controls to `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Device Background` to match the default that Live devices use for these panels
- Since `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Control Header` is the same color as the default Max background, it's a good idea to set the project `Device Inspector > Color > Locked Patcher Background Color > Dynamic > Live Theme Colors: Control Header`, which will show the default Live background color when the device is locked. To also use this color when unlocked, also set `Unlocked Patcher Background Color`
