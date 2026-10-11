# Cadenza releases

Installers for Cadenza, a personal music player for Windows. The source code lives in a private repo; this one only holds what the app needs to update itself.

## Install

Download `Cadenza_<version>_x64-setup.exe` from the [latest release](https://github.com/Asarez31/cadenza-releases/releases/latest) and run it.

If Cadenza is already installed, the installer updates it in place. You click Install once, and your library and settings stay as they are.

## Updates

Cadenza checks this repo when it starts and once a day after that. When there's a new version, it shows "Update to x.y.z". Click it and Cadenza downloads the update, closes, installs it and opens again.

## What's in each release

- `Cadenza_<version>_x64-setup.exe`: the installer.
- `Cadenza_<version>_x64-setup.exe.sig`: its signature. Cadenza won't install an update unless the signature matches its built-in public key.
- `latest.json`: version, notes and download link, read by the in-app updater.
