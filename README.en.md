# Codex Account Switcher

[Русский](README.md) | [English](README.en.md)

<img align="right" src="assets/logo.png" alt="Codex Account Switcher" width="220" height="220">

A local Windows utility for saving and quickly switching accounts in the Codex Desktop application.

Easily manage multiple accounts under recognizable names, switch between them in one click, launch Codex, and create desktop shortcuts for each profile or for a new sign-in session.

Supports **both the official [Microsoft Store](https://apps.microsoft.com/detail/9nxq8fg885bb) / installer version and portable builds** of Codex.

**Version:** 1.0.0  
**Author:** [CodoMagia](https://github.com/codomagia)  
**Support:** [Boosty](https://boosty.to/codomagia/donate)

Builds are available in [Releases](https://github.com/codomagia/CodexAccountSwitcher/releases).

## Preview

![Codex Account Switcher](assets/screenshot.png)

## Download

1. Open the [latest Release](https://github.com/codomagia/CodexAccountSwitcher/releases/latest).
2. Download `Codex-Account-Switcher-1.0.0.zip`.
3. Extract the archive to a permanent folder.
4. Run `Codex Account Switcher.exe`.
5. If needed, select your `ChatGPT.exe` or `codex.exe` in Settings (or the app will discover it automatically on launch).

No installation is required. Do not run the application directly from the ZIP archive.

## System requirements

- Windows 10 or Windows 11
- .NET Framework 4.7.2 or newer
- Codex Desktop application:
  - Official version from the [Microsoft Store](https://apps.microsoft.com/detail/9nxq8fg885bb) or installer
  - **OR** any standalone portable build containing `ChatGPT.exe` / `codex.exe`

## Features

- **Supports all versions:** works seamlessly with installed versions (including Microsoft Store) and portable builds.
- **Multiple accounts:** save any number of profiles with custom names.
- **Safe switching:** validates `auth.json` before and after copying, automatically rolls back on error.
- **Auto-sync:** updates the outgoing profile automatically before switching to another account.
- **Fast launch & shortcuts:** create desktop shortcuts for instant login into a specific profile or into a fresh session.
- **Automatic process guard:** detects running Codex processes in Windows and blocks operations to prevent session corruption.
- **100% offline & private:** works entirely on your PC, includes no telemetry, and sends no data to remote servers.

## How to use

1. Close Codex if it is currently running.
2. Save your current account as a profile (click "Save Profile").
3. To switch, select the desired profile from the list and click "Launch".
4. To start a clean new session, click "New Session".

Profiles are stored locally in `%USERPROFILE%\.codex\_saved_accounts`.

> **Security note:** Profiles contain local authorization tokens (`auth.json`). Never upload or share your profile folder with anyone.

*This is an independent, unofficial utility and is not affiliated with or endorsed by OpenAI.*

## License

Copyright © 2026 CodoMagia. All rights reserved.

Allowed:
- freely download and use the program;
- redistribute the unmodified official distribution.

Not allowed:
- modifying the program and distributing modified copies;
- presenting the program as someone else's or removing author attribution.
