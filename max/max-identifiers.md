# Max Identifiers

## Special

- In messages `$1`, `$2`, etc... get replaced by arguments in an incoming list.
- Using `#0` at the start of a variable name gets replaced by a unique identifier at runtime. E.g., to use multiple copies of the same patch that use `send` and `receive`. (Note that this is only `#0`, `#1`, `#2`, etc... behave differently).
- Note that while Max for Live supports `#0` it is not guaranteed to be unique across *different devices*. In Max for Live there is `---` that can be used instead, but that is unique across *devices but not patcher instances*. You can work around this by using something like `---_<unique-instance-id>` (e.g., `---_foo`) as an argument to a `bpatcher`, but in general the best approach is to use patch chords where possible to avoid these issues.
