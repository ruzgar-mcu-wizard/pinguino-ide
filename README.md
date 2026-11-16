# Pinguino IDE 13 — Windows Port

An unofficial Windows port of the discontinued **Pinguino IDE**, bringing the legacy PIC microcontroller development environment to modern Windows systems.

This project is intended for hobbyists, educators, and anyone who still works with older Pinguino-compatible hardware or wants to revisit the original development environment.

> **This is an unofficial port.** It is not maintained, endorsed, or supported by the original Pinguino IDE authors.

## Download

Get the Windows release from the [Releases page](https://github.com/ruzgar-mcu-wizard/pinguino-ide/releases).

The current release is **v13.0.0 — Pinguino IDE Windows Port Release**. It is published as a pre-release and is available in these archive formats:

- [7-Zip archive (.7z)](https://github.com/ruzgar-mcu-wizard/pinguino-ide/releases/download/pinguino-ide-windows/Pinguino-IDE.7z)
- [RAR archive (.rar)](https://github.com/ruzgar-mcu-wizard/pinguino-ide/releases/download/pinguino-ide-windows/Pinguino-IDE.rar)
- [ZIP archive (.zip)](https://github.com/ruzgar-mcu-wizard/pinguino-ide/releases/download/pinguino-ide-windows/Pinguino-IDE.zip)

Choose the archive format you can extract. You only need to download one.

## Getting started

1. Open the [latest release](https://github.com/ruzgar-mcu-wizard/pinguino-ide/releases).
2. Download one of the available archives.
3. Extract the archive to a folder on your computer.
4. Open the extracted folder and launch the included Pinguino IDE executable.

No source-code checkout is required to use the packaged Windows release.

## What is included

- A Windows executable build of Pinguino IDE.
- Basic compatibility with existing Pinguino toolchains, where applicable.
- The original Pinguino workflow preserved as closely as possible.

The project revives a legacy embedded-development environment; it does not guarantee that every original feature, board, programmer, or toolchain will work on every Windows installation.

## Compatibility and limitations

- The port is intended for modern Windows systems, but behavior may vary between Windows versions and configurations.
- Toolchain compatibility is not universal. Your existing compiler, programmer, and target hardware setup may affect what works.
- Some legacy features may behave differently or have quirks.
- This is a revival of discontinued software, not a complete modernization or a replacement for current development environments.

**Release status:** Pre-release. The build is usable for compiling projects, but compatibility and behavior may vary.

## About Pinguino

Pinguino is an integrated development environment created for programming supported PIC-based microcontroller boards. This repository is based on the discontinued Pinguino IDE project and packages a Windows-oriented build for people who still use the ecosystem.

For the original project, see [PinguinoIDE/pinguino-ide](https://github.com/PinguinoIDE/pinguino-ide).

## Issues and feedback

Found a bug, compatibility problem, or something that does not work as expected?

Please [open an issue in this repository](https://github.com/ruzgar-mcu-wizard/pinguino-ide/issues) and include:

- Your Windows version.
- What you were trying to do.
- What happened and what you expected to happen.
- Any relevant error message or screenshot.

Please keep in mind that this is an unofficial port of discontinued software, so not every upstream issue can necessarily be fixed here.

## License

See the repository's [LICENSE](LICENSE) file for the license information that applies to this codebase. Components and dependencies originating from upstream projects may have their own licensing terms; check their respective license files before redistributing them.
