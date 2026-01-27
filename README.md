# Disciples 2: Rise of the Elves Editor (ROTE Editor)

A WinForms editor for **Disciples II: Rise of the Elves** that allows you to view and modify game data (units, attacks, stats, and more) using a safe workflow: **load → edit → review changes → save**.

> ⚠️ This tool is aimed at Disciples II: Rise of the Elves, but you also could use it to modify/edit **another versions** of Disciples2, **MODS**, or even create your own mode.

---

## ✨ Features

⚠️Disclaimer: Most of the described parts of the editor have **hotkeys** for tools and for their functions 

### ✅ Translations
The editor's main menu language will be set according to the game's internal language.
The tools or functions in English. The translations of the **MODS** could be broken, but it is just a description. Main functions are still available.

### ✅ Unit editing
- Browse units and edit core stats:
  - HP, Armor, Regen
  - XP to next level / XP when killed
  - size flags, attack flags, etc.
- Edit unit descriptions and combat-related fields
- Edit Attack 1 / Attack 2 links and related parameters
- View unit portrait preview (from game resources)
- **Double-click** the unit portrait to open **Media → Resource Explorer** and jump to the unit’s **FACEB** image in **Faces.ff**

### ✅ Media (browse & preview game assets)
- **Resource Explorer** (Media → Resource Explorer)
  - Browse `*.ff` files from **Imgs\** and **Interf\**
  - Fast filtering/search by file name and item name (e.g., `FACEB`, `0177`)
  - Preview images/animations and export selected items (if enabled in your build)
- **Media Explorer** (Media → Media Explorer)
  - Browse sound containers `*.wdb` / `*.wdt` plus folders: **SoundsP**, **MusicP**, **Music**, **Briefing**, **Video**
  - Play audio and preview videos inside the window (and also open externally)
    > All data could be exported to a clear format (editing, modifying)

### ✅ Smart change tracking (per unit)
- Highlights changed fields directly in the UI
- Supports editing multiple units before saving
- The save list shows what will be applied
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

### ✅ Debug settings (optional)
“Debug Settings” contains experimental tools (for advanced users).

### ✅ Script manager
Gives you the possibility to create a dedicated patch for your changes (if you want to apply them to some mode, campaign, or map that you created)
That function allows you to install those changes and return them to the default (without the editor). 
For advanced users: you could insert the script into the installation process of your setup.

### ✅ Simple DB editor
Save your time and give you access to the DBs of the game for manual editing. The function "save" is present

### ✅ Simple Internet Browser 
Inside the **HELP menu**, you could use the help window like an internet browser if you need to search for something. 
It doesn't have most of the functions of browsers, but it is still useful for simple searches. 
Has a **"HOME"** button for returning to the help window.

### ✅ About menu
Has a checker for the new version of the editor. If the new version becomes available, you will receive a message about this and a direct link to download it

---
## 📦 Installation

### Requirements
- Windows 10/11
- .NET (the editor is built using WinForms)
- A copy of **Disciples II: Rise of the Elves** installed

### Download
Go to the [**Releases**](https://github.com/Vanosz/Disciples2-ROTE-Editor-Releases/releases) page of this repository and download the latest build.

---

## 🚀 How to use

### 1) Open the game
1. Launch the editor
2. Click **Open**
3. Select your `Discipl2.exe` file  
   The editor will detect and load the required DB data.

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
Click **Save** to apply edits to the DB files.

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
- Use Change History/backups
- Prefer incremental saves instead of doing everything at once

---

## ⚠️ Disclaimer
This project is a fan-made tool for modding and learning.  
Not affiliated with the original developers of Disciples II.

You can use it at your own risk.

---

## 📸 Screenshots

### Main menu
<img width="1145" height="912" alt="image" src="https://github.com/user-attachments/assets/e447a9eb-6445-425a-bf25-7b9554b257a2" />

### Backup Manager
<img width="1082" height="641" alt="image" src="https://github.com/user-attachments/assets/4a2da7f2-3501-46bb-a141-38b6a0231b82" />

### Simple DB Editor
<img width="2278" height="1228" alt="image" src="https://github.com/user-attachments/assets/a4914ca3-b81e-47ad-8437-e9fe8a22f9fc" />


---

## ❤️ Credits
- Inspired by community modding tools and reverse engineering work
- Built by **Vano_sz**
- [Support developer](https://ko-fi.com/vano_sz)
