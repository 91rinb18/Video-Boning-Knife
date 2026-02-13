# Changelog

[简体中文](./CHANGELOG_CN.md) | **English**

## [1.2.18] - 2026-02-14
**Core keywords: Stability, Localization, Ultimate Polish**

### Changed
- Deep localization: Unified professional terms like "Extract/Mux/Split".

### Fixed
- Script engine enhancement: Fixed escaping errors in complex file paths (Syntax/Escaping fix).

### UX
- Smart directory management: Prevents path errors.

### UI
- Layout adaptive fix: Resolved button occlusion in "About" window on high-DPI scaling screens.

## [1.2.12] - Maintenance Update
**Core keywords: Multi-threading, Logging, Anti-freeze**

### Performance
- Asynchronous analysis engine: Introduced multi-threading for file analysis, completely solving UI "white screen/freeze" on large files (e.g., 4K HDR movies).

### Added
- Real-time log system: New scrolling log window displaying FFmpeg process status in real-time.

### Fixed
- Container compatibility patch: Fixed PS container recognition crash.
- Fixed command parsing exceptions caused by carriage return/line feed issues on some Windows systems.

## [1.2.5] - Detail Perfection
**Core keywords: Icons, Path Compatibility, Split Warnings**

### Improved
- Path compatibility: Refactored path parsing algorithm for perfect support of Windows paths with spaces/special characters.

### UX
- Smart guidance: Added keyframe warning in "Lossless Split" module, alerting users to precision limits in lossless mode.

### Fixed
- Fixed NameError crashes from color variable references in specific operations.

## [1.2.0] - Major Update (Midnight Nebula)
**Core keywords: New UI, Drag & Drop, Deep Analysis**

### Refactored
- Visual overhaul: Introduced "Midnight Nebula" design language with dark blue frosted glass style, reducing eye strain for nighttime use.

### UX
- Drag & Drop streams: Support direct drag of files into main interface or specific track slots.

### Core
- FFprobe deep integration: Auto-analyze codec formats (HEVC/AVC/AAC etc.) upon drag-in, no manual inspection needed.

### Fixed
- Resolved interface layout collapse and jitter across different resolutions.

## [1.1.5] - Logic Enhancement
**Core keywords: Smart Containers, Codec Mapping**

### Smart Features
- Auto container switching: In Mux mode, switches to MKV if MP4 incompatible streams detected.

### Core
- Codec mapping table: Built complete codec-to-extension mapping library, greatly improving extraction success rate.

### Fixed
- Fixed out-of-order timestamp issues.

## [1.1.0] - Feature Expansion
**Core keywords: Three-in-One, Split, Mux**

### Added
- Modular architecture: Established Extract, Split, Mux as three core modules.
- Lossless splitting: Millisecond-level cutting via `-ss` and `-to` (keyframe-limited).
- Stream muxing: Lossless muxing of separate video/audio/subtitle files into one.

## [1.0.0] - Official Release
**Core keywords: Desktopization, Lossless Philosophy**

### Released
- Architecture transition: Migrated from web prototype to Python desktop app for fully offline operation.

### Core
- "Re-encoding Refused" philosophy: All operations use `-c copy` for 100% lossless quality and speed.

### Added
- Basic track extraction functionality.

---
© 2026 91rinb18. All rights reserved.
