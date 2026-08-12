# YT Clipper — release channel

Install files for [YT Clipper](https://github.com/snhuahmed/ytclip). Source lives
in a separate repository; this one exists to serve downloads.

## Install (Windows)

1. Download `ytclip-*-win.zip` from [Releases](../../releases/latest)
2. Right-click the zip → **Properties** → tick **Unblock** → OK
3. Extract it anywhere, then run `install.bat`
4. Follow the last step it prints: load the extension in Chrome, once

Nothing else to install — Node, yt-dlp and ffmpeg are all included.

### That last step, in full

Chrome only auto-installs off-store extensions on enterprise-managed machines,
so on a personal computer it has to be loaded by hand once:

1. Go to `chrome://extensions`
2. Turn on **Developer mode** (top right)
3. Click **Load unpacked**
4. Choose `%LOCALAPPDATA%\YTClipper\extension` — the installer puts this path on
   your clipboard, so you can paste it into the file picker

You will not need to repeat this. Updates replace that folder in place and Chrome
picks them up next time it starts.

## Using it

Open any YouTube video. A **Clipper** panel appears in the right sidebar.

- **In** / **Out** — type a time, or press the bracket buttons to use the
  playhead. The `I` and `O` keys do the same when the panel has focus.
- **Download clip** — saves exactly that range
- **Full video** — saves the whole thing, with no re-encoding at all

Files land in `Downloads\ytclip`.

## Removing it

Run `uninstall.bat` from the folder you extracted. Downloaded videos are left
alone.
