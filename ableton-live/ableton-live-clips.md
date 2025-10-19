# Ableton Live Clips

## Follow Actions

`Follow Actions` are used to perform an action after a clip plays.

In the `Clip View`, open the `Launch` section of the clips settings, and toggle on `Follow Action`. To play the next clip in the scene when this one ends, choose `Next` for the action (or `Previous` for the previous clip).

- If a `Follow Action` is setup on a clip, the clip's play button icon will have lines through it on the `Session View`
- If a clip is going to play next after a `Follow Action` conditions are met, then its play icon will flash in the `Session View`
- `Linked` / `Unlinked`: When set to linked, a multiplier can be set that determines how many times the clip plays before the Follow Action is triggered. When set to `Unlinked` a number of bars can be chosen instead.
- Follow actions *do not trigger unless there's an explicit launch event to start the timer*, e.g., this means if a Live set is saved with the play button active on a clip, then the live set is opened again, the global transport play button is clicked, then that clip's Follow Actions *will not trigger*, but if that clip's play button is then clicked again (i.e., an explicit launch event) then that clip's follow action timer will start and *the follow action will trigger*.
- The timer for a Follow Action is setup *when the launch event happens*, e.g., if you click the play button for a clip, and then change the timing setting for the follow action, that timing change won't be incorporated *until the clip is launched again*.
