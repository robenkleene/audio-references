# Max Rewire

I've given up trying to get Max to sync with Logic Pro via ReWire because it's just not worth the headaches, but this is a summary how far I've gotten:

1. In order to get ReWire to start syncing, "Options > Audio Status..." has to be set to `ad_rewire`. (There are some UI nicety with `dac~` and `ezdac~` to help with this.)
2. A `metro` is generally used to drive a `transport` with `clocksource rewire` set to get up-to-date transport information, e.g., to power a `live.step`.

The problems:

1. At it's most basic, I haven't found a way to get start and stop messages from the ReWire host, which alone makes the whole premise DOA.
2. Each time Logic Pro loops, a new global transport is created, when that happens the `metro` stops (why?).

So even if I require manually triggering a button in Max when Logic Pro's transport has started, which I'd have to do because I can't receive start and stop messages, then I'd have to trigger that button again each time Logic loops.

You can simply create a `metro` that constantly polls the `hostsync~` for the status, but aside from that being sloppy programming, it also causes performance issues when syncing in practice.

It's better just to get on with your life and use another piece of software like Reaktor that actually wants to support your use case. This entire situation isn't worth your time.