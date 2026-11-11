# VideoLUA /Studio

**Portable video and GIF conversion for EdgeTX Lua widget animations.**

VideoLUA /Studio is a free, closed-source Windows desktop utility for preparing video frames and generating animation assets for EdgeTX Lua widgets.

## Features

- Import videos and animated GIFs; queue multiple media files
- Original and processed previews with timeline trimming
- Crop and rotation controls, device-oriented output presets
- Scaling modes: **Fit**, **Stretch to Fill**, and **Crop to Fill**
- Export BMP frame sequences and experimental transparent PNG frames
- Batch processing and dark/light interface themes

## Download

Download **VideoLUA.exe** from [GitHub Releases](https://github.com/SparkyCFW/VideoLUA/releases) when a release is available. The Windows x64 executable is designed to run without an installer, separate .NET installation, or separate FFmpeg download. It can be copied to a USB drive and used offline. Some components may be extracted to a temporary folder at runtime.

## Use

1. Open `VideoLUA.exe`.
2. Import a video or animated GIF.
3. Choose output dimensions or a preset, then adjust trim, crop, rotation, and scaling.
4. Review the processed preview and export your frame assets.
5. Integrate the exported assets into your EdgeTX Lua widget project.

Output compatibility depends on the target device, firmware, and widget. PNG transparency is experimental.

## License and third-party software

Copyright (c) 2026 **SparkyCFW**. VideoLUA /Studio is **proprietary freeware**; its application source code is not publicly distributed. See [LICENSE.txt](LICENSE.txt).

The portable executable includes **FFmpeg** (GPLv3) and a self-contained **Microsoft .NET 10/WPF runtime**, which have separate license terms. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) and [COPYING.GPLv3.txt](COPYING.GPLv3.txt). These third-party terms are not superseded by VideoLUA's proprietary license.

## Support

Use the repository's **Issues** tab for bugs and feature requests. Please include your Windows version, input format, output settings, and steps to reproduce.
