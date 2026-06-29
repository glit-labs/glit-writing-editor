# Glit Release Notes — v1.1.0

**Release date:** 2026-05-31  
**Previous version:** v1.0.1

---

## New Features

### PDF Viewer

PDF files can now be opened inline in the editor and in a standalone window.

- Pages are rendered sharply at any zoom level.
- Zoom with the **−** / **+** buttons or `Cmd+Scroll` (macOS) / `Ctrl+Scroll` (Windows/Linux). The **⊡** button fits the page to the current window width.
- Text in the PDF can be selected and copied, with accurate selection highlights at any zoom level.
- An **↗** button opens the PDF in a standalone window with a custom toolbar (file name, zoom controls).
- PDF files display an extension badge in the sidebar and can be copied/pasted via the clipboard.
- PDF files are opened securely: scripts embedded in PDFs are disabled and external resource loading is blocked.

### Markdown Front Matter — Parsing and Visualization

YAML front matter at the top of `.md` files is now parsed and visualized.

- Front matter blocks surrounded by `---` delimiters are recognized and parsed.
- The front matter block is hidden from the preview, standalone window, and sub-sidebar — only the main content is displayed.
- In the editor, the front matter region is visually highlighted, with keys and values color-coded to match the active theme.
- The highlight updates automatically when the font size or line spacing changes.

### Markdown Preview — Click Image to Open in Image Viewer

Hovering over an image in the Markdown preview now shows an **"↗ Open in New Window"** overlay button. Clicking it opens the image in the standalone image viewer window.

### Text Files: Extension-Agnostic Copy/Paste and Editing

Files are now identified as text or binary by their content rather than by their extension. Files with unusual or missing extensions are opened in the editor and included in copy/paste operations as long as they contain no binary data.

### Close Related Windows When Workspace Is Closed

Clicking the **×** button on a workspace in the sidebar now closes all associated image, Markdown preview, and PDF windows that were opened from files within that workspace.

### External Drag-and-Drop: Folders and All Supported File Types

Dragging items onto the app previously only accepted image files. It now supports folders and all other supported file types (`.txt`, `.md`, `.pdf`, etc.), consistent with the clipboard paste behaviour.

### Clipboard Copy of External Files into Workspace

Files from outside a workspace can now be copied into it via the clipboard (`Cmd/Ctrl+C` → `Cmd/Ctrl+V`). Name conflicts are resolved with an automatic numeric suffix.

### Settings — Language Selector with Theme-aware Dropdown

The language selector in Settings now uses a custom dropdown that matches all four themes. It closes on outside click or Escape, and the selected language is highlighted with the accent color.

### Trash (Recycle Bin)

Deleted files and folders from the sidebar are now moved to a trash folder instead of being permanently deleted immediately.

- Deleted items are saved in a dedicated trash folder in the app's data directory, along with their original location and deletion time.
- **Settings → Trash** tab: items are grouped by workspace in card-style blocks, each showing the workspace name and full path on separate lines. Deletion timestamps and a file-tree preview for deleted folders are also shown.
- Each trash item displays its relative path within the workspace below the file name.
- Per-item **Restore** button and **Delete** button for permanent removal. A confirmation modal appears before any deletion.
- On restore conflict: a popup offers **Show All** (restores with a `_restored` suffix, incrementing if needed) or **Overwrite**.
- Per-workspace **Empty** and global **Empty All** buttons, each requiring confirmation. The **Empty All** button is highlighted with the accent color.
- The trash list updates in real time when an item is deleted from the sidebar.
- Full support for all 8 UI languages, with language-specific restore suffixes.

### Auto Backup

While you edit text files inside a workspace, backups are now created automatically to protect your work from unexpected errors or mistakes.

- **Session original**: Each time you save, a copy of the current content is saved to a hidden backup folder inside your workspace.
- **Periodic snapshots**: At the configured interval, a timestamped snapshot is saved. Identical consecutive snapshots are skipped, and the oldest snapshot is removed automatically when the limit is reached.
- **Settings → Auto Backup** section: enable/disable toggle, backup interval (default 5 min), maximum number of backups (default 10), and an optional "Auto-delete old backups" setting (off by default) with a configurable retention period (default 30 days).
- Only text files inside your workspace are backed up; binary files and files outside the workspace are excluded.
- The backup folder is hidden and does not appear in the sidebar.
- Full support for all 8 UI languages.

### Preview (DeviceView): Multiple Independent Windows

The preview (DeviceView) now supports multiple independent instances, one per episode.

- Right-clicking an episode in the sidebar now shows an **"Open Preview"** context menu item. Different episodes open in separate windows; clicking the same episode again focuses the existing window instead of opening a duplicate.
- The toolbar **Preview** button and **WnReview** panel preview button share one window per file, regardless of how the preview was opened.
- A **Preview** button has been added to the WnReview panel.
- Default font size increased from 9 px to 16 px.
- Preview windows save and restore font size, device selection, and window size/position across sessions.
- All preview windows close automatically when the main window closes.
- Full support for all 8 UI languages.

### Settings Panel Navigation: Resizable Width, Icons, and Labels

The side navigation panel in Settings can now be resized by dragging its right edge, and each tab now displays an icon alongside its label.

- Drag range: 120 px minimum to 300 px maximum; the chosen width is saved automatically.
- The panel width adjusts automatically to fit the longest label, ensuring correct display across all 8 UI languages.
- Five navigation icons added: editor, appearance, auto backup, trash, and info.
- The **Info** tab is anchored to the bottom of the navigation panel, separated by a divider line — matching the app's left sidebar footer layout.

---

## Bug Fixes

### Image/PDF Viewer: Horizontal Scroll (Panning) Not Working When Zoomed In

When zoomed in past the window width, scrolling left to view the left portion of the content was not possible. This is now fixed.

### Font Size Change Causes Incorrect Editor Bottom Margin

After changing the font size or line spacing, the editor sometimes cut off the last few lines of text at the bottom. This is now fixed.

### Markdown Preview Window Shows Bright Border Line (macOS)

On macOS, a bright line appeared along the edge of Markdown preview windows. This is now fixed.

### Preview Window Theme Not Synchronised in Real Time

Changing the theme while the Settings panel was open did not update preview windows immediately. This is now fixed.

### File Tree Displays `.DS_Store` Entries

On macOS, `.DS_Store` system files appeared in the sidebar file tree. They are now hidden.

### Editor Options Auto-save Toggle Button Displayed Incorrectly

The auto-save toggle button in the editor options panel was displayed incorrectly, with the thumb extending outside the track. This is now fixed.

### Multilingual: Preview Window Title Always Shown in Korean

When using the app in a language other than Korean, the preview window title was still displayed in Korean. This is now fixed.

### Sidebar: Extension Badge Border Not Removed When Sidebar Is Narrowed

When the sidebar was narrow enough to truncate a filename, the extension badge remained visible with its border. The badge is now hidden in this case.

### World-building / Background Folder: Paste Blocked in Web Novel Mode

Files could not be pasted into World-building or Background folders while Web Novel mode was active. This is now fixed.

### Sidebar: Three Inline Filename Rename Bugs Fixed

Three separate bugs in the inline rename flow have been fixed:

1. **Unsaved content loss on rename**: Renaming a file with unsaved changes now saves those changes first, so no content is lost.
2. **Silent overwrite on duplicate filename**: Renaming to an existing filename now shows a red border on the input and blocks the action until a unique name is entered.
3. **Invalid characters not blocked**: Names starting with `.` or containing `/` or `\` are now rejected with the same red-border treatment.

---

## Improvements

- The **sidebar resize handle** hit area has been widened, making it easier to grab without changing the visual appearance. Applied consistently to both the left sidebar and the right auxiliary sidebar, across all four themes.
- The **settings panel header** divider line is now aligned to the same height as the sidebar header, regardless of the UI text size setting.
- The **gear icon** on the sidebar's "Settings" button now scales proportionally when the UI text size is changed.
- The **UI text size** slider range has been extended from 16 px to 24 px. Additional interface elements now respond to the setting: sidebar header labels and action button icons, workspace name labels and web novel mode badges, web novel mode toggle button and icons, range folder and episode title inputs, web novel info panel labels/descriptions/buttons, and collapsed sidebar folder and hover action icons.
- When **creating or renaming** a file or folder, unsupported names (Windows reserved device names, names starting with `.`, names containing `/` or `\`, names ending with a trailing period or space, or excessively long names) are now blocked before the action is submitted, with a red-border input field and an inline error message. Supported in all 8 UI languages.
