# SDOH Data Explorer Downloads

This repository is the public download channel for **SDOH Data Explorer** desktop builds.

The application source code remains in a separate private repository. This repository only contains current download links, checksums, and end-user installation guidance.

## Download The Current Build

Current public build: **SDOH Data Explorer 0.1.0 Preview 2**

- [Download for macOS (Apple Silicon)](https://github.com/lifu777/SDOH-releases/releases/download/v0.1.0-preview.2/SDOH.Data.Explorer-0.1.0-mac-arm64.dmg)
- [Download for Windows (x64)](https://github.com/lifu777/SDOH-releases/releases/download/v0.1.0-preview.2/SDOH.Data.Explorer-0.1.0-win-x64-setup.exe)
- [Download SHA256 checksums](https://github.com/lifu777/SDOH-releases/releases/download/v0.1.0-preview.2/SHA256SUMS.txt)
- [Installation and first-launch notes](./LATEST-RELEASE.md)

Older GitHub releases may still exist for rollback and verification, but this page only links to the current public build.

## Platform Support

- macOS: Apple Silicon (`arm64`)
- Windows: `x64`

## Prerequisite

Install **R 4.5.x** before launching the desktop app:

- [Download R from CRAN](https://cran.r-project.org/)

The desktop app is a lightweight launcher. It does **not** bundle R or a preinstalled package library.

## Checksum Verification

Use `SHA256SUMS.txt` from this repository root or from the current build links above to verify downloads.

Examples:

```bash
shasum -a 256 "SDOH.Data.Explorer-0.1.0-mac-arm64.dmg"
certutil -hashfile "SDOH.Data.Explorer-0.1.0-win-x64-setup.exe" SHA256
```

## Support Scope

This repository is limited to release distribution and installation notes.

Issues related to:

- downloading release assets
- checksum mismatches
- basic desktop installation problems

can be tracked here. Application source development remains in the private project repository.
