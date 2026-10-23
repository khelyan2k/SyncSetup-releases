<div align="center">

<img src="assets/logo.png" width="112" alt="SyncSetup logo" />

# SyncSetup

### All your Windows software, in one place.

Install, update, repair and uninstall your apps — back up your browsers, apps and games — and get your whole setup back on a new PC in a few clicks.

[![Latest release](https://img.shields.io/github/v/release/khelyan2k/SyncSetup-releases?style=for-the-badge&label=Download&color=5b8cff)](https://github.com/khelyan2k/SyncSetup-releases/releases/latest) [![Downloads](https://img.shields.io/github/downloads/khelyan2k/SyncSetup-releases/total?style=for-the-badge&color=38bdb0)](https://github.com/khelyan2k/SyncSetup-releases/releases) ![Windows 10 / 11](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?style=for-the-badge&logo=windows&logoColor=white) ![Free](https://img.shields.io/badge/Price-Free-2ea44f?style=for-the-badge)

**[⬇️ Download](https://github.com/khelyan2k/SyncSetup-releases/releases/latest)** · **[What's new](https://github.com/khelyan2k/SyncSetup-releases/releases)** · **[Report a bug](https://github.com/khelyan2k/SyncSetup-releases/issues)** · **[🇫🇷 Version française](README.fr.md)**

<br />

<img src="assets/screenshots/en/01-dashboard.png" width="900" alt="SyncSetup dashboard" />

</div>

<br />

## Why SyncSetup?

Setting up a PC means visiting dozens of websites, clicking through installers, then keeping everything up to date by hand. **SyncSetup does it for you** — and does it carefully:

- 🧩 **One app for everything** — 314 hand-picked apps, plus every package from winget, Scoop, Chocolatey, pip, npm and 6 other managers.
- 🔒 **Only official sources** — apps come from their publisher through winget (Microsoft's package manager) or the Microsoft Store. Never a repackaged installer.
- ✅ **Nothing is assumed** — every install, update or uninstall is checked afterwards. If it didn't work, SyncSetup tells you why, in plain words.
- 💾 **Your setup, anywhere** — profiles, backups and a full export let you move to a new PC without starting from scratch.

<br />

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 📦 Catalogue

**314 apps** sorted by category — browsers, games, communication, development, video, security, drivers, streaming, VPNs…

- Install in one click from the **official source**, or the **Microsoft Store** version when you prefer
- Choose a **specific version**, or a channel (stable, beta, nightly, LTS…)
- **Mods** in one click: Spicetify for Spotify, Vencord, Equicord, BetterDiscord
- Web services without a Windows app (YouTube…) as clearly labelled web shortcuts

</td>
<td width="50%" valign="top">

<img src="assets/screenshots/en/02-catalog.png" alt="Catalogue" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/screenshots/en/04-updates.png" alt="Updates" />

</td>
<td width="50%" valign="top">

### 🔄 Updates

All your apps **and** packages in a single list.

- Update everything in one click — **several at once** when it's safe (never two Windows Installer setups together)
- Live download speed, clear statuses: ✅ done · ℹ️ already up to date · ⚠️ needs attention · ❌ failed, with the reason
- Reminders when updates are waiting (at startup, every 2, 4 or 8 h)
- **Scheduled maintenance**: check and update automatically, on your schedule
- Ignore a version, or an app for good

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🖥️ Installed apps

- Everything installed on the PC — even **portable apps** dropped on the Desktop and games installed by **Steam, Epic, Riot**…
- **Other programs** tab: uninstall anything Windows knows about, with its official uninstaller
- Changes made outside SyncSetup are picked up automatically
- Something blocks an update? SyncSetup finds which program is holding the files and offers **Close and retry**

</td>
<td width="50%" valign="top">

<img src="assets/screenshots/en/03-app-details.png" alt="App details" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/screenshots/en/08-backups.png" alt="Backups" />

</td>
<td width="50%" valign="top">

### 💾 Backups & transfer

**76 browsers, apps and games**: bookmarks, settings, extensions, Discord and its mods, Spotify, VS Code, Minecraft worlds, Steam collections, VALORANT settings…

- Restore on this PC or another one, **integrity-checked** (SHA-256)
- **Never** any password, cookie or sign-in session
- **Export / import** all of SyncSetup in a single file
- **Profiles**: your app list, reinstalled in one click on a new PC
- Optional backup to a **secret GitHub Gist**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⚡ Optimization

- **Optimize now**: closes what runs for nothing, frees memory, cleans temporary files — with a health score based on real measurements
- Knows hundreds of programs: what can be closed, what must stay open (drivers, antivirus, anti-cheat, sync…)
- **Startup manager**, including system-wide entries, with a warning before you disable something important
- Hardware and drivers at a glance

</td>
<td width="50%" valign="top">

<img src="assets/screenshots/en/07-optimization.png" alt="Optimization" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/screenshots/en/09-themes.png" alt="Themes" />

</td>
<td width="50%" valign="top">

### 🎨 Made to feel at home

- **16 themes** (dark, light, OLED, high contrast…), accent colours, density, animations — or create your own
- **Performance profile**: lighter on modest PCs, richer on recent ones
- **English or French**
- Keyboard shortcuts, search everywhere, notification centre, system tray
- **Updates itself** (verified download, one-click rollback to any previous version)

</td>
</tr>
</table>

<br />

## 🔒 Safe by design

| | |
|---|---|
| **Official sources only** | Apps are installed through winget or the Microsoft Store, from the publisher's own files. When SyncSetup has to download a publisher's installer itself, its **digital signature** is checked before it runs. |
| **Checked, not assumed** | An operation is reported as successful only after SyncSetup has verified the result on your PC. |
| **Your data stays yours** | Settings and backups stay on your PC (`%APPDATA%\syncsetup`). **No account required, no ads, no telemetry.** Online backup (GitHub Gist, SyncSetup account) only if you turn it on. |
| **No secrets copied** | Backups never contain passwords, cookies, payment data or sign-in tokens. |
| **Windows security respected** | Administrator mode is optional and never bypasses Windows' UAC prompt. Important startup items and drivers are protected by a confirmation. |
| **Verified self-updates** | Each SyncSetup update is checked (SHA-512) before it's installed, and you can roll back at any time. |

<br />

## 📥 Installation

1. Download **`SyncSetup-Setup-x.y.z.exe`** from the **[latest release](https://github.com/khelyan2k/SyncSetup-releases/releases/latest)**.
2. Run it and follow the installer — it installs for your Windows account, no administrator rights needed.
3. That's it. SyncSetup keeps itself up to date from now on.

> [!NOTE]
> The installer is not code-signed yet (a certificate costs several hundred euros a year), so Windows may show **“Windows protected your PC”**. Click **More info → Run anyway**. You can check any release on [VirusTotal](https://www.virustotal.com) before running it.

**Requirements:** Windows 10 or 11, 64-bit · winget (included in Windows 11 and up-to-date Windows 10).

<br />

## ❓ FAQ

<details>
<summary><b>Is SyncSetup free?</b></summary>
<br />
Yes, completely — no ads, no premium version, no account needed.
</details>

<details>
<summary><b>How is it different from winget, UniGetUI or Ninite?</b></summary>
<br />
SyncSetup uses winget under the hood, like UniGetUI, and covers the whole Ninite list. On top of that it checks every result, explains errors in plain words, backs up and restores your apps' settings, moves your setup to a new PC, and helps you keep the PC clean and fast.
</details>

<details>
<summary><b>Do I need to run it as administrator?</b></summary>
<br />
No. It works with normal rights; Windows asks for permission when an installer needs it. An optional administrator mode (one Windows confirmation, once) avoids repeated prompts. Apps that refuse administrator rights are automatically run with your normal rights.
</details>

<details>
<summary><b>Where are my data and backups stored?</b></summary>
<br />
In <code>%APPDATA%\syncsetup</code> on your PC (backups in <code>%APPDATA%\syncsetup\Sauvegardes</code>, or any folder you choose — a OneDrive folder works great to find them on another PC).
</details>

<details>
<summary><b>What does SyncSetup connect to?</b></summary>
<br />
winget and the package registries you use (to install and update), GitHub (SyncSetup's own updates), icon services (app icons) — and, only if you turn them on, your GitHub Gist or SyncSetup account for online backup. Nothing else.
</details>

<details>
<summary><b>How do I uninstall it?</b></summary>
<br />
Windows Settings › Apps › SyncSetup › Uninstall. Your settings stay in <code>%APPDATA%\syncsetup</code> until you delete that folder.
</details>

<br />

## 💬 Support

Found a bug or have an idea? **[Open an issue](https://github.com/khelyan2k/SyncSetup-releases/issues)** — or reach me on Discord: **`.khelyan`**.

If SyncSetup saves you time, a ⭐ on this page helps a lot!

<br />

<div align="center">

Made with ❤️ by **[khelyan](https://github.com/khelyan2k)**

</div>
