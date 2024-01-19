# Max Tasks Gain

`live.gain~` has a `Unity Style: Loudness (dB)`, but if you use a `*~`, then the signal won't be adjusted by the appropriate amount (the magnitude of a `-70 dB` signal will be greater than `0 dB` for example).

This is because `live.gain~` is output in logarithmic scale, while `*~` expects a value from `0` to `1`.

The solution is to convert the output of `live.gain~` to a `0` to `1` range value, this is done by passing its output through an `expr pow(10., $f1 / 20.)` object.
