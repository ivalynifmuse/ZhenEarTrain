# Changelog

Notable project changes are recorded here. Entries are grouped by date and use **Added**, **Changed**, and **Fixed** sections.

## 2026-10-21

### Changed

- Renamed the English brand from **ZhenEar** to **JaNear**, including the page title, wordmark, manual, and README.

### Added

- Renamed the app **臻耳朵训练室 / JaNear Listening Lab** and added a bilingual user manual in About & Settings covering exercises, metrics, app-only difficulty levels, spatial limits, and standards-backed terminology.
- Added reference links and definitions informed by ITU-R BS.1116-3, ITU-T P.811, ISO 532-2, ISO 266, and IEC 61260-1. Clarified that low/mid/high have no universal cutoffs for every task and that this app does not define certified grades.
- Expanded the band-identification choices to preferred one-third-octave center frequencies from 31.5 Hz to 16 kHz.
- Maintained the bilingual Chinese/English interface, multiple listening exercise types, local practice history, generated noise, and support for user-selected local audio.
- Added project acknowledgements describing the Harman “How to Listen” inspiration, the macOS Tahoe development context, and the project's unofficial status.

### Changed

- Reworked spatial localization as horizontal stereo-image localization, with normalized pan-coordinate error and app-specific tolerance. Removed the unsupported front/back and elevation interpretation.
- Renamed A/B controls to Reference / Change for non-EQ tasks; Flat / EQ now appears only for band-identification EQ/filter trials.
- Simplified task setup by showing attribute and filter options only when relevant and removing redundant task-category and session-test navigation. Task changes immediately refresh their matching controls, answer area, and bilingual labels; spatial wording stays consistent with the horizontal-only task.
- Published the project under the MIT License for its original code and documented that third-party trademarks and audio are not covered by that license.
- Added the direct live-demo URL to the repository metadata and README so visitors can open the app without first figuring out how to run the source file.

### Fixed

- Corrected inaccurate claims that two-dimensional screen clicks measured front/back localization. Documented browser, headphone, and calibration limits.
- Clarified that difficulty levels, score thresholds, and spatial hit tolerance are project-defined practice metrics, not Harman or ITU/ISO certifications.
