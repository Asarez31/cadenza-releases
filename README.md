# Cadenza releases

Installers for Cadenza, a personal music player for Windows and Android. The source code lives in a private repo; this one only holds the builds and the files the apps read to update themselves.

## Install

Get both from the [latest release](https://github.com/Asarez31/cadenza-releases/releases/latest).

On Windows, download `Cadenza_<version>_x64-setup.exe` and run it. Cadenza installs to Program Files, so Windows asks for admin rights. If it's already installed, the installer updates it in place and your library and settings stay as they are.

On Android, download `Cadenza-<version>-arm64.apk` on the phone and open it. Android asks once to allow installs from your browser or file manager.

## Updates

Both apps check this repo when they start and once a day after that. When there's a new version, they offer "Update to x.y.z". On Windows, Cadenza downloads the update, closes, installs it and opens again. On Android, it downloads the APK and hands it to Android's installer.

## What's in each release

- `Cadenza_<version>_x64-setup.exe`: the Windows installer.
- `Cadenza_<version>_x64-setup.exe.sig`: its signature. Cadenza won't install an update unless the signature matches its built-in public key.
- `latest.json`: version, notes and download link, read by the Windows updater.
- `Cadenza-<version>-arm64.apk`: the Android app, signed with Cadenza's release key. Android only installs it over an earlier version signed with the same key.
- `latest-android.json`: version, notes, download link and the APK's SHA-256, read by the Android updater, which checks the hash before installing.
