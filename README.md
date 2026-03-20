# SDOH Data Explorer Releases

This repository is the public download channel for **SDOH Data Explorer** desktop builds.

The application source code remains in a separate private repository. This repository only contains release assets, checksums, and end-user installation guidance.

## Latest Release

Download the latest installers from:

- [Releases](https://github.com/lifu777/SDOH-releases/releases)
- [v0.1.0-preview.1](https://github.com/lifu777/SDOH-releases/releases/tag/v0.1.0-preview.1)

Available assets in `v0.1.0-preview.1`:

- `SDOH.Data.Explorer-0.1.0-mac-arm64.dmg`
- `SDOH.Data.Explorer-0.1.0-win-x64-setup.exe`
- `SHA256SUMS.txt`

## Platform Support

- macOS: Apple Silicon (`arm64`)
- Windows: `x64`

## Prerequisite

Install **R 4.5.x** before launching the desktop app:

- [Download R from CRAN](https://cran.r-project.org/)

The desktop app is a lightweight launcher. It does **not** bundle R or a preinstalled package library.

## Installation

### macOS

1. Install `R 4.5.x`.
2. Download `SDOH.Data.Explorer-0.1.0-mac-arm64.dmg` from the latest release.
3. Open the `.dmg` and move **SDOH Data Explorer.app** into `Applications`.
4. Launch the app.

Notes:

- This build is for Apple Silicon only.
- The app is currently unsigned / not notarized.

### Windows

1. Install `R 4.5.x`.
2. Download `SDOH.Data.Explorer-0.1.0-win-x64-setup.exe` from the latest release.
3. Run the installer.
4. Launch **SDOH Data Explorer** from the Start menu or desktop shortcut.

## First Launch Behavior

On launch, the desktop app checks for:

- `Rscript` on the local machine
- a compatible `R 4.5.x` version
- required R packages for the application

If R is missing, the launcher will stop and show an installation prompt.

If required packages are missing, the launcher will stop and show the exact `renv::restore(...)` command to run in R or RStudio. The launcher does not install packages automatically in this build.

## Checksum Verification

Use `SHA256SUMS.txt` from the same release to verify downloads.

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
