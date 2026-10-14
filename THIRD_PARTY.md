# Third-party components

Bass Forge's user interface, DSP, project format and orchestration are original
code licensed under MIT. The installer downloads the following independent
components and preserves their package notices. The custom rack is built in;
this version does not host external VST plug-ins.

| Component | Role | Upstream / license |
| --- | --- | --- |
| Python | Private runtime | https://www.python.org/ — PSF |
| PySide6 Essentials / Qt | Native widgets | https://doc.qt.io/qtforpython-6/licenses.html — LGPLv3/GPL/commercial options |
| NumPy / SciPy | Array math and filters | https://numpy.org/ / https://scipy.org/ — BSD |
| SoundFile / libsndfile | Audio files | https://github.com/bastibe/python-soundfile — BSD / LGPL |
| sounddevice / PortAudio | Local audio playback | https://github.com/spatialaudio/python-sounddevice — MIT |
| Demucs | Trained bass separation | https://github.com/facebookresearch/demucs — MIT |
| PyTorch / torchaudio | AI inference | https://pytorch.org/ — BSD-style |
| yt-dlp / EJS | YouTube import | https://github.com/yt-dlp/yt-dlp — Unlicense; EJS also includes MIT/ISC components |
| Deno | YouTube challenge runtime | https://deno.com/ — MIT |
| Microsoft VC runtime | Native Windows libraries | Microsoft VCLibs Desktop redistributable, downloaded from Microsoft |
| imageio-ffmpeg / FFmpeg | Decode and MP3 export | https://github.com/imageio/imageio-ffmpeg — BSD wrapper; FFmpeg build licensing applies |

Python packages and their transitive dependencies are installed under
`%LOCALAPPDATA%\BassForgeStudio\runtime\Lib\site-packages`; their license and
dist-info records remain there. Qt libraries are dynamically loaded and are
not embedded into the application executable; they can be replaced with
compatible builds. The complete application source is provided. FFmpeg builds
are supplied by imageio-ffmpeg, with provenance and source information in that
project. Model files are fetched by Demucs from its upstream model host.

Technical references used for this build:

- https://github.com/facebookresearch/demucs/blob/main/README.md
- https://github.com/yt-dlp/yt-dlp/wiki/EJS
- https://pytorch.org/get-started/previous-versions/
- https://docs.python.org/3.12/using/windows.html#the-embeddable-package

Only import audio you are entitled to download and edit. The app does not
bypass DRM, paywalls, sign-in requirements or access restrictions.
