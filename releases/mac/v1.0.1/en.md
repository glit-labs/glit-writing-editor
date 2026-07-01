---
date: 2026-05-01
---
# Glit Release Notes — v1.0.1

**Release date:** May 2026  
**Previous version:** v1.0.0

---

## New Features

### Right-side Auxiliary Sidebar (Inline Preview Panel)

A new toggle button on the right side of the toolbar opens an inline preview panel on the right edge of the app.

* Markdown files are rendered with the same security policies as the existing preview (external images blocked; links open via the system browser only).
* The panel width can be adjusted by dragging, and the setting is automatically saved.
* The save status indicator ("Saving" / "Saved") has moved from the toolbar button to a text label in the top-right corner of the editor for a cleaner look.

### Sidebar Item Selection Highlight

Clicking a file or folder in the sidebar now shows a **selection state (border outline)**.

* The selected item (border) is visually distinct from the actively edited file (orange background), and both states can appear simultaneously.
* Clicking a sidebar item transfers focus to the sidebar panel without disrupting the editor's internal focus.

### Right-click Context Menu and Copy/Paste Shortcuts

Right-clicking a sidebar item opens a context menu with the following actions:

| Action | Description |
|--------|-------------|
| New Document | Create a new file inside the selected folder |
| New Folder | Create a new subfolder inside the selected folder |
| Show in Finder | Reveal the item in the OS file manager |
| Copy | Copy the file or folder to the clipboard |
| Paste | Paste the copied item into the current folder (name conflicts are resolved with an automatic suffix) |
| Rename | Rename the item inline |
| Delete | Delete the item |

Keyboard shortcuts: `Cmd+C` / `Cmd+V`

> When a sidebar item is clicked, focus shifts to the aside panel so clipboard shortcuts do not conflict with editor paste operations.

### Global UI Font Size Setting

The UI font size configured in Settings is now applied consistently across **all components** — sidebar, editor, search bar, toolbar, and settings panel. Previously, several areas used hardcoded sizes that ignored the setting.

### World-building Folder File Move, Sort Improvements, and Image Badges

* Dragging items within the world-building folder now correctly triggers filesystem moves.
* Image files (`.png`, `.jpg`, etc.) in the sidebar now display an extension badge.
* Drag-to-reorder within world-building folders works correctly.

### File Info Panel in the Right Sidebar

A new **File Info** toggle in the right-side auxiliary sidebar displays detailed metadata for the currently open file.

* Shows: file name, workspace, format, file size, character count (with and without spaces), creation time, last modified time, and full path.
* File size updates automatically whenever the file is saved.
* In Web Novel mode during the **Completed Manuscripts batch view**, the panel switches automatically to an aggregate stats view showing episode count and total character counts. A "Details" toggle expands a per-episode character count breakdown.

### Edit Options Panel — Correction Tools (Web Novel Mode)

Three correction sections are now available in the Edit Options panel when Web Novel mode is active.

**Quote Correction**

| Action | Description |
|--------|-------------|
| Curly → Straight | Converts curly/smart quotes to straight ASCII quotes |
| Straight → Curly | Converts straight ASCII quotes to curly quotes |
| Dialogue Style | Normalises dialogue formatting |

**Punctuation Correction** _(Korean only)_

| Action | Description |
|--------|-------------|
| Period → Middle Dot | Replaces `...` ellipses with the `···` middle-dot style |

**Indent Correction**

| Action | Description |
|--------|-------------|
| Paragraph Indent | Normalises leading whitespace at the start of each paragraph to a single space |

While a correction is running, the editor is covered by a non-interactive overlay to prevent accidental edits. Each button shows a progress indicator (`···`) during processing and a brief confirmation highlight on completion.

---

## Bug Fixes

### File Rename Leaves Editor State Stale — Saves to Wrong Path

When a file was renamed in the sidebar while open in the editor, `currentFile.path` and the `draftBuffer` key were not updated. This caused subsequent saves to create a new file at the **old (deleted) path**. The editor state is now updated immediately on rename.

### Episode Read-only State Not Reflected Immediately

Changing an episode's status to "Complete" inside a range folder did not switch the open editor to read-only mode until the file was reopened. The `currentFile.isEpisodeDone` flag is now updated in real time.

### Text Search Results Not Cleared When Closing a Workspace

Search results from a previous workspace persisted on screen after the workspace was closed. Results are now cleared on workspace close.

### Multilingual Initial-load Flash and Language-change Bug

* A brief flash of the wrong language at startup has been eliminated. The locale is now loaded synchronously in the preload phase so the correct language is shown from the very first render.
* Switching languages in Settings no longer leaves parts of the UI in the previous language.
* Some languages were missing from the Settings language dropdown; the list now includes all available locales.

### Range Folder Reorganization Deletes Leading Episodes

When a range was shrunk, episodes that fell outside the front boundary of the new range were incorrectly deleted from the list. This is now fixed. A related NFC normalization issue (Korean filenames returned as NFD by Google Drive) that caused reorganization to fail is also resolved.

### Drag-and-drop Restricted to Prevent Folder Contamination

Dragging items from outside into the Draft or Completed Manuscript folders is now blocked. This prevents accidental file placement in managed folders.

### Quote Correction Preview Shows Wrong Characters

In the Edit Options panel (Web Novel mode), both the **Curly → Straight** and **Straight → Curly** items in the Quote Correction section displayed the same characters on both sides of the arrow, making the two options visually indistinguishable. The result side of each example now correctly shows straight ASCII quotes and curly quotes respectively.

---

## Improvements

* The **character count** is now shown in the top bar of read-only editors, and the bar layout has been improved ("Read Only" centered; character count and preview button right-aligned).
* The **total character count** is now displayed at the top of the Completed Manuscripts batch view.
* After a drag-move operation, `draftBuffer` internal paths are updated correctly so subsequent saves go to the right location.

---

## Internal Changes

* Removed unnecessary `console.error` debug log statements.
* Removed dead code and redundant IPC calls from the multilingual system.
* Added `.claude/settings.local.json` to `.gitignore`.
* Removed the GitHub releases-based self-update checker (automatic banner and manual check button). macOS is distributed exclusively through the Mac App Store; updates are handled automatically by the store.
