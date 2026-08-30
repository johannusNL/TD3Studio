# Changelog

## 1.1.0 — 2026-08-30

A feature release: the track, and the TD-3's setup without SynthTribe.

- **The TRACK**: queue patterns with the + in the library or TO TRACK on the plate, and they play back to back, handing over exactly on the bar. The bay under the keyboard reorders them with arrows, renames them in place, and a double-click puts one back on the plate. Write to... stores the track as a run of slots on the device, with a step-by-step walkthrough to save it as a real track there.
- **Device setup...** under the setup key: the TD-3's own settings over USB — MIDI channels, accent threshold, key priority, multi-trigger, clock, transpose, pitch bend range — plus the firmware version. No SynthTribe needed.
- **READ** next to WRITE fetches any slot onto the plate; READ, pick another slot, WRITE is the panel's copy/paste.
- **RANDOM** next to CLEAR rolls a fresh acid line on the minor pentatonic, with rests, ties, accents, slides and octave jumps.
- The up octave is reachable at last: scrolling a cell walks past the upper C to C# up … B up and the top C. + / - move the selected step an octave; Ctrl + / - transpose the whole pattern a semitone, with Shift an octave.
- A long MIDI file's + asks to place the window on the plate first; the introduction grew a card that demonstrates the track.

## 1.0.7 — 2026-08-30

- Windows: settings now live in `%APPDATA%\TD3 Studio` (the folder carried the project's old working name); settings saved by an earlier build move over automatically.
- Housekeeping under the hood: the code base carries the product name throughout.

## 1.0.6 — 2026-08-30

- macOS: the update check and Report an issue work again. A stray newline in the build's baked-in token made every request fail — the check then pretended you were up to date, and a report ended in "authorization header is not a string".

## 1.0.5 — 2026-08-30

- The step cells reach the up octave: scrolling a cell walks past the upper C into C# up through B up, to the C two octaves above the root — the same range the TD-3 itself plays.
- New shortcuts: + and - move the selected step an octave up or down (the TD-3's up/dn transpose), keeping the note.
- The help explains the up/dn octave flag shown under a step's note.

## 1.0.4 — 2026-08-28

- Report an issue or request a feature...: the form now has two categories, Something is wrong and Feature request, so requests land in the right place.

## 1.0.3 — 2026-08-27

- Report an issue... is now a form inside the app: what happened plus an optional e-mail address, sent with your version and setup attached. No GitHub account needed.

## 1.0.2 — 2026-08-27

- Links open in the browser again: Credits and Report an issue... did nothing on both Windows and macOS.

## 1.0.1 — 2026-08-27

- macOS build (Apple Silicon and Intel, macOS 11 or later) as a disk image; settings live in `~/Library/Application Support/TD3 Studio`.
- Small screens: the instrument scales down so a 13-inch laptop fits the plate with both the HELP and LIBRARY housings open; the window shrinks to the screen it opens on.
- The update check picks the installer for its platform; on macOS the downloaded disk image opens in Finder.
- On a Mac the modifier keys read Cmd and Option: Cmd+Z undoes, Cmd + scroll zooms the timeline.
- Report an issue... under the setup key opens a GitHub issue with the version and your setup filled in.

## 1.0.0 — 2026-08-27

First release.

- MIDI file to TD-3 pattern, with a timeline window over the clip: drag, scroll, step by bar, Ctrl + scroll to zoom.
- The plate: sixteen step cells with note, octave, accent and slide; scroll to transpose, modifier-click for accent, slide, tie and rest; undo.
- Three-octave screen keyboard with 303-style step recording; MIDI keyboard input with velocity accents and legato slides.
- Output to the TD-3 over USB, any MIDI output, or the built-in simulator (saw / square, filter, envelope, accent, slides).
- WRITE to a slot on the device; BACKUP of all 64 patterns.
- Library of `.syx`, SynthTribe `.seq` / `.sqs` and `.mid` files with thumbnails and audition; 107 bundled Acid-Tabs patterns; online MIDI search.
- Introduction tour, help panel and hover explanations.
- Automatic update check, once a day.
