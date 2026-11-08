<p align="center">
  <img src="https://raw.githubusercontent.com/Qubyte-Labs/peekin-releases/main/icon.png" width="96" height="96" alt="Peekin">
</p>

<h1 align="center">Peekin</h1>

<p align="center">
  Sticky notes that live on the edge of your screen.<br>
  Free for Windows, macOS and Linux.
</p>

<p align="center">
  <a href="https://github.com/Qubyte-Labs/peekin-releases/releases/latest"><b>Download the latest version</b></a>
</p>

---

## Install

The quickest way is one line in a terminal. It downloads the latest version,
installs it and starts it, without the "unknown app" warnings.

**macOS and Linux** (Terminal)

```sh
curl -fsSL https://github.com/Qubyte-Labs/peekin-releases/releases/latest/download/install.sh | sh
```

**Windows** (PowerShell)

```powershell
irm https://github.com/Qubyte-Labs/peekin-releases/releases/latest/download/install.ps1 | iex
```

Run the same line again any time to reinstall or update.

### Or download a file

From the [latest release](https://github.com/Qubyte-Labs/peekin-releases/releases/latest), under **Assets**:

| System | File |
|---|---|
| Windows 10 and 11 | `Peekin_<version>_x64-setup.exe` |
| macOS, Apple Silicon (M1 and newer) | `Peekin_<version>_aarch64.dmg` |
| macOS, Intel | `Peekin_<version>_x64.dmg` |
| Linux: Debian, Ubuntu | `Peekin_<version>_amd64.deb` |
| Linux: Fedora, openSUSE | `Peekin-<version>-1.x86_64.rpm` |
| Linux: any distribution | `Peekin_<version>_amd64.AppImage` |

> **Peekin isn't code-signed yet**, so your system may warn you the first time:
>
> - **Windows:** "Windows protected your PC" → **More info** → **Run anyway**.
> - **macOS:** right-click Peekin in Applications → **Open** → **Open**.
> - **Linux AppImage:** make it executable (`chmod +x`), then open it. Some systems need `libfuse2`.
>
> The one-line installs above skip these prompts.

## What it does

- **The deck.** Your notes sit as slim tabs on the edge of the screen. Rest on a
  tab to peek, click to open, drag to reorder.
- **Today.** One note always on top for the day ahead. Each morning it starts
  fresh and carries over what you didn't finish.
- **Quick note.** <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>N</kbd> from any app, type, press Enter.
- **Checklists, reminders, colours and fonts**, with progress right on the tab.
- **Notes for an app.** Tie a note to VS Code, Chrome, Excel… and it shows only while that app is in front.
- **Pin a note** to keep it above every window while you work.
- **All notes** (<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>A</kbd>): search, archive, export to JSON or Markdown.

## Updates

Peekin updates itself. It checks once a day, tells you when a new version is
ready, and installs it when you say so. Every update is signature-checked
before it installs. Your notes are always kept.

What changed in each version is in the [release notes](https://github.com/Qubyte-Labs/peekin-releases/releases).

## Private by design

- No account, no cloud, no tracking.
- Your notes stay on your computer, in one file in `Documents/Peekin`, with the
  last good copy kept as a backup.
- The only thing Peekin fetches from the internet is its own updates, from this page.

## Requirements

| | |
|---|---|
| Windows | 10 or 11, 64-bit |
| macOS | 10.15 Catalina or newer, Apple Silicon or Intel |
| Linux | 64-bit (x86_64) with WebKitGTK 4.1; X11 or Wayland |

## Uninstall

- **Windows:** Settings → Apps → Peekin → Uninstall.
- **macOS:** quit Peekin from the menu bar, then move it from Applications to the Bin.
- **Linux:** `sudo apt remove peekin`, `sudo dnf remove peekin`, or delete the AppImage.

Your notes stay in `Documents/Peekin` until you delete that folder.

---

<p align="center"><sub>© Qubyte Labs. This repository hosts Peekin's releases; the source code is private.</sub></p>
