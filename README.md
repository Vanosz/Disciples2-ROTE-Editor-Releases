# Disciples 2: Rise of the Elves Editor (ROTE Editor)

A WinForms editor for **Disciples II: Rise of the Elves** that allows you to view and modify game data (units, attacks, stats, and more) using a safe workflow: **load → edit → review changes → save**.

> ⚠️ This tool aimed on Disciples II: Rise of the Elves but you also could use it to modify\edit **another versions** of Disciples2, **MODS** or even create your own mode.

---

## ✨ Features

### ✅ Unit editing
- Browse units and edit core stats:
  - HP, Armor, Regen
  - XP to next level / XP when killed
  - size flags, attack flags, etc.
- Edit unit descriptions and combat-related fields
- Edit Attack 1 / Attack 2 links and related parameters
- View unit portrait preview (from game resources)

### ✅ Smart change tracking (per unit)
- Highlights changed fields directly in the UI
- Supports editing multiple units before saving
- Save list shows what will be applied
- Changes are grouped per unit for clarity

### ✅ Safe save workflow
- “Nothing to save” protection
- Only saves actual changes (no noise / fake diffs)
- Confirmation prompts for destructive actions

### ✅ Reset unit (session reset)
- **Reset unit** restores the currently selected unit to the values loaded at the start of the session:
  - Removes unsaved edits for that unit
  - Does not affect other units
  - Does not write anything to disk (until you save)

### ✅ Change History / Backup system (recommended)
- Stores steps in history so you can restore previous states
- Helps prevent accidental edits and allows safe rollback

### ✅ Debug tools (optional)
Hidden “Debug Settings” contains experimental tools (for advanced users).

---

## 📦 Installation

### Requirements
- Windows 10/11
- .NET (the editor is built using WinForms)
- A copy of **Disciples II: Rise of the Elves** installed

### Download
Go to the **Releases** page of this repository and download the latest build.

---

## 🚀 How to use

### 1) Open the game
1. Launch the editor
2. Click **Open**
3. Select your `Disciples2.exe` file  
   The editor will detect and load required DB data.

### 2) Edit units
- Select a unit from the unit list
- Modify values in fields (stats, description, attacks)
- Changed fields will be highlighted

### 3) Review changes
Open the **Save changes** window to review:
- Which units were modified
- Which fields were changed
- Before → After values

### 4) Save changes
Click **Save** to apply edits into the DB files.

---

## ♻️ Reset unit

You can reset the current unit to session defaults:
- Select a unit
- Click **Reset unit**
- Confirm action

This restores only the currently opened unit to the values loaded at session start.

---

## 🧠 Tips / good workflow

✅ Recommended safe editing flow:

1. Make a small number of changes  
2. Save and test in-game  
3. Repeat  

If you do big edits:
- Use Change History / backups
- Prefer incremental saves instead of doing everything at once

---

## 🛠️ Development (for contributors)

### Build
1. Clone the repo
2. Open the solution in Visual Studio
3. Build in `Release` mode
4. Run the editor

### Code structure notes
- WinForms UI is built around data grids + change tracking
- Editing workflow uses:
  - per-unit snapshots
  - per-unit pending changes
  - baseline comparison for highlighting

---

## ⚠️ Disclaimer
This project is a fan-made tool for modding and learning.  
Not affiliated with the original developers of Disciples II.

Use at your own risk.

---

## 📸 Screenshots

### Main menu
<img width="1145" height="912" alt="image" src="https://github.com/user-attachments/assets/e447a9eb-6445-425a-bf25-7b9554b257a2" />

### Backup Manager
<img width="1082" height="641" alt="image" src="https://github.com/user-attachments/assets/4a2da7f2-3501-46bb-a141-38b6a0231b82" />

### Simple DB Editor
<img width="2278" height="1228" alt="image" src="https://github.com/user-attachments/assets/4325e76a-d4f2-44ca-b0a5-5567610dc1ba" />

---

## ❤️ Credits
- Inspired by community modding tools and reverse engineering work
- Built by **Vanosz**
