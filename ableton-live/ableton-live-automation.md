# Ableton Live Automation

- You can show automation by a control either by changing its value, or, to show automation without changing the current value, right-click the control and choosing `Show Automation`
- If automation is just setting a parameter to a single value (e.g., `Device On`), then you only need one point at the beginning (e.g., a second point at the end isn't necessary)

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

### Copy & Paste

- Clip automation can be cut and pasted by dragging out a selection over the enveloped and `right-click > Copy Envelope` (or just `⌘C`) and then `⌘V` to paste on another clip. Only the breakpoints need to be selected, e.g., if there's only single `Device On` breakpoint at the beginning of a clip, then only the section of the single breakpoint needs to be copied.

### Troubleshooting

- By default session automation is only turned on for armed tracks, which means MIDI clips will record automation by default, but Audio tracks will not. To change this, set `Preferences > Record > Record Session Automation in: All Tracks` (as opposed to `Armed Tracks`)
