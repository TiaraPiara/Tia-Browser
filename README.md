# Tia Browser

**Explore beyond.**

Tia is a customizable desktop browser for **Windows 64-bit**, built with Electron and Chromium. It brings everyday browsing together with a flexible interface, a personal New Tab workspace, privacy controls, and practical tools for downloads and browser management.

[**Download Tia**](https://github.com/TiaraPiara/Tia-Browser/releases/latest) · [Release history](https://github.com/TiaraPiara/Tia-Browser/releases) · [Report a problem](https://github.com/TiaraPiara/Tia-Browser/issues)

---

## Explore Tia

### Make the browser feel like yours

- A customizable New Tab workspace with Quick Access, bookmarks, recent searches, and wallpapers.
- Dark, Light, and System appearance modes, custom accent colors, and a full interface palette randomizer.
- Tabbed browsing with drag-and-drop tab reordering and session restoration.
- A bookmarks bar you can show or hide, plus customizable keyboard shortcuts.

### Browse your way

- Address-bar search and suggestions with Google, Bing, or DuckDuckGo.
- Browsing history, bookmarks, Find in page, and page zoom.
- Hard Reload shortcuts for pages that keep showing cached content: **Ctrl+Shift+R**, **Ctrl+F5**, or **Shift+F5**.
- Open supported local files—including HTML, PDF, images, text, and media—in Tia.

### Privacy and control

- Private windows use a separate temporary session. Private browsing history and download records are not added to your normal Tia profile.
- Manage site permissions for camera, microphone, location, notifications, and other browser capabilities.
- Clear browsing data and review saved site permissions.
- An optional Ghostery-powered ad and tracker blocker.
- Optional SponsorBlock integration for community-marked segments on YouTube.
- A local password vault with passwords protected on disk and user-controlled autofill. Tia does not automatically submit login forms.
- Flexible proxy modes: system settings, automatic detection, direct connection, or manual configuration.

### Downloads and everyday tools

- A built-in download manager with pause, resume, retry, open, and file-management actions.
- Optional Internet Download Manager (IDM) handoff for supported direct links. IDM is a separate application and must be installed independently.
- Import bookmarks from Chrome or Firefox, and import saved passwords from supported CSV exports.

## Download and install

1. Open the [latest Tia release](https://github.com/TiaraPiara/Tia-Browser/releases/latest).
2. Download **Tia Setup** for Windows 64-bit.
3. Run the installer and follow the setup steps.
4. Launch Tia from the Start menu or your chosen shortcut.

The public release channel provides a Windows 64-bit installer. Check the release page for the current version, release notes, and verification files.

## Security, authenticity, and transparency

Tia is currently **closed-source software**. Its development source code is maintained privately and is not published in this repository. This means visitors cannot independently inspect or reproduce the browser from this repository. We want to be clear about that rather than imply that Tia is open source or independently audited.

For safer downloads:

- Download Tia only from the [official GitHub Releases page](https://github.com/TiaraPiara/Tia-Browser/releases). Avoid third-party mirrors and repackaged installers.
- Each official release includes a SHA256SUMS.txt file for the installer, blockmap, and update metadata. Use it to compare the SHA-256 hash of a downloaded asset with the published value. A matching hash confirms that the file matches the published release checksum; it does **not** prove that software is harmless or independently audited.
- On Windows, calculate the installer hash with PowerShell: `Get-FileHash ".\Tia Setup 1.0.0.exe" -Algorithm SHA256`. Compare its `Hash` value with the installer entry in `SHA256SUMS.txt`.
- On Windows, calculate the installer hash with PowerShell: `Get-FileHash "./Tia Setup 1.0.0.exe" -Algorithm SHA256`. Compare its `Hash` value with the installer entry in `SHA256SUMS.txt`.
- Review the release notes and version before installing. Report unexpected behavior through [GitHub Issues](https://github.com/TiaraPiara/Tia-Browser/issues).
- Keep Microsoft Defender and Windows security features enabled. Do not ignore a security warning solely because a file is hosted on GitHub.

### Windows SmartScreen and code signing

Tia is a new independently distributed Windows application, so Windows may show a Microsoft Defender SmartScreen reputation warning when the installer is not yet widely known. The project's current packaging configuration does not itself establish a public Authenticode signing identity. Check the release notes and the installer's **Properties → Digital Signatures** tab for the signing status of the specific release. If no valid signature is shown, Windows cannot display a verified publisher identity for that installer.

A SmartScreen warning is not, by itself, proof that a file is malicious—but it is also not proof that a file is safe. Verify that the download came from the official release, compare its checksum, and scan it with security software before deciding whether to run it. We do not ask users to disable Windows security protections.

Code signing is a trust improvement to consider for future releases. A valid Authenticode signature can identify the publisher and help detect changes made after signing. SmartScreen reputation may still take time to build for a new application, including signed releases. See [Microsoft's SmartScreen guidance](https://learn.microsoft.com/windows/apps/package-and-deploy/smartscreen-reputation) and [Windows code-signing options](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/code-signing-options).

## Updates

Tia checks for updates automatically. In **Settings → Tia updates**, you can check manually and choose whether updates download automatically. When an update is ready, you can restart Tia to install it immediately, or keep using the current version and let it install silently after the next full browser exit.

Tia's Windows NSIS updates support differential downloads when the installed version and update package are compatible. This can reduce the amount of data transferred: the release still contains a full installer, but existing users may only need to download changed portions. A first-time installation requires the full installer.

## Your data

Bookmarks, history, settings, downloads information, and saved passwords are stored in your local Tia profile on your device. Private windows use a separate temporary session. Tia does not currently provide account-based cloud synchronization, so profile data does not automatically sync between computers.

Uninstalling Tia does not automatically remove its profile data. Keep your own backups of anything important before uninstalling, resetting Windows, or moving to another PC.

## Help and troubleshooting

- **A page looks outdated:** try a normal reload first, then use **Ctrl+Shift+R** or **Ctrl+F5** for a hard reload that bypasses the normal HTTP cache.
- **A download is stuck:** check the Downloads page and your configured download folder. If you use IDM, verify that Tia points to the correct IDMan.exe.
- **An update is not appearing:** open **Settings → Tia updates** and select **Check for updates**. Automatic updates are available in installed Windows releases, not development or portable builds.
- **A problem persists:** [open an issue](https://github.com/TiaraPiara/Tia-Browser/issues) and include your Tia version, Windows version, and steps to reproduce the problem. Review any logs before sharing them; do not attach passwords, cookies, private browsing data, or update tokens.

## About this repository

This public repository distributes official Tia releases, SHA-256 verification files, and update packages. Tia's development source code is maintained privately and is not included here. Release assets are compiled application installers and the metadata required by Tia's updater.

Tia is built with Electron and Chromium. Ghostery, SponsorBlock, and Internet Download Manager are separate components or products; IDM must be installed independently.

---

**Tia Browser 1.0.0** · First stable release · Windows 64-bit
