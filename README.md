# Bass Forge

A Windows bass remix studio: import a YouTube link or audio file, separate
the bass locally, shape it with custom effects and a graphic EQ, and export.

## Download 1.0.1

**[Download BassForge.exe](https://raw.githubusercontent.com/Paralied/BassForgePublic/main/releases/v1.0.1/BassForge.exe)** — Windows 10/11 x64.

Run the EXE. The setup dashboard shows every stage, live activity and download
progress. First setup downloads the audio tools and local AI engine; allow
several GB of disk space and an internet connection. No Python installation,
account, API key or paid service is needed. The app is currently unsigned.

## Updates inside the app

Click **Check for updates → Download update → Install & restart**. Bass Forge
checks this repository, verifies the downloaded installer, asks you to save
any unsaved session, and opens the visible setup screen. Existing tools and
models are reused. Version 1.0.0 needs this download once to gain the updater.

## Included

- Local bass separation with Demucs; a two-stem waveform editor and looping.
- 12-band graphic EQ, sub boost, rumble cut, low-band saturation, mono lows,
  compressor, master limiter, presets, live spectrum and meters.
- WAV, FLAC and MP3 export; self-contained saved projects.
- A built-in demo to try the effects immediately.

If setup pauses, use **Copy details** or **Open log** in the setup window.
Run the EXE again to retry. Use the Issues tab to report problems.

See [changes](CHANGELOG.md), [third-party notices](THIRD_PARTY.md), and
[download checksum](releases/v1.0.1/SHA256SUMS.txt).

This repository distributes Windows builds and update metadata. Development
is maintained in the owner's private BassForgePrivate repository. The app's
Python implementation is included in its installer payload.
