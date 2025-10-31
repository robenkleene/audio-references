# Ableton Live Automation

- You can show automation by a control either by changing its value, or, to show automation without changing the current value, right-click the control and choosing `Show Automation`
- If automation is just setting a parameter to a single value (e.g., `Device On`), then you only need one point at the beginning (e.g., a second point at the end isn't necessary)

## Automation

- Automation sets a parameter to a specific value
- In Session View, Automation is by clip, while in the Arrangement View it's by track
- If a parameter is being automated, a red dot is displayed on its control

## Modulation

- Modulation is always relative to the parameters current value
- Modulation is by clip both in the Arrangement and Session views
- Modulated parameters change the section that's blue
- If a parameter is being modulated, a blue dot is displayed on its control (note the blue dot does not seem to appear for clip-based automation)
- Boolean parameters (like `Device On`) cannot be modulated because they only have two values
- A green dot, means the parameter is linked to a macro

### Multiplicative vs. Additive

Modulation can either by multiplicative or additive, if the modulation range goes from `0--100%`, it's multiplicative, if it goes from -`50--50%`, then it's additive.

- Multiplicative never increases the value of a parameter it only attenuates it (so if a parameter is set to `70%`, setting the modulation to `0`% will set it to `0%`, and `100%` will set it to `70%`)
- Additive will increase or decrease the value of a parameter by up to half of the parameters range (so if a parameter is set to `70%`, setting the modulation to `-50%` will set it to `20%` and `+50%` will set it to `100%`)


## Devices

- `Right-click` a parameter and choose `Show Automation`
- To delete automation on a Device, right-click on a control and select `Delete Automation`

## Graph Editor

With the pointer tool enabled (e.g., make sure the pencil tool is toggled off with `⌘B`):

- `click`: Add / remove point
- `click&drag`: Move point
- `⇧click`: Move point or line

### Snap

- Turn off snap under `Options > Snap to Grid` (`⌘4`).
- Hold `⌘` to disable snap while dragging
- Constrain to one axis by holding `⇧` while dragging

## Arrangement

- `A`: Toggle `Automation` in the arrange view (if this isn't working, it's probably because `Options > Computer MIDI Keyboard` [keyboard icon in upper right] is toggled on, `M` to toggle off)

### Deleting

- `⌘A ⌫` will select all clips and automation and delete it (this includes *all* automation data, not just the selected automation data)

### Duplicating

There's a lock icon in the upper right of the `Arrangement View` for `Lock Envelopes`, if `Lock Envelopes` is *toggled off*:

- Moving the clip, will also move the automation data
- `⌘D` will duplicate the clip *and the Automation Data

### Master & Return Tracks

To add automation to master or return tracks, just open the disclosure triangle on those tracks in the session view.

## Session (Clip Automation)

Clip automation can either be `Modulation` or `Automation`. If a parameter doesn't support `Modulation` (e.g., like `Device On` which is a boolean value, so it can't be modulated), then only `Automation` will be visible. For parameters that support both, tabs below the graph editor allow switching between `Automation` and `Modulation`.

### Copy & Paste

- Clip automation can be cut and pasted by dragging out a selection over the enveloped and `right-click > Copy Envelope` (or just `⌘C`) and then `⌘V` to paste on another clip. Only the breakpoints need to be selected, e.g., if there's only single `Device On` breakpoint at the beginning of a clip, then only the section of the single breakpoint needs to be copied.

### Troubleshooting

- By default session automation is only turned on for armed tracks, which means MIDI clips will record automation by default, but Audio tracks will not. To change this, set `Preferences > Record > Record Session Automation in: All Tracks` (as opposed to `Armed Tracks`).

## Session to Arrangement

### Automation

- **Clip-based automation in the Session View is converted to track-based automation in the Arrangement View.** Automation sets the value of a parameter. Automation is clip-based in the Session View, because there's no lanes, whereas it's lane-based in the Arrangement View.
- Clip-based modulation stays as clip-based in the Arrangement View.
