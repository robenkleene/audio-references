# Phrase Seq 16

- **Attach**: Edit the currently playing note
- **Len / Mode**: Set the current sequence (starting state), length of a sequence (second state), or the mode (third state)
- **Tran / Rot**: Transpose or rotate the current sequence
- **Copy-Paste**: copy sequence then switch to another sequence and past. (You can’t copy in attach mode?)
- The slide duration can range from 0 to T seconds, where T is the duration of a clock period (the default is 10% of T)
- **Gate 1** / **Gate 2**: Whether the current step is on or off for that gate
- Tied note is just a held note

## Modes

The mode determine how the steps are traversed.

- **FWD**: Forward
- **REV**: reverse
- **PPG**: ping-pong, also called forward-reverse
- **PEN**: pendulum, like PPG but the first and last steps are not played twice
- **BRN**: Brownian random
- **RND**: random
- **FW2**: forward, play twice
- **FW3**: play three times
- **FW4**: four times

For example, setting the run mode to FWD for sequences and to RND for the song will play the phrases that are part of a song randomly, and the probability of a given phrase playing is proportional to the number of times it appears in the song. For sequences, the FW2, FW3 and FW4 modes can be used to repeat sequences more easily without consuming additional phrases in the song. These last three modes are not available for the song's run mode however. Holding the MODE button for two seconds allows the selection of the clock resolution, and is the mechanism used to enable the advanced gate mode.

## Copy-Paste

- When ALL is selected, the run mode and length are also copied for a sequence?
- **4** / **8** / **All**: Pastes to the 4th or 8th step?

## Changing the Sequence via MIDI

By default "SEQ #: 1-16" are mapped to `0-10V`. To configure it to more easily map to MIDI notes, right-click and select "Seq CV in: 0-10V, <C4-D5#>, Trig-Incr". It doesn't look like there's any way to see which state this setting is in, but clicking it once seems to put it into the note mode.

In the note mode `C3` will be "SEQ #: `1`" and `C3#` will be "SEQ #: `2`". `D4#` is "SEQ #: `16`"