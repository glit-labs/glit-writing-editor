# Glit Release Notes — v1.1.1

**Release date:** 2026-06-03  
**Previous version:** v1.1.0

---

## Improvements

### Windows: Title Bar Color Synced with App Theme

All windows (main, preview, Markdown, image, PDF) now use the Window Controls Overlay style, replacing the native title bar with the existing Toolbar component. System button colours (minimise, maximise, close) update immediately when the theme changes.

- macOS retains its existing `hiddenInset` behaviour.

### Empty Screen — [Open Folder] / [Start Web Novel] Buttons

The placeholder text shown in an empty editor area has been replaced with two action buttons.

- **[Open Folder]**: opens a folder as a new workspace.
- **[Start Web Novel]**: launches web novel writing mode directly, with a modal that branches based on the number of existing workspaces.
- Button accent colour reflects the active workspace and web novel mode state.
- Full support for all 8 UI languages.

### Web Novel Mode: Folder Tree Auto-Expand on Activation

When web novel mode is turned on, the Story, In Progress, World-building, and Completed folders expand automatically so the project structure is immediately visible without any extra interaction.

---

## Bug Fixes

### Windows: Images, PDF Content, and Markdown Images Not Displayed

Images embedded in the editor, PDF viewer content, and Markdown preview images were not displayed on Windows. This is now fixed.

- Replaced `net.fetch('file://')` (which fails on Windows) with `fs.readFile`.
- Fixed Windows drive-letter path normalisation (leading slash removal and colon restoration).
- Normalised backslashes in PDF standalone window paths.
- Preserved colons in Markdown image URIs by switching from `encodeURIComponent` to `encodeURI`.

### Windows: Title Bar Button Hover Colour Not Visible in Midnight Theme

The hover colour for native title bar buttons was invisible against the dark background of the Midnight theme on Windows. `nativeTheme.themeSource` is now synced with the active theme so that the correct dark/light mode hover colour is applied.

