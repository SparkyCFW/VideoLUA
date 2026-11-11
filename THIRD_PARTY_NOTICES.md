# Third-party notices — VideoLUA /Studio

VideoLUA /Studio copyright (c) 2026 SparkyCFW. The original application is proprietary freeware. Third-party components retain their own licenses and rights.

## FFmpeg

- **Component:** FFmpeg 9.0.2 Essentials build by gyan.dev (`9.0.2-essentials_build-www.gyan.dev`)
- **Copyright:** Copyright (c) 2000–2026 the FFmpeg developers
- **License:** GNU General Public License version 3 (GPLv3), as indicated by `--enable-gpl --enable-version3`
- **Distribution:** Embedded as a resource in VideoLUA and extracted and executed as a separate process at runtime
- **GPLv3 license text:** [COPYING.GPLv3.txt](COPYING.GPLv3.txt)
- **Build provider:** https://www.gyan.dev/ffmpeg/builds/
- **Build release:** https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2
- **Upstream source revision identified for this release:** https://github.com/FFmpeg/FFmpeg/commit/946fcce07b
- **Upstream source archive:** https://github.com/FFmpeg/FFmpeg/archive/946fcce07b.zip
- **Official licensing information:** https://ffmpeg.org/legal.html

Selected third-party codec/source projects enabled in the build include:

- x264: https://code.videolan.org/videolan/x264
- x265: https://bitbucket.org/multicoreware/x265_git
- libvpx: https://chromium.googlesource.com/webm/libvpx/
- libaom: https://aomedia.googlesource.com/aom/

**Corresponding-source compliance is not yet verified.** The upstream links above do not establish complete corresponding source for the precise static FFmpeg binary, including exact third-party library versions, patches, and build materials. See [RELEASE_COMPLIANCE_CHECKLIST.md](RELEASE_COMPLIANCE_CHECKLIST.md). Do not present these links alone as fulfillment of GPLv3 section 6.

## Microsoft .NET 10 and WPF

VideoLUA is published as a self-contained Windows x64 WPF application. Its published EXE contains Microsoft .NET runtime and Windows Desktop/WPF components.

- .NET repository and license information: https://github.com/dotnet/runtime
- WPF repository and license information: https://github.com/dotnet/wpf
- .NET distribution licensing information: https://dotnet.microsoft.com/en-us/platform/free
- .NET third-party notices (inspect the applicable release): https://github.com/dotnet/runtime/blob/main/THIRD-PARTY-NOTICES.TXT

The links above are reference locations, not a verification that all notices for the precise runtime version have been included. The exact .NET 10 runtime build and its required redistribution notices must be checked before public release.

## Other dependencies

The inspected `VideoLUA.csproj` contains no `PackageReference` entries. That does not by itself prove that the distributed runtime and FFmpeg have no additional third-party components. No complete binary-level license audit has been performed.
