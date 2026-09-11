# Changelog

## 1.3.0 — 2026-09-11

Pattern length on the plate, and an update ring.

- **STEPS** beside BANK B sets the pattern's length — the same one FUNCTION + STEP sets on the TD-3. Use - and +, or scroll over it like a note; the cells past the last step go dark. The length is stored in the pattern, so it goes to the device with every WRITE. Before, the length and triplet time could only be set through the MIDI conversion; both now edit any pattern, from the library or an empty one, and the Pattern settings in the HELP housing show for every loaded pattern.
- Changing the length no longer rebuilds a converted clip, so hand edits survive it.
- **Update ring**: under the setup key, choose *Updates: the latest build* or *Updates: one version behind*. One behind keeps you on the release before the newest — a fresh release waits until the next one is out — and from the newest it offers that release as a step back, clearly marked, with its own button. Windows, macOS and Linux.

## 1.2.0 — 2026-09-08

Linux, Spanish, and a quieter scroll wheel.

- **Linux**: TD3 Studio now ships as an x86_64 AppImage (Ubuntu 22.04 or newer, any distribution from 2022 on). The first start from the AppImage puts the app in the app menu and lets you pin it to the dock; the updater replaces the AppImage in place. MIDI goes through ALSA, so the TD-3 must show up in `aconnect -l`. Runs on a roomier audio buffer so the simulator does not crackle under PipeWire or in a virtual machine.
- **Spanish interface**: pick the language at the first start or under the setup key. Everything in the app is translated; the plate's own printing stays as on the TD-3.
- Scroll wheel: turning a cell, a knob, the selector or the timeline no longer scrolls the whole window along.
- Help: a new topic *The TD-3 in a DAW* — Ableton MIDI and audio routing, External Instrument, sync, and what TD3 Studio does and does not do next to a DAW. READ joined the plate topic.

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
