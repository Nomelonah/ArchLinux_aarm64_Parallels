# ArchLinux_aarm64_Parallels

<p align="left">
  <a href="./README_zh.md"><b>📄 简体中文 README (Switch to Chinese Version)</b></a>
</p>

---

## 📌 Description
A perfectly configured, pure Arch Linux ARM64 virtual machine environment tailored for **Parallels Desktop on Apple Silicon Mac** (M1/M2/M3 chips). 

This box eliminates the painful manual installation process of Arch on ARM64 architectures by providing a fully fixed GNOME desktop environment, native Chinese localized fonts, completely repaired home directory permissions, and pre-configured lightweight alternative tools (`firefox`, custom `pacman` and `yay` AUR package manager configurations). Ready to deploy and roll!

## 🔐 Credentials & Environment Accounts
To prevent permission locking or broken environments from previous configurations, the system uses a clean, unified standard account. Use the following credentials to log in or execute administrative commands:

| Account Type | Username | Password | Privileges / Group |
| :--- | :--- | :--- | :--- |
| **Daily User** | `watermelon` | *1234* | `wheel`, `storage`, `power` (Full `sudo` Access) |
| **Superuser** | `root` | *1234* | Ultimate System Administrator (`#`) |

> ⚠️ **Note**: These passwords are initial, you can change it whenever you want!

## 🚀 How to Use / Deployment Guide

Since Parallels Desktop encapsulates the entire virtual machine as a single, independent capsule, deployment is incredibly simple.

### Step 1: Download the Virtual Machine Capsule
Download the single `ArchLinux_aarm64_Parallels.pvm` file directly from this repository (or from the Releases page) and save it to your local directory on your Mac (e.g., `~/Documents/Parallels/`).

### Step 2: Import into Parallels
1. Locate the downloaded file named **`ArchLinux_aarm64_Parallels.pvm`** (the official Parallels VM capsule).
2. Double-click the `.pvm` file to trigger Parallels Desktop.
3. When prompted with the dialog window **"Was this virtual machine moved or copied?"**, make sure to click **`Copied`**.
4. The system will automatically update its internal hardware bindings and boot into the GNOME login interface smoothly.

### Step 3: Run Post-Installation Tools
Once logged in, open the terminal and feel free to manage packages directly:
* Run standard updates: `sudo pacman -Syu`
* Use AUR packages out-of-the-box: `yay -S <package_name>`

---
*Author:Nomelonah.- Some issues are fixed by AI*
