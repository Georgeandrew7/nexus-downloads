# Troubleshooting

Solutions to the most common issues with the Nexus desktop app. If none of these help,
[open an issue](../../issues/new) and include your **operating system**, the **app version**
(Settings → About), and any **error message** you see.

---

## The app won't open / closes immediately

- **Windows:** Make sure **WebView2** is installed. It ships with current Windows, but on
  older machines you can install the *Evergreen WebView2 Runtime* from Microsoft.
- **macOS:** If you see *"Nexus is damaged"* or *"can't be opened because it is from an
  unidentified developer,"* right-click the app → **Open** → **Open**. Early builds aren't
  notarized yet.
- **Linux:** Most "won't launch" cases are a missing **WebKitGTK 4.1** library. Install your
  distro's `webkit2gtk-4.1` package (names vary), then relaunch.

## "Unrecognized publisher" / SmartScreen warning (Windows)

Early builds are not yet code-signed. Click **More info → Run anyway**. This warning will go
away once signed builds are published.

## Can't connect / "server unavailable"

1. Check your internet connection.
2. Confirm you're pointing at the correct server address in **Settings → Connection**.
3. If you self-host the Nexus server, verify it's running and reachable from this machine.
4. Corporate firewalls or VPNs sometimes block the connection — try another network to isolate it.

## Can't log in

- Double-check your email and password (passwords are case-sensitive).
- If you enabled **two-factor authentication**, enter the current 6-digit code from your
  authenticator app — codes rotate every 30 seconds, so make sure your device clock is accurate.
- Forgot your password? Use **Forgot password** on the login screen to receive a reset link.

## Two-factor (2FA) codes are rejected

TOTP codes depend on an accurate clock. Make sure your computer's **date & time are set to
automatic/network time**. A clock that's off by more than ~30 seconds will reject valid codes.

## The app looks broken or won't update

1. Fully quit and reopen the app.
2. Install the latest version from the [Releases](../../releases/latest) page.
3. If problems persist, uninstall, then reinstall the latest build.

## Where are the logs?

When reporting a bug, logs help a lot. They live at:

- **Windows:** `%APPDATA%\Nexus\logs\`
- **macOS:** `~/Library/Logs/Nexus/`
- **Linux:** `~/.local/share/Nexus/logs/` (or `~/.config/Nexus/logs/`)

---

## Reporting a bug

[Open an issue](../../issues/new) with:

- Your OS and version (e.g. *Windows 11*, *macOS 14*, *Ubuntu 24.04*)
- The Nexus app version (Settings → About)
- What you did, what you expected, and what happened
- Any error message or relevant log lines
