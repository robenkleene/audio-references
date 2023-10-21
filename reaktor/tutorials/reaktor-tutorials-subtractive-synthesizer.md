# Reaktor Subtractive Synthesizer

## Setup

1. Choose `File > New Ensemble`
2. Choose `Library > 02 - Oscillator > OSC Sync`
3. Choose `Library > 04 - LFO, Envelope > AHDSR`
4. Connect `OSC Sync HQ > Out` to `AHDSR > In`
5. Connect `AHDSR > Out` to `Out 1` and `Out 2`

## Cleanup Panel

1. Unlock the `Panel` by clicking the padlock icon
2. Drag the `AHDSR` below the `OSC Sync HQ`

    ![Panel](assets/reaktor-subtractive-synthesizer-panel.png)

3. Lock the `Panel` again by clicking the padlock icon

## MIDI

1. Open the search box (`↩`) and add a `Pitch and Gate (09 - Utility, Display)`
2. Connect the `Pitch and Gate > P` output to the `OSC Sync HQ > P` input, and the `Pitch and Gate > G` output to the `AHDSR > G` input.
3. Clean up the panel, by unlocking and dragging the elements so they aren't overlapping.
4. The keyboard can now be played if `Options > MIDI Keyboard Activated` is toggled on (try hitting the `S` key)

*Stopped this tutorial at this point, because this was all I needed for now