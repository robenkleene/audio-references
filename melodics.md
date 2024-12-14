# Melodics

After initial setup, most of the settings persist. To send MIDI to Melodics again:

1. Launch Live, and on the MIDI track channel strip, choose `MIDI To > IAC Driver`
2. Make sure the device is selected in Melodics under `Audio & Devices > Connected instruments > Selected instrument: Virtual MIDI Bus`

## Initial Setup

### Ableton Live

1. Connect Push and turn on Live
2. Push the scale button and toggle `In Key` to `Chromatic`

### Audio MIDI Setup

1. Open `Audio MIDI Setup`
2. Choose `Window > Show MIDI Studio`
3. Double-click `IAC Driver`
4. Choose `Ports > Bus 1` (add a port if it's missing), and toggle on `Device is online`

### Ableton Live

1. In Live's preferences, toggle off `Input > IAC Driver > Track` (a feedback loop will happen if this isn't toggled off), and toggle on `Output > IAC Driver > Track`.
2. For the MIDI track channel strip in Live, choose `MIDI To > IAC Driver`

### Melodics

1. Install the `virtual-midi-bus.json` device at `~/Library/Application Support/Melodics/Melodics/devices`.
2. In Melodics settings, set `Audio & Devices > Connected instruments > Selected instrument: Virtual MIDI Bus`

### Device JSON

``` json
{
    "version": 3,
    "name": "Virtual MIDI Bus",
    "layouts": [
      {"instrument":"keys", "layout":"88"}
    ],
    "ports": {
      "mac_regex": "^IAC Driver.*$",
      "win_regex": "^loopMIDI.*$"
    },
    "inputs": [
      { "channel": 1, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 2, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 3, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 4, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 5, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 6, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 7, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 8, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 9, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 10, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 11, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 12, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 13, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 14, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 15, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] },
      { "channel": 16, "instrument": "keys", "events": [ { "type": "NoteOn" }, { "type": "NoteOff" } ] }
    ]
  }
```
