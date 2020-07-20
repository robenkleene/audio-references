# Reaktor Setup Spiral

1. In the Reaktor standalone app, drag "Reaktor Factory Library > Sequenced Synthesizers > Akkord.ens" onto the canvas.
2. Make sure "Edit" button in the upper left is turned on. Click on the name of the ensemble (`Akkord 1.3`) to enter the structure editor.
3. Select the `AKKROD-SEQ` and delete it.
4. Drag an instance of `Spiral.ens` in to replace it. You don't have to wire Spiral to anything since it generates MIDI.
5. Click "Panel" in the breadcrumbs to go back to the panel view and drag `AKKORD` down below Spiral.
6. Click Spiral to select it and go to "Properties > Connect" in the sidebar (it should say "Instrument: `Spiral`" up top). In "MIDI OUT", set "Internal: `AKKORD`".