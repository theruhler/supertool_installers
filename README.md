# FreeEd4Med Media SuperTool — Downloads

A desktop app for musicians and content creators: lyric videos, audio
visualizers, AI transcription, stem separation, notation, social-media
exports and more, all in one window.

This page only hosts the installers. Each release is built automatically from
the FreeEd4Med source code and published here unchanged.

## Download

Get the newest version for your computer:

| Your computer | Download |
|---------------|----------|
| Windows (64-bit) | [FreeEd4Med-SuperTool-Setup.exe](https://github.com/theruhler/supertool_installers/releases/latest/download/FreeEd4Med-SuperTool-Setup.exe) |
| Mac with Apple Silicon (M1 or newer) | [FreeEd4Med-SuperTool.dmg](https://github.com/theruhler/supertool_installers/releases/latest/download/FreeEd4Med-SuperTool.dmg) |
| Linux (64-bit) | [FreeEd4Med-SuperTool-x86_64.AppImage](https://github.com/theruhler/supertool_installers/releases/latest/download/FreeEd4Med-SuperTool-x86_64.AppImage) |

Older versions and release notes are on the [Releases page](https://github.com/theruhler/supertool_installers/releases).

The downloads are large (about 280–380 MB) because everything the app needs,
including `ffmpeg`, is built in. You don't need to install Python or any other
tools first.

The Mac version doesn't run on older Intel Macs yet.

## Install

### Windows

1. Run `FreeEd4Med-SuperTool-Setup.exe`.
2. If Windows shows "Windows protected your PC", click **More info**, then
   **Run anyway**. (This appears because the installer isn't code-signed yet.)
3. Follow the installer. It adds a desktop shortcut and a Start menu entry.

### macOS

1. Open `FreeEd4Med-SuperTool.dmg` and drag **FreeEd4MedSuperTool** into
   **Applications**.
2. The first time, **right-click** (or Control-click) the app and choose
   **Open**, then click **Open** again. (macOS asks because the app isn't
   signed by Apple yet.) After that it opens normally.
   You can also go to **System Settings → Privacy & Security** and click
   **Open Anyway**.

### Linux

1. Make the file executable and run it:
   ```
   chmod +x FreeEd4Med-SuperTool-x86_64.AppImage
   ./FreeEd4Med-SuperTool-x86_64.AppImage
   ```
2. If you get a FUSE error ("cannot mount AppImage"), run it like this instead:
   ```
   ./FreeEd4Med-SuperTool-x86_64.AppImage --appimage-extract-and-run
   ```

### After installing

The main features work straight away. Optional heavy tools (Whisper
transcription, Demucs stem separation, Ardour, MuseScore) can be added from
the app's **Setup Studio Tools** page whenever you need them. No admin rights
are needed for those.

## Check your download (optional)

Every release includes a `SHA256SUMS.txt` file. Comparing your download
against it confirms the file arrived complete and unchanged. Put
`SHA256SUMS.txt` in the same folder as the installer, then run:

- **Windows (PowerShell):** `Get-FileHash FreeEd4Med-SuperTool-Setup.exe` and
  check that the value matches the line for that file in `SHA256SUMS.txt`
  (capital or small letters don't matter).
- **macOS:** `shasum -a 256 -c --ignore-missing SHA256SUMS.txt`
- **Linux:** `sha256sum -c --ignore-missing SHA256SUMS.txt`

On macOS and Linux, the word `OK` next to the file name means it matches.

Only download the installers from this page or from a link on the official
FreeEd4Med website.

## License

Copyright © 2026 FreeEd4Med Corp. Licensed under
[CC BY-NC-ND 4.0](LICENSE.md): free to use and share unchanged for
noncommercial purposes. Commercial use needs written permission from
FreeEd4Med Corp.
