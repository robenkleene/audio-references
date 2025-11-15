# Max for Live Coding Guidelines

- Use `CamelCase` (not `snake_case`) for patcher names
- Sub-patcher and script files start with an upper case (e.g., `FooBar`)
- When the name contains an abbreviation, capitalize only the first letter (e.g., `FlowLcd`)
- These same guidelines apply to `Scripting Name` (i.e., first-letter capitalized `CamelCase`)

## Inlets & Outlets

- Schema: `(type(s), unit, range) description per list element`
- `unit` and `range` are optional (and only used for `int` and `float`)

### Examples

- `(float, ms) attack`
- `(float, 0 - 1) sustain`
- `(symbol) new track name`
- `(float float, %) x, y`
- `(int float symbol) id, amount, key`
- `(list) all filter coefficients <= if the list length is not fixed and/or the list is long`

## Acronyms

- **Amp**
- **Amt**
- **Dur**
- **Env**
- **Filt**
- **Freq**
- **Osc**
- **Semi**
