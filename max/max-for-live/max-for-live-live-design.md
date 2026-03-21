# Max for Live Live Design

## Device Height

### Pixel Measurements

When viewing a device in Ableton Live on macOS, the height of a device is `342px` measured from the bottom of the `Device Title Bar` to the divider line below devices. But the last `4px` are not actually drawable by a device, so the drawable device height is `338px`.

### Max Dimensions

- Max for Live inserts a comment with a Y origin of `170px`, indicating the real device height is `169px` (i.e., the device height ends `1px` before the comment)
- This is reinforced by the pixel measurements on macOS, the drawable device height is `338 / 2 = 169`.

## Device Spacing

- `4px` separate colored sections (including from the border)
- The black background section for visual content typically extends to the bottom of the device (with the standard `5px` margin)
- Tabs use a black background, and the selected tab visually connects to the black content area below it (i.e., the tab bar and the visual area appear as one continuous black region)

## Color

- For visual content, like graphs, use a black background (graphical controls [e.g., like dials] never go on the black background, but number controls, toggles, and pull-down menus do)
- Groups of related controls (e.g., a few dials that belong together) have their own background panel, and `5px` gaps separate these groupings from each other and from adjacent sections

(e.g., often the correct height to use is `169px` in order to leave a `4px` empty border at the bottom which matches the design of most built-in devices)
