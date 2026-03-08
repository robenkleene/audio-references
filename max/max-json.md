# Max JSON

## `grep`

`grep` commands to find common settings to clean up.

- `grep -E "default_fontsize|default_fontname" *.maxpat`: Font override (can be deleted)
- `grep -E "fontsize|fontname" *.maxpat`: Font override (can be deleted)
- `grep '"gridsize"' *.maxpat`: Grid size setting (can be deleted)
- `grep '"gridsnaponopen"' *.maxpat`: Snap to objects setting (can be deleted)
- `grep '"objectsnaponopen"' *.maxpat`: Snap to objects setting (can be deleted)
- `grep 'patching_rect.*25.0, 25.0' *.maxpat`: Too small inlets and outlets (should be `30.0`)