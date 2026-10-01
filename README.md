# VIDGET for macOS Apple Silicon

Download the app ZIP from [the latest release](https://github.com/tiennguyenbrb196-sys/vidget-releases/releases/latest), unzip, copy VIDGET.app into `~/Applications`, and open it. First installation may need approval in macOS Privacy & Security. The app is signed with Apple Development and is not notarized.

Version 0.4.0 (build 4) is the bootstrap for signed in-app updates. Older installations need this version or newer installed once. Then use Settings → Cập nhật app or the app menu → Kiểm tra cập nhật. Clients do not need GitHub login. Checks run every six hours; downloading automatically is optional. Installation waits while downloading/processing files or playing media. Local settings, download history, playlists and library stay in the same profile.

Update metadata and app archives carry Ed25519 signatures; the public key is embedded in the app. A valid SHA256 alone does not authorize an update. Apple code signing is also verified by the native installer. Release artifacts are immutable and build numbers only increase.

This repository contains release artifacts and instructions, not the development project, tests, Git history or signing keys. VIDGET is an Electron application: distributed app bundles include JavaScript/runtime assets and can be inspected. A private source repository is not copy protection.

Bundled third-party software includes Electron/Chromium, Node.js, yt-dlp, FFmpeg and libraries. Their licenses are included in the app. FFmpeg build is GPL; source and build formula: https://ffmpeg.org/download.html and https://formulae.brew.sh/formula/ffmpeg . yt-dlp: https://github.com/yt-dlp/yt-dlp . No credentials, user profiles or downloaded test media are included in releases.
