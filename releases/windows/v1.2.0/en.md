---
date: 2026-06-30
---
# Glit Release Notes — v1.2.0

**Release date:** 2026-06-30  
**Previous version:** v1.1.1

---

## New Features / Improvements

### Theme Overhaul — System and Paper Added, Clean Removed

The theme lineup has been reorganized. The System and Paper themes have been added, and the Clean theme has been retired.

- **System**: A neutral palette that automatically follows the operating system's light/dark mode. When the system switches to dark mode, the body and title bar update immediately.
- **Paper**: A light, paper-like background with a calm navy accent color.
- If you were using the Clean theme, it is automatically migrated to Paper.
- The default theme for new installs remains Warmth, as before.

### Improved Identification of Unintended Line Breaks (Korean)

It was previously hard to tell automatic soft wraps apart from actual line breaks (Enter) while typing. This has been improved.

- **Show line breaks** toggle: displays a faint `↵` marker at each actual line break. It does not affect where the body text wraps, and is off by default.
- **Line-break mode** selection (Korean): choose between syllable-based (default) and word-based wrapping. Syllable-based wrapping matches the way web novel readers display text.

### Preview (DeviceView) — Settings Moved to an Options Popup

The device selector and font-size controls in the preview (DeviceView) toolbar have been consolidated into a "Settings" popup. The window title is now centered.

### Image Viewer UI Cleanup

The file name in the image viewer is now centered, and the zoom controls have moved to the right side of the bottom status bar.

---

## Bug Fixes

### Preview (DeviceView): Live Edits Not Reflected in Real Time

Edits made in the editor were not reflected in the preview (DeviceView) window in real time. This is now fixed.
