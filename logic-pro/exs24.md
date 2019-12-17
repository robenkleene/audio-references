# EXS24

If the edit button is missing, go to "Preferences > Advanced" and enable "Advanced Editing".

## Make an Instrument

The EXS24 has very flexible ways of working, this method is for making sample instruments that can than be imported into other platforms. There are other methods of saving instruments that for example prioritizing samples only being in a single location, this method prioritizes packaging up samples.

1. Open EXS24 and click the edit button in the upper left
2. Drag samples onto each key
3. Export the samples and save the instrument files: Go to "Instrument > Export Sampler Instrument and Sample Files", note that the instrument should be exported into the default `~/Music/Audio Music Apps/Sampler Instruments` path, otherwise they won't work to load back into the EXS24.

To load the instrument back into the EXS24 in Logic, just click the loaded preset in the display and select it.

## Ableton Live Import

To import the instrument into Ableton Live, since we usually just want to use the kit for a single project, the best method is to first copy the `.exs` file and samples into the Ableton Live project folder, so that that the samples are saved with the project. Then drag the `.exs` file into Ableton to import. After importing and loading the instrument as a Sampler track, there will be a file at `~/Music/Ableton/User Library/Sampler/Imports` which can simply be deleted.

## AudioLayer Import

To import to AudioLayer, in the iOS Files app, copy the folder with the `.exs` file and samples into the AudioLayer `import` folder. Then open the `.exs` file in the import folder from Files.

## Slicing a Loop

1. Select a region on an audio track and hit `w` to open the audio file editor.
2. Select "File" in the Audio File Editor, and turn on transient editing, and use the "+" and "-" buttons to change the sensitivity.
3. Right-click the region and select "Convert to Sampler Instrument"
4. For drum samples the "Create '1Shot' Zones" options is useful to make the whole sample play, regardless of how long the MIDI note is held down.
