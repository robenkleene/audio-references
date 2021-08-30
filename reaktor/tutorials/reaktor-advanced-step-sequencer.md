# Reaktor Advanced Step Sequencer

## Clean Up

1. Start with the finished Basic Step Sequencer
2. Delete the `Order` and `Event Table` modules
3. Add an empty `Macro` and rename it to `Table`
4. Double-click into the `Table` and add `In` and `Out` ports
5. Go back up a level and connect the `StpFlt > Out` to the `Table > In` and the `Table > Out` to the `Out`.

## Interface

1. Double-click into `Table`
2. Add a `Mouse Area`
3. Add a new `Macro` and name it `Display` (this macro is to make sure the display stays below the mouse area and doesn't block input)
4. Double-click into `Display` and add a `Multi Display` (since the `Multi Display` is in a macro one level lower, it will be under the `Mouse Area`)
