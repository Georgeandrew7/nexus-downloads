# Nexus Chat App

**A privacy-first communication platform for Windows, macOS, and Linux.**

Nexus is a fast, modern chat app for teams and communities — servers, channels, and
direct messages, with privacy and account security (including two-factor authentication)
built in.

> ⚠️ Nexus is in early development. The first public installers are being prepared —
> watch the [**Releases**](../../releases) page for the initial download.

---

## Download

Grab the latest build from the [**Releases**](../../releases/latest) page:

| Platform | Download |
| --- | --- |
| **Windows** | `Nexus_x.y.z_x64-setup.exe` (installer) or `.msi` |
| **macOS** | `Nexus_x.y.z_universal.dmg` |
| **Linux** | `.AppImage` (portable), `.deb` (Debian/Ubuntu), or `.rpm` (Fedora/RHEL) |

---

## Install

### Windows
1. Download the `.exe` (or `.msi`) from the latest release.
2. Run it and follow the installer prompts.
3. If Windows SmartScreen warns about an unrecognized publisher, click **More info → Run anyway**
   (early builds are not yet code-signed).

### macOS
1. Download the `.dmg` and open it.
2. Drag **Nexus** into your **Applications** folder.
3. On first launch, right-click the app → **Open** → **Open** (needed once for unsigned builds).

### Linux
- **AppImage:** `chmod +x Nexus_*.AppImage` then run it.
- **Debian/Ubuntu:** `sudo apt install ./Nexus_*.deb`
- **Fedora/RHEL:** `sudo dnf install ./Nexus_*.rpm`

---

## System requirements

- **Windows:** Windows 10 or later (64-bit), with WebView2 (preinstalled on current Windows).
- **macOS:** macOS 11 (Big Sur) or later.
- **Linux:** A modern 64-bit distribution with WebKitGTK 4.1 available.

---

## Having trouble?

See **[Troubleshooting](docs/TROUBLESHOOTING.md)** for fixes to common issues, or
[open an issue](../../issues/new) describing what went wrong (include your OS, app version,
and any error message).

---

© 2026 George / VELOCIPHITECH. Nexus and the Nexus logo are trademarks of VELOCIPHITECH.
This repository distributes the prebuilt Nexus desktop application; redistribution terms
are described in the release notes.
