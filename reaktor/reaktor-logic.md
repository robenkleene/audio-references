# Reaktor Logic

To change snapshots via a MIDI region, send a program change.

1. Create a MIDI region.
2. Toggle on the `List Editors` icon in the upper right (`D`), and select the `Event` tab.
3. Next to the `Create new event` plus button, select `Progr. Change` as the event type, then hit the plus button.

## Automation

To show program change automation for a region:

1. Select the MIDI region and view the Editor (`E`).
2. Make sure automation is visible in the Editor by clicking the `Show/Hide Automation` icon in the Editor toolbar (`A`).
3. Make sure `Region` is selected in the `Automation/MIDI` area, and choose `Program Change` from the parameter pop-up menu.

### Program Change

- `Num` corresponds to Banks
- `Val` corresponds to Snapshots

#### Tips

- Logic starts its numbering schemes from `0` whereas Reaktor starts them from `1`. So for bank and snapshot numbering, subtract one from the Reaktor value to get the Logic value.