# Logic Pro Video

## Importing

To import a video, choose `File > Movie > Open Movie...`, you probably want to switch the project settings to match the video when Logic offers to do so.

- When you are opening the movie, you'll probably get alerts indicating that the sample rate and frame rate of the project don't match the movie. You'll probably want to select the options to use the frame rate and sample rate from the movie.

## Hiding & Showing

You can hide and show the preview by double-clicking the video track.

## Time

- Under `File > Project Settings > Synchronization...` you can set where the first bar (`1 1 1 1`) starts. It starts at one hour by default, which is a convention for video editing because it allows adding additional footage before the video starts (for slates, countdowns, and test signals).
- There doesn't seem to be anyway to automatically set a bar to an exact length, but you can simply enter a fractional value into the BPM field (and get the correct length through trial and error).

### Getting

A few methods for getting the SMPTE timecode:

- Open the file in QuickTime and activating `Edit > Trim...` (`⌘T`), clicking the right most trim handle will then show the timecode.
- Just move the playhead to the last frame of the video.
- Open the video in a video editor and view the timecode there.
