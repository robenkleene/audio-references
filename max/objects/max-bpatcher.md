# Max `bpatcher`

## Arguments

- In the Inspector, for the `bpatcher` object (e.g., in the patcher *containing* the `bpatcher`), set the `Argument(s)` field.
- In the `bpatcher` the arguments can then be used as `#1`, e.g., in messages, but also for `Short Name`, `Long Name`, and `Scripting Name`, but *only* at the beginning (e.g., `#1-foo`)
- The `#1` can also be used in the arguments list, e.g., so a parent `bpatcher` can pass its argument to a child `bpatcher`

## Troubleshooting
