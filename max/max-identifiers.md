# Max Identifiers

- In messages `$1`, `$2`, etc... get replaced by arguments in an incoming list.
- Using `#0` at the start of a variable name gets replaced by a unique identifier at runtime. E.g., to use multiple copies of the same patch that use `send` and `receive`. (Note that this is only `#0`, `#1`, `#2`, etc... behave differently).
- Using `pattrforward` is another good alternative to `send` / `recieve`, you can even `pattrforward` to a `t b` to send a bang
- Using `pvar` is often another good alternative to `send` / `recieve`
- Note that while Max for Live supports `#0` it is not guaranteed to be unique across *different devices*. In Max for Live there is `---` that can be used instead, but that is unique across *devices but not patcher instances*. You can work around this by using something like `---_<unique-instance-id>` (e.g., `---_foo`) as an argument to a `bpatcher`, but in general the best approach is to use patch chords where possible to avoid these issues.
- The best system for having a unique identifier for both Max for Live and Max is to have the top-level instrument pass `---` for Max for Live and `#0` for Max to all `bpatcher` and patchers that need send and receive, and then use `s #1-<identifier>` and `r #1-<identifier>`. This approach works for multiple devices. For multiple patcher instances, add a unique identifier to each `bpatcher` argument, e.g., pass in `#1_0`, `#1_1`, etc...
