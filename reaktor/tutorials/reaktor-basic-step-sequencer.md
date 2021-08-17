# Reaktor Basic Step Sequencer

## Test Tone

1. Create a new Ensemble
2. Add a `Sine Oscillator`
3. Add a `Button` and rename it to `Test Tone`
4. Connect the `Test Tone` output to the `Sine > A` input
5. Set `Test Tone > Properties > Range > On Value: 0.75` (this is to avoid an amplitude of `1` which can overload Reaktor)
6. Add a `Constant` and set its value to `60`, connect its output to the `P` input of `Sine`
7. Connect the `Sine > Out` output to the two `Out`
8. Now pressing the `Test Tone` button should toggle the tone

## Sequencer

1. Add a `Macro` and rename it to `Sequencer`

### Clock

1. Add a `Clock Oscillator` module to use as a clock source
2. Right-click the `Clock Osc > F` input and choose `Create Control`
3. Right-click the `Clock Osc > A` input and choose `Create Constant`
4. Add a `Separator` module, this will be used to filter out `0` events, so we can just use the output of `1` as our frequency
5. Connect the `Clock Osc > Out` output to the `Separator > In` input (and leave `Thld` disconnected because it defaults to `0`)
6. Add a `Counter`, connect the `Separator > Hi` output to the `Counter > Up` input

### Event Table

1. Add an `Event Table`
