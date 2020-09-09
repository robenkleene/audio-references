# Modular Synth

- **EOC**: End of cycle (used as a trigger?)
- **Reset**: In a sequencer, this generally means reset the sequencer back to the first beat
- **Multiple**: Take a signal as input and give several outputs of the same signal. There are "passive" and "active" multiples, passive multiples just split signals, which means there's some loss in voltage strength, whereas active multiples (usually a "Buffered Multiple") maintain the voltage strength.

## Using Envelopes

- With a **Gate**, use a ADSR, this is because a gate sends a sustain signal, replicating a note.
- With a **Trigger**, use a AD, this is because a trigger just sends singe burst.