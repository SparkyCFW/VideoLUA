# VideoLUA /Studio

**Portable video and GIF conversion for EdgeTX Lua widget animations — now available for Windows and macOS.**

VideoLUA /Studio is a free desktop utility that prepares video frames and Lua animation assets for EdgeTX color-screen radios. Import a video or animated GIF, preview your edits, then export the frames and Lua script for your EdgeTX widget.

## Features

- Import videos and animated GIFs; queue and reorder multiple files for batch conversion.
- View original and processed previews while adjusting your output.
- Trim clips using an interactive timeline, with playback and scrubbing.
- Rotate videos and resize or reposition the crop directly in the preview.
- Choose device-oriented output presets, custom dimensions, and frame rates.
- Scale using **Fit**, **Stretch to Fill**, or **Crop to Fill**.
- Export BMP frame sequences or **experimental transparent PNG** frames.
- Export widget files as a ZIP or extracted folders.
- Run conversions locally without requiring an internet connection.

PNG transparency works, but device, firmware, and widget support vary. Test exported PNG animations on your target radio before relying on them.

## Download

Get the latest published files from **[VideoLUA /Studio — GitHub Releases](https://github.com/SparkyCFW/VideoLUA/releases)**.

| Platform | Download | Notes |
| --- | --- | --- |
| **Windows x64** | `VideoLUA.exe` | Portable; Windows release **v1.0.0** |
| **Mac — Apple Silicon** | `VideoLUA-v0.9.0-macOS-arm64.dmg` | For M-series Macs; macOS **14+** |
| **Mac — Intel** | `VideoLUA-v0.9.0-macOS-x64.dmg` | For Intel Macs; macOS **14+** |

**Version note:** The existing Windows release is **v1.0.0**. The macOS applications identify themselves as **v0.9.0**, even if their installers are attached to the same GitHub release.

### Windows installation

1. Download `VideoLUA.exe` from the release assets.
2. Put it in a folder of your choice and run it. No installer is required.

The Windows x64 release includes the .NET runtime and FFmpeg. It does not require a separate .NET or FFmpeg download and is designed for offline use. Some packaged components may be extracted to a temporary directory at runtime.

### macOS installation

1. Download the DMG matching your Mac: **ARM64** for Apple Silicon, or **x64** for Intel.
2. Open the DMG and drag `VideoLUA.app` into **Applications**.
3. Open VideoLUA from Applications.

The macOS releases are self-contained and include the .NET runtime, FFmpeg, and FFprobe. **Homebrew, FFmpeg, and .NET do not need to be installed separately.**

**macOS security notice:** These builds are **ad-hoc signed, not Apple Developer ID signed or notarized**. macOS may block the first launch. If you downloaded VideoLUA from this official release and trust the file, try opening the app once, then go to **System Settings → Privacy & Security → Open Anyway** and confirm. Do not globally disable Gatekeeper. Managed Macs may prevent this override.

## How to use

1. Import a video or animated GIF. You can add multiple files to the media queue.
2. Select a device preset or enter custom output dimensions and FPS.
3. Adjust trimming, crop, rotation, and scaling while checking the previews.
4. Choose BMP frames or PNG transparency, then select ZIP or folder export.
5. Export your files and copy the generated Lua widget and frames to your EdgeTX setup.

Output compatibility depends on your target radio, EdgeTX firmware, and widget configuration. Check memory usage, playback smoothness, and transparency on the actual device.

## Compatibility and testing

- **Windows:** Portable Windows x64 application.
- **Apple Silicon:** ARM64 build tested on an Apple Silicon M4 Mac.
- **Intel Mac:** x64 build tested under Rosetta on an M4 Mac and passed automated native-Intel build and verification tests. It has **not** been manually tested on physical Intel Mac hardware.
- **macOS:** Requires macOS 14 or newer.

## License and third-party software

Copyright (c) 2026 **SparkyCFW**.

VideoLUA /Studio is distributed as freeware. The original **Windows application is proprietary software**, and its source code is not publicly distributed. See [LICENSE.txt](LICENSE.txt) for the original application's terms. The macOS version is maintained as a separate implementation; its source repository and its distribution terms should be reviewed separately.

VideoLUA uses third-party components under their own licenses, including **FFmpeg** and the **Microsoft .NET runtime**. The Windows portable executable includes an FFmpeg GPLv3 build and a self-contained .NET 10/WPF runtime; see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) and [COPYING.GPLv3.txt](COPYING.GPLv3.txt). The macOS application bundles its FFmpeg license and source materials inside the application at `VideoLUA.app/Contents/Resources/ThirdParty/FFmpeg/`.

These third-party rights are independent of VideoLUA's application license.

## Support

Report bugs and request features through the repository's **[Issues](https://github.com/SparkyCFW/VideoLUA/issues)** tab. Please include your operating system, whether your Mac is Intel or Apple Silicon, the input format, output settings, and steps to reproduce the issue.
