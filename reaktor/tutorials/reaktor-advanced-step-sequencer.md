# Reaktor Advanced Step Sequencer

1. Start with the finished Basic Step Sequencer
2. Delete the `Order` and `Event Table` modules
3. Add an empty `Macro` and rename it to `Table`
4. Double-click into the `Table` and add `In` and `Out` ports
5. Go back up a level and connect the `StpFlt > Out` to the `Table > In` and the `Table > Out` to the `Out`.
