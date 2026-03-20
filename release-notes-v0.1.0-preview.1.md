# SDOH Data Explorer 0.1.0 Preview 1

## Downloads

- `SDOH.Data.Explorer-0.1.0-mac-arm64.dmg`
- `SDOH.Data.Explorer-0.1.0-win-x64-setup.exe`
- `SHA256SUMS.txt`

## Before You Launch

Install **R 4.5.x** first:

- [CRAN](https://cran.r-project.org/)

This desktop build is a lightweight launcher. It does not bundle R or a preinstalled package library.

## Installation

### macOS

1. Download the `.dmg`.
2. Move **SDOH Data Explorer.app** into `Applications`.
3. Open the app.

### Windows

1. Download the `.exe`.
2. Run the installer.
3. Open **SDOH Data Explorer**.

## First Launch Checks

The launcher checks for:

- local `Rscript`
- `R 4.5.x`
- required R packages

If packages are missing, the app will display the exact `renv::restore(...)` command to run manually in R or RStudio.

## Notes

- macOS build: Apple Silicon only
- current macOS build is unsigned / not notarized
