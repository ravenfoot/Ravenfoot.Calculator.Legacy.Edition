<h5><code>#!/usr/bin/env markdown</code><br>
<code>#==============================================================================</code><br>
<code># 🧮 RAVENFOOT CALCULATOR — LEGACY</code><br>
<code>#==============================================================================</code><br>
<code># Purpose: Simple standard calculator built with Python & Tkinter.</code><br>
<code># Audience: Reviewers; personal archive of early projects.</code><br>
<code># Stack: Python · Tkinter</code><br>
<code># Version: 0.x (Legacy)</code><br>
<code># License: (see repo)</code><br>
<code># Status: Archived / Learning Project</code><br>
<code># Author: Ravenfoot</code><br>
<code>#==============================================================================</code></h5>

## 0. 🧬 Ravenfoot projects

* **a)** Ravenfoot Calculator (Legacy) <--- You are here
* **b)** [Ravenfoot Passwords — P100 (Teletext Edition)](https://github.com/ravenfoot/Ravenfoot.Passwords.P100.Teletext-Edition)
* **c)** [Ravenfoot Rune Timer (Dota 2)](https://github.com/ravenfoot/Ravenfoot.Rune.Timer.Dota.2)
* **d)** [Ravenfoot NAS Automation (Bash Edition)](https://github.com/ravenfoot/Ravenfoot.NAS.Automation.Bash.Edition)
* **e)** [Ravenfoot Webpage](https://github.com/ravenfoot/Ravenfoot.Webpage)
* **f)** [Ravenfoot Scryer — AoW Overlay (Stage 1)](https://github.com/ravenfoot/Ravenfoot.Scryer.AoW.Overlay.1)


## 1. 📜 Origin Story

This was **Project Zero**.

My very first attempt at building a GUI application with Python. No AI assistance, no advanced frameworks, just me fighting with `Tkinter` grids and global variables.

It represents the start of the coding journey. While the code is rough by modern standards, it remains fully functional and stands as a testament to learning the basics the hard way.

**⚠️ Recent Polish (2024):⚠️**
I recently dusted off this project to give it a professional "packaging" treatment. It now includes:
* **Dynamic Icon Loading:** Automatically detects OS (Windows/Linux) and loads the correct `.ico` or `.png`.
* **Resource Bundling:** Uses `sys._MEIPASS` handling to ensure icons work inside compiled executables.
* **Code Refactoring:** Added comments and cleaned up unused imports while preserving the original "legacy" logic.

---

## 2. ⚡ Capabilities

* **Basic Arithmetic:** Addition, Subtraction, Multiplication, Division.
* **Input Handling:** Clickable UI buttons (no keyboard binding).
* **Clear Function:** Wipes the memory state.
* ⚠️**Cross-Platform:** Now runs natively on Windows and Linux.⚠️

---

## 3. 🛠️ Tech Stack

* **Language:** Python 3.x
* **GUI Library:** Tkinter (Standard Lib)
* **IDE:** PyCharm (The original dojo)
* **Build Tool:** PyInstaller
* **Packaging:** DEB (Debian/Ubuntu), EXE (Windows)

---

## 4. 🚀 Usage

```bash
# Clone the repo
git clone [https://github.com/ravenfoot/calculator_legacy.git](https://github.com/ravenfoot/calculator_legacy.git)

# Run the script
python ravenfoot_calculator.py
```
Or

## 5. 📦 Build Instructions

This project includes build steps to generate standalone executables for Windows and installable packages for Linux.

**🪟 Windows (.exe)**
Run this command in a Windows environment (Powershell/CMD):

PowerShell
```Bash
pyinstaller --noconfirm --onefile --windowed --name "Ravenfoot Calculator" --icon "ravenfoot_icon.ico" --add-data "ravenfoot_icon.ico;." ravenfoot_calculator.py
Output: dist/Ravenfoot Calculator.exe
```

**🐧 Linux (.deb)**
Generate the binary (ensure you are on Linux):

```Bash
pyinstaller --onefile --windowed --name "ravenfoot-calc" ravenfoot_calculator.py
Package into .deb (requires standard directory structure):
```
**Move binary to staging**
```Bash
cp dist/ravenfoot-calc build/deb/ravenfoot-calc/usr/local/bin/
```
**Build package**
```Bash
dpkg-deb --build build/deb/ravenfoot-calc
Output: build/deb/ravenfoot-calc.deb
```
OR

just download:

**🐧 Linux (.deb)**

* **a)** [Ravenfoot Passwords — P100 (Teletext Edition)](https://github.com/ravenfoot/Ravenfoot.Calculator.Legacy.Edition/releases/download/Linux_Software_Package/ravenfoot-calc.deb)

**🪟 Windows (.exe)**
* **b)** [Ravenfoot Passwords — P100 (Teletext Edition)](https://github.com/ravenfoot/Ravenfoot.Calculator.Legacy.Edition/releases/tag/Windows_Executable_Binary)

<code>#==============================================================================</code><br>
<code>#🛑 END</code><br>
<code>#==============================================================================</code></h5>
