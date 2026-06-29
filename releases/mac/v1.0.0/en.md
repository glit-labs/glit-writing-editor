# Glit Release Notes — v1.0.0

**Release date:** April 2026  
**First public release**

---

## Overview

Glit is a desktop writing app built for long-form fiction — in particular web novels. It runs natively on macOS and Windows via Electron and stores all files directly on the local filesystem.

---

## Core Features

### Web Novel Writing Mode

A dedicated mode for managing serialised fiction with a structured folder hierarchy.

- **Draft folder** holds in-progress episodes; **Completed Manuscripts folder** holds finished ones.
- **Range folders** group episodes into numbered arcs (e.g. 1–50, 51–100) and are managed automatically — episodes are assigned to the correct range as they are created.
- **Completed Manuscripts batch view** displays all finished episodes in a single scrollable list with per-episode and total character counts.
- Episode status (in-progress / complete) can be toggled; completed episodes open in read-only mode.
- **World-building folder** stores reference documents (character profiles, setting notes, etc.) alongside the manuscript.

### Multi-workspace Support

Multiple independent workspaces can be open at the same time. Each workspace maps to a folder on disk and appears as a separate entry in the sidebar.

### Editor

- Plain-text editor with configurable font size and line spacing.
- Auto-resizing textarea — the editor grows with the content; no fixed viewport height.
- **Find & Replace** bar with match highlighting and result list.
- Unsaved-changes confirmation dialog on file close or workspace switch.

### Multi-window Support

Files can be opened in additional floating windows — useful for referencing notes while writing in the main window.

### Image Inline Preview

Image files (`.png`, `.jpg`, `.gif`, `.webp`, etc.) open directly in the editor pane as an inline preview with zoom controls (− / + buttons and `Cmd/Ctrl+Scroll`).

### Markdown Preview Window

`.md` files can be opened in a standalone preview window that renders Markdown with full security sandboxing — external images are blocked and links open in the system browser.

### Multi-language Support

The UI is fully localised in **8 languages**: Korean, English, Japanese, Simplified Chinese, German, French, Spanish, and Italian. The language is detected automatically from the OS locale on first launch and can be changed in Settings.

### Themes

Four built-in colour themes: **Light**, **Dark**, **Sepia**, and **Dark Sepia**. Themes apply consistently across the main window and all secondary windows.

### Settings

- **Editor** — font size, line spacing, auto-save toggle.
- **Appearance** — theme selection, UI font size.

### macOS Support

Native build for macOS (Mac App Store). Uses the appropriate window chrome and keyboard conventions for the platform.
