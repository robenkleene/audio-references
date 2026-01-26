# Max for Live Coding Guidelines

- Use `CamelCase` (not `snake_case`) for patcher names
- Sub-patcher and script files start with an upper case (e.g., `FooBar`)
- When the name contains an abbreviation, capitalize only the first letter (e.g., `FlowLcd`)
- These same guidelines apply to `Scripting Name` (i.e., first-letter capitalized `CamelCase`)
- Check the Max for Live project by choosing `Edit in Max` (or just opening the `.amxd` file in Max) then choosing `Show Containing Project`

## Inlets & Outlets

- Set the assistance comment
- Schema: `(type(s), unit, range) description per list element` (`unit` and `range` are optional and only used for `int` and `float`)

### Examples

- `(float, ms) attack`
- `(float, 0 - 1) sustain`
- `(symbol) new track name`
- `(float float, %) x, y`
- `(int float symbol) id, amount, key`
- `(list) all filter coefficients <= if the list length is not fixed and/or the list is long`
- These are examples from Ableton's coding guidelines, but in practice capitalization is inconsistent

## Acronyms

Only use these abbreviations.

- **Amp:** Amplifier
- **Amt:** Amount
- **Ch:** Channel
- **Dur:** Duration
- **Env:** Envelope
- **Filt:** Filter
- **Freq:** Frequency
- **Man:** Maximum
- **Min:** Minimum
- **Mod:** Modulator
- **Osc:** Oscillator
- **Param:** Parameter
- **Pch:** Pitch
- **Rand:** Random
- **Semi:** Semitones
- **Trig:** Trigger
- **Val:** Value
- **Vel:** Velocity
- **Vol:** Volume

Use abbreviations in the `Short Name`, `Long Name`, and `Scripting Name`, but *not* in the `Hit` or `Info View Text`.

## Documentation

Use the `Info View Text` field to provide a text description of each parameter (the `Hint` field does not appear to be necessary).
