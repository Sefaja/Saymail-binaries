# Saymail — release binaries

This repository hosts the official, code-signed release binaries for
**[Saymail](https://saymail.eu)**, the AI-powered desktop email client.

Saymail uses AI to read your incoming mail and automatically sort it by
importance, so the messages that actually matter rise to the top and the noise
stays out of your way. It runs as a native desktop app on **Windows, macOS, and
Linux**.

## What's in here

Each GitHub Release in this repo corresponds to one Saymail version (tagged
`v<version>`, e.g. `v1.0.1173`) and contains the installers and update packages
for every platform:

| Platform | Asset |
| --- | --- |
| Windows | `Saymail_<version>_x64-setup.exe` |
| macOS (Apple Silicon) | `Saymail_<version>_aarch64.dmg`, `…_aarch64.app.tar.gz` |
| macOS (Intel) | `Saymail_<version>_x64.dmg`, `…_x64.app.tar.gz` |
| Linux | `Saymail_<version>_amd64.AppImage`, `…_amd64.deb`, `Saymail-<version>-1.x86_64.rpm` |

Each binary ships with a `.sig` minisign signature. The Saymail desktop app's
built-in auto-updater verifies this signature before installing any update, so a
download is only trusted if it was signed with Saymail's private updater key.

## How it's used

- **Download:** the buttons at **[saymail.eu/download](https://saymail.eu/download)**
  link to the latest release here.
- **Auto-update:** the desktop app reads its update manifest from
  `https://saymail.eu/version.json` and pulls the matching binary from this repo.

This repo exists purely to serve these files with fast, unmetered downloads. The
Saymail application source code is **not** public.

## License

These binaries are **proprietary**. See [`LICENSE`](LICENSE). Use of Saymail is
governed by the [Saymail Terms](https://saymail.eu/en/legal/terms).

— A product of **Sefaja** · https://saymail.eu
