# Ableton Live User Library

- The library can be reset by deleting, `~/Library/Application\ Support/Ableton/Live\ Database/Live-files-12107.db`
- Don't make `User Library` a symlink, otherwise there will be problems recreating the library if the `.db` file is deleted
- Ableton Live should try and recreate the library on launch after deleting the `.db` file
