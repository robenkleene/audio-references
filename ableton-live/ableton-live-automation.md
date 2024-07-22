# Ableton Live Automation

## Turning On

- `A`: Toggle `Automation` in the arrange view (if this isn't working, it's probably because `Options > Computer MIDI Keyboard` [keyboard icon in upper right] is toggled on, `M` to toggle off)
- Automation for clips is found under `Envelopes` tab along the top

## Editing

- `click`: Add / remove point
- `click&drag`: Move point
- `⇧click`: Move point or line
- `right-click` a parameter and choose `Show Automation` to make it automate-able
- To delete automation, right-click on a control and select `Delete Automation`
- To move all automation at once, right-click the track channel and select `Select all content` than move the cursor near the automation until the full automation highlights and click and drag the automation line up or down.

## Snap

- Turn off snap under `Options > Snap to Grid` (`⌘4`).
- Hold `⌘` to disable snap while dragging
- Constrain to one axis by holding `⇧` while dragging

## Graph Editor

- With the pointer tool enabled (toggle off the pencil tool with `⌘B`):
    - Click on a graph to add a point
    - Click on a point to delete a point
    - Drag a point to move it

## Clips


### Troubleshooting

- By default session automation is only turned on for armed tracks, which means MIDI clips will record automation by default, but Audio tracks will not.
- To fix this, set `Preferences > Record > Record Session Automation in: All Tracks` (as opposed to `Armed Tracks`)

## Master & Return Tracks

To add automation to master or return tracks, just open the disclosure triangle on those tracks in the session view.
