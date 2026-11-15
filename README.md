# ⚡ SWEAT Executor for macOS

**SWEAT Executor** is a lightweight, native macOS script execution environment built with Electron and custom memory-injection tooling, designed to run seamlessly on Apple Silicon (M1/M2/M3/M4) and Intel Macs.

---

## 🚀 Features

- **Native macOS Packaging:** Distributed as a clean `.dmg` installer with zero bloatware.
- **Apple Silicon Optimized:** Built natively for `arm64` architecture for minimal CPU overhead and low heat output.
- **Modern UI:** Fast, responsive interface for managing, editing, and executing scripts effortlessly.
- **Custom Runtime Configuration:** Tailored entitlements (`allow-jit`) to ensure smooth script execution without unnecessary crashes.

---

## 📋 System Requirements

- **OS:** macOS 12.0 (Monterey) or newer
- **Architecture:** Apple Silicon (`arm64`) — *Intel (`x64`) support coming soon*
- **Storage:** ~250 MB of free disk space
- **Roblox Client:** Latest official macOS version installed

---

## 📥 Installation & Gatekeeper Fix (READ THIS)

Because **SWEAT Executor** is an independent project and is not signed with a paid $99/year Apple Developer Certificate, macOS Gatekeeper will block the app on first launch or show a warning saying *"SWEAT Executor is damaged and can't be opened"*. **This is completely normal.**

Follow these steps to install and bypass Gatekeeper safely:

### Step 1: Install the App
1. Go to the [**Releases**](https://github.com/plsandroid-collab/sweat-executor/releases/latest) page and download `SWEAT.Executor-1.0.0-arm64.dmg`.
2. Double-click the `.dmg` file and drag **SWEAT Executor** into your **Applications** folder.

### Step 2: Bypass the macOS Security Warning
Choose **one** of the two methods below:

#### Method A: Via Terminal (Fastest & Recommended)
Open the **Terminal** app on your Mac and paste the following command, then press **Enter**:
```bash
xattr -dr com.apple.quarantine /Applications/SWEAT\ Executor.app                                                                                                                         After running this, you can open the app normally from Launchpad or your Applications folder.
Method B: Via System Settings
Try opening SWEAT Executor once and click Cancel when the warning pops up.
Open System Settings → Privacy & Security.
Scroll down to the Security section and click Open Anyway next to the SWEAT Executor message.
Enter your Mac password and confirm.
❓ Frequently Asked Questions (FAQ)
Q: Why does my antivirus or macOS say the file is damaged or unsafe?
A: Executors interact directly with game memory and are unsigned binaries. Both macOS Gatekeeper and standard antivirus heuristics flag unsigned injection tools by default. Always verify you downloaded the .dmg exclusively from the official GitHub Releases page of this repository.
Q: Does it work on M1, M2, M3, and M4 Macs?
A: Yes. The current release is compiled specifically for arm64 (Apple Silicon), so it runs natively without Rosetta 2 translation overhead.
Q: Roblox updated and the executor stopped attaching. What do I do?
A: Roblox pushes frequent updates that change memory offsets. Check the Releases tab or our Discord server for updated builds whenever a new Roblox patch drops.
⚠️ Disclaimer
This software is provided for educational and research purposes only. Use it responsibly and at your own risk. The developers are not responsible for any account actions taken by third-party platforms.
