# Logging

## Signal

- `snapshot~ 5 > print`

### Only Active

To log a signal only if it's `> 0`:

- `snapshot~ 5 > t f f`
- `> 0.`: Open `gate`
- `gate > print`