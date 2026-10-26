# Changelog

Notable project changes are recorded here. Entries are grouped by date and use **Added**, **Changed**, and **Fixed** sections.

## 2026-10-21

### Added

- Added an interactive moving-source continuity exercise: paired horizontal trajectories use the same pink-noise stimulus and browser HRTF panner; five-trial rounds let listeners identify the smooth path at three jump-detection levels. Playback must complete before an answer counts.
- Added a Spatial Audio workspace scaffold with research-screening dimensions (static localization, motion continuity, spatial acuity, externalization) and 3D mix-training lesson concepts. Includes playback-condition planning fields and an interactive horizontal motion-continuity exercise and a simple trajectory editor for start/end azimuth, curve shape and duration, using browser HRTF rendering. It does not run validated research screening or save screening data.
- Added a Formal Test section with independently selected objective tasks. Each task starts at Level 1, uses five trials per level, advances at four correct answers, and stops at the first failed level or after Level 12. Spatial trials require at least 80% pairwise ordering accuracy to count as correct; preference ratings are excluded.
- Added per-task manual Level 1–12 selection for training, alongside adaptive difficulty.
- Replaced spatial candidate cards with a compact horizontal player axis of draggable A–N markers. Clicking a marker toggles its audio; dragging changes rank and snaps markers to evenly spaced positions.
- Reworked Spatial Mapping into a replayable candidate-ranking task: listeners drag multiple panned candidates into left-to-right order. Level 1 starts with 3 candidates, adding one per level to 14 at Level 12; scoring uses pairwise ordering accuracy. Counts and scoring are JANEAR-defined, not a claimed Harman level schedule.
- Added a lossless ODAQ training excerpt (`26_claves/reference.wav`, CC0) to the material library, with download access and source/license details.
- Added a bilingual user manual in About & Settings covering exercises, metrics, app-only difficulty levels, spatial limits, and standards-backed terminology.
- Added reference links and definitions informed by ITU-R BS.1116-3, ITU-T P.811, ISO 532-2, ISO 266, and IEC 61260-1. Clarified that low/mid/high have no universal cutoffs for every task and that this app does not define certified grades.
- Expanded the band-identification choices to preferred one-third-octave center frequencies from 31.5 Hz to 16 kHz.
- Maintained the bilingual Chinese/English interface, multiple listening exercise types, local practice history, generated noise, and support for user-selected local audio.
- Added project acknowledgements describing the Harman “How to Listen” inspiration, the macOS Tahoe development context, and the project's unofficial status.

### Changed

- Reworked spatial localization as horizontal stereo-image localization and removed unsupported front/back and elevation claims.
- Renamed A/B controls to Reference / Change for non-EQ tasks; Flat / EQ now appears only for band-identification EQ/filter trials.
- Simplified task setup by showing attribute and filter options only when relevant and removing redundant task-category and session-test navigation. Task changes immediately refresh their matching controls, answer area, and bilingual labels; spatial wording stays consistent with the horizontal-only task.
- Published the project under the MIT License for its original code and documented that third-party trademarks and audio are not covered by that license.
- Added the direct live-demo URL to the repository metadata and README so visitors can open the app without first figuring out how to run the source file.

### Fixed

- Limited Band ID answer choices to a level-specific set of center frequencies (3 at Level 1, increasing to all 28 at Level 12), and selected each trial target only from the frequencies shown for that level.
- Removed the inspiration and rights section from the README as requested.
- Replaced the previous single-position choice with relative-order scoring, so small placement errors do not count as a full-trial miss. The spatial task hides the generic A/B transport controls and offers per-candidate playback.
- Added explicit stop controls for generated library previews and made the 60 Hz hum preview a finite, audible signal with low-order harmonics.
- Corrected inaccurate claims that two-dimensional screen clicks measured front/back localization. Documented browser, headphone, and calibration limits.
- Clarified that difficulty levels, score thresholds, and discrete location steps are project-defined practice metrics, not Harman or ITU/ISO certifications.
