# Max Presets

The strategy for presets with Max for Live:

1. Have the `pattrstorage` system only read and write JSON files
2. Store the current state with Ableton Live

## Presets Object

- `⇧-click`: Save current preset
- `click`: Restore preset
- `⇧⌥-click`: Delete preset

## Troubleshooting

### Saving Empty Values

If saving a preset is just saving an empty value (i.e., `[]`) in the presets JSON file, the reason is simply that that value is empty in the stored preset. I.e., when saving, the stored preset is saved, which will be missing a parameter if that parameter was added after the preset was saved.

The workaround here is usually to re-save each individual preset (by clicking the preset to load it, then `⇧-click` to re-save the preset), and then saving again.