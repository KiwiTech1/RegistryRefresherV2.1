# 🧰 Registry Key Refresher

A lightweight utility designed to refresh critical Windows Registry keys related to anti-cheat compatibility and system stability. Primarily intended to help resolve issues with **EAC (Easy Anti-Cheat)** and **BattlEye** where cheats or injected modules fail to load properly, even after installation and correct setup.

> ⚠️ **Disclaimer**  
> This tool is intended for **educational and debugging purposes only**. Do not use it to bypass or tamper with anti-cheat systems in a way that violates any game's terms of service. Misuse may result in bans or legal consequences.

---

## 🚀 Features

- Refreshes registry keys related to:
  - Kernel & driver loading behavior
  - TrustedInstaller permissions
  - Virtualization status
  - Hardware compatibility flags
- Works on both **x64 and x86** architectures
- No injection, patching, or system file modification
- Fast, portable, and open source

---

## 🛠️ Use Cases

- Troubleshooting failed cheat injection on **EAC**/**BattlEye**
- Resetting registry flags after system updates or anti-cheat blocks
- Prepping clean testing environments for development/debugging
- Avoiding "stuck" driver handles or invalid trust flags

---

## 📦 Installation

1. Download the latest `RegistryKeyRefresher.exe`
2. Run as Administrator
3. Let the tool complete the refresh
4. Reboot (if prompted)

---

## 🔍 How It Works

The tool scans and refreshes relevant registry entries in:

- `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services`
- `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall`
- `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager`

It optionally removes or resets conflicting flags such as:

- `StartOverride`
- `Type`
- `ImagePath` mismatches
- Driver loading restrictions that prevent injection

---

## 💡 Notes

- **Does not disable or bypass anti-cheats** — it simply helps resolve compatibility issues for tools that fail to inject or initialize properly.
- Always back up your registry before running any system tool.

---

## 🧪 Example Output

