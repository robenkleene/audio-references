# Logic Pro Automation

- `⌃⌘⌫`: Delete visible automation for track
- `⌥Click` a point to select all points afterwords (this is the easiest way to select all automation for a track)
- Double-click an automation point to delete it.
- There are various options for deleting automation under "Mix > Delete Automation".

## Recording

Display automation (`A`) and switch from `Read` to `Touch`, when `Touch` is set, any values changed will automatically be written to automation, regardless of which parameter is currently selected (a parameter being edited will automatically be selected), and regardless of whether record is enabled. Switch back to `Read` after you've finished recording.

## Move Automation

To move automation between two parameters, select the source parameter, then hold `⌘` while switching to the destination parameter, and a dialog will pop-up offering to move the automation.

## Region

To create region-based automation:

1. Create a MIDI region
2. Show Automation (`A`)
3. Switch `Track` to `Region`

## Troubleshooting

- If your region-based automation isn't catching, try just moving the position of the first node a bit forward.
