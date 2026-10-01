# VIDGET releases

**VIDGET is developed by 9,6Hz Agency.**

Official macOS Apple Silicon builds, macOS 13 or later. This repository contains installation/update binaries and instructions, not the development project, user data, signing keys or test media. Electron app bundles include their executable JavaScript/runtime assets and can be inspected.

## Install

Download the **VIDGET 0.5.0 macOS arm64 PKG** from [the latest release](https://github.com/tiennguyenbrb196-sys/vidget-releases/releases/latest). Quit older copies of VIDGET before installation. The package installs into `~/Applications/VIDGET.app` for your current account; no administrator access, GitHub login, Homebrew or developer tools are required. Open that installed copy after installation.

The official app and installer are Developer ID signed and notarized by Apple. Downloads, library, playlists, favorites, ratings, playback position and settings are stored outside the app bundle and retained.

**Users of 0.4.x:** install the first official PKG once. The older Apple Development release uses a different signing team, so a native update from 0.4.x to the official Developer ID build is not supported. After the first official installation, subsequent builds use the same Developer ID trust.

## Updates

In VIDGET, open **Cài đặt → Cập nhật app** or the application menu **Kiểm tra cập nhật**. Automatic checks run every six hours while the app is running and idle; automatic downloads are optional. Choose when to install. Install/relaunch waits for download/Studio tasks and active media playback to stop.

Update metadata and the entire ZIP are independently signed with Ed25519. The app verifies the embedded key, SHA256, size, repository URL, bundle ID/architecture and increasing build, then the native macOS installer verifies Apple code signatures. Clients do not need GitHub credentials or the private source repository.

Assets: first-install PKG, app/update ZIP, signed `update.json`, SHA256SUMS.txt. Updates use ZIP, not PKG for each version. Published assets are immutable; fixes use a higher build number. A source push alone does not update client machines.

Real build-machine package/signature/notarization checks do not replace acceptance on a second physical Mac. Download support varies by website; DRM is not supported.
