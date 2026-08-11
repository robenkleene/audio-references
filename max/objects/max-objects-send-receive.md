# Max Send Receive

- Double-clicking a `send` or `receive` object will show a menu of all the corresponding objects with the same destination (i.e., to quickly find the other objects in a send and receive pair)
- Use `s #0scales` and `r #0scales` to assure sends and receives are unique per instance of a patcher.
- Note that while Max for Live supports `#0` it is not guaranteed to be unique across *different devices*. In Max for Live there is `---` that can be used instead, but that is unique across *devices but not patcher instances*. You can work around this by using something like `---_<unique-instance-id>` (e.g., `---_foo`) as an argument to a `bpatcher`, but in general the best approach is to use patch chords where possible to avoid these issues.
