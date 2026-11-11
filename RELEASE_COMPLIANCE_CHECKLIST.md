# Release compliance checklist (not a public clearance certificate)

This document records open items. **Do not publish the executable as legally cleared on the strength of this document.**

- [x] Confirm application project targets .NET 10 Windows/WPF and uses self-contained single-file publish.
- [x] Confirm project embeds `ffmpeg.exe` as `VideoLUA.Tools.ffmpeg.exe`.
- [x] Confirm no direct NuGet `PackageReference` entries in the inspected `.csproj`.
- [x] Identify bundled FFmpeg as gyan.dev 9.0.2 Essentials, GPLv3 (`--enable-gpl --enable-version3 --enable-static`).
- [ ] Obtain and offer **complete corresponding source** for the exact FFmpeg binary, including GPL-covered statically linked libraries, patches, and build scripts, through a GPLv3 section 6 compliant method.
- [ ] Confirm exact .NET runtime version, applicable license texts, and Microsoft third-party notices for the published binary.
- [ ] Check other assets, dependencies, and source ownership/permissions.
- [ ] Obtain qualified legal review of whether embedding/extracting and invoking GPLv3 FFmpeg as a separate process keeps proprietary VideoLUA code outside GPL coverage.
- [ ] Verify final release EXE matches the audited source project and FFmpeg binary.

Useful references:
- https://www.gnu.org/licenses/gpl-3.0.html#section6
- https://ffmpeg.org/legal.html
- https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2
- https://github.com/FFmpeg/FFmpeg/commit/946fcce07b

**Do not upload the private project RAR, `.csproj`, C# files, or source folders to the public repository.**
