# Folder Fonts Installer

A simple, portable Windows CLI tool to install fonts from a folder.  
Intended to suit my need for an easy automated installation process of fonts on Windows.  
FontReg may be more suitable for most people's needs — you may want to check that out first.

---

## 📥 Download

👉 [Download folderfontsinstaller.exe](https://github.com/AC34/folder-fonts-installer-exe/releases/download/v1.0.0/folderfontsinstaller.exe)

> ⚠️ You must run the program as **Administrator** to install fonts correctly on Windows.

---

## 💡 Features

- Installs `.ttf`, `.otf`, and `.ttc` fonts from any folder
- Recursively scans subfolders
- Prevents duplicate installations
- Applies fonts immediately without reboot
- Lightweight, compiled into a single `.exe` file

---

##  📦 System Requirements
 - Windows 10 or later

 - Administrator privileges

---

## 🚀 How to Use

1. Download the `.exe` file from the [Releases page](https://github.com/AC34/folder-fonts-installer-exe/releases)
2. Right-click the `.exe` and **Run as Administrator**
3. Use the command line to specify options like the target folder and logging

### 🛠 Basic Syntax

```bash
folderfontsinstaller.exe --folder "C:\MyFonts"
```

#### ⚙️ Available Options

| Option      | Description                                               |
| ----------- | --------------------------------------------------------- |
| `--folder`  | Path to the folder containing font files (`.ttf`, `.otf`) |
| `--lang`    | Language for log messages (e.g., `en`, `jp`)              |
| `--verbose` | Enables detailed terminal output                          |
| `--log`     | Path to save a log file (e.g., `logs/output.log`)         |

---
### 🌐 Supported Languages
The installer supports multilingual log output via the --lang option:

| Language Code | Description       |
| ------------- | ----------------- |
| `en`          | English (default) |
| `jp`          | Japanese          |


ℹ️ If no --lang is specified, the tool detects your system locale.
If detection fails or the language is not supported, it defaults to English.

Example:
```
folderfontsinstaller.exe --folder "C:\Fonts" --lang jp
```


