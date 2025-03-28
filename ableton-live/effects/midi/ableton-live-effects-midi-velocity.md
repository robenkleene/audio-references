# Ableton Live Effects Midi Velocity

- `Out Low` / `Out Hi`: Set the minimum and maximum output velocity, any incoming note is re-mapped into this range (for example, with an `Out Low: 64` and `Out Hi: 127`, then an incoming velocity of `1` becomes `64` and an incoming note of `64` becomes `95` [`64` is halfway between `1` and `127` and `95` is halfway between `64` and `127`])
- `Lowest` / `Range`: Controls the incoming range is remapped based on the `Mode` setting. `Clip` forces notes higher or lower into the range, `Gate` filters out notes that aren't in the range, and `Fixed` forces all notes to use the `Out Hi` velocity
- The X-Y display shows how an incoming velocity is mapped to a new value, the X-axis is the incoming velocity and the Y-axis is the remapped value
- `Random`: Adds or subtracts a value from the outgoing velocity, this is represented by the gray area in the X-Y display
- `Comp.` ("Compand"): Lower values make notes more likely to be in the middle of the range, and higher values make notes more likely to be at the ends of the range
- `Drive`: Forces the middle of the velocity curve higher or lower
