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

## Clean Up

1. Unlock the panel
2. Toggle off `Multi Display > View > Show Label`
3. Set `Macro > View > Frame: None`
4. Move the panel elements so the `Table` and `Rate` are no longer overlapping
5. Set `Mouse Area > View > Width (Pixels): 300`
6. Set `Multi Display > View > Width (Pixels): 300`

    ![Display](assets/advanced-step-sequencer/reaktor-advanced-step-sequencer-display.png)

## Wiring Together

1. Double-click into the `Display` macro, add two `In` ports and name them `X` and `Y`
2. Go back up a level to `Table` and connect the `Mouse Area` `X` & `Y` outputs to the `Display` `X` & `Y` inputs
3. Go back into the `Display` and wire up `X` and `Y` as follows:

    ![X & Y](assets/advanced-step-sequencer/reaktor-advanced-step-sequencer-x-y.png)

    The second output of the `Order` module for the `Y` value is used to ensure it's processed after the `Idx` is set.
