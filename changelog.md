# Changelog

Release notes for every published version of Skitter.

## 1.1 (upcoming)

**Bug Fixes — Exercises & Music Theory**
- Tunings with sharps or flats (Half Step Down, Open D, Open E, and others) now produce correct pitches everywhere: tuner targets, exercise note names, Learn mode, and note-accuracy grading. Previously every sharp/flat string was treated as a natural note.
- Broken-interval exercises (Broken Thirds through Broken Tenths) now play correct intervals across the G→B string crossing. Previously several "octaves" in Broken Octaves were actually sevenths.
- Three-Notes-Per-String now plays the complete scale in position. Previously it skipped scale degrees at most string crossings and drifted far up the neck.
- CAGED System Positions now generates all five shapes in every key (previously four).
- Scale runs and circle exercises no longer repeat a note where two strings share the same pitch.

**Bug Fixes — Trophies & Records**
- The "First Perfect" trophy now requires a true 100% rhythm score. Previously it unlocked after almost any graded session. Trophies granted by this bug are automatically removed once and can be re-earned honestly.
- BPM personal bests and the 100/140 BPM trophies no longer count Learn-mode sessions — self-paced playing speed isn't a metronome record.
- The Personal Records card now shows a real per-exercise trend instead of always displaying "improving."

**Bug Fixes — Audio & Sessions**
- Phone calls, Siri, and alarms now pause the session cleanly instead of leaving the beat counter running silently. The tuner resumes automatically when the interruption ends, and rhythm grading picks up where it left off.
- Plugging in or unplugging an audio interface mid-use no longer freezes the tuner or rhythm grader, and the metronome resumes smoothly after output changes instead of firing a rapid burst of catch-up clicks.
- Rhythm grading is more accurate: beats are graded against the exact metronome click time, removing small device-timing jitter from scores.
- Learn mode can no longer advance two positions from a single sustained note.
- Ending a session template early now saves the partial exercise (matching single-exercise behavior) and properly stops the microphone.
- Backgrounding the app mid-template now pauses the session, preventing a burst of skipped beats on return.
- Fixed several rare instabilities caused by concurrent audio processing in the metronome, rhythm grader, and Learn mode.

**Bug Fixes — Notifications & Display**
- Key-of-the-Day notifications now announce each day's actual key. Previously every notification repeated the key from the day it was scheduled.
- The notation view now shows accuracy shapes for all feedback styles. Previously users with "String Glow" selected saw no accuracy feedback in notation.
- The exercises screen no longer shows a confusing empty-search message when only filters produced no results.

**Improvements**
- Every Skitter Pro prompt now includes an "Unlock Pro" button so you can purchase right where you hit the limit.
- Text size now follows your system Dynamic Type setting (within limits that keep the practice layouts intact).
- Long practice sessions use noticeably less battery: the fretboard and the scrolling tab/notation views were significantly optimized.
- VoiceOver: switches now announce their on/off state, and the navigation tabs announce which tab is selected.
- Free-tier limits are now applied consistently everywhere, including session templates and sessions launched from progressions.

**Removed**
- Dropbox backup has been removed. iCloud sync remains the supported way to back up and sync your practice data across devices. (Dropbox was never visible in the released app's interface; this removes the behind-the-scenes machinery and its documentation.)

---

## 1.0.1

**Bug Fixes**
- Fixed an issue where free users could access Intermediate and Advanced exercises through the Suggested list without being prompted about Skitter Pro. Suggested exercises now show a preview notice encouraging users to unlock Pro.
- Fixed starting fret changes in one exercise incorrectly carrying over to other exercises in progressions. Each exercise now remembers its own starting fret.
- Fixed Broken Octaves and other interval exercises skipping notes in Learn mode when consecutive notes share the same fret on different strings.

---

## 1.0

Initial public release.

**Features**
- Finger coordination exercises for guitar and bass: spiders, scales, arpeggios, intervals, and chord shapes
- Three display modes: fretboard diagram, tablature, and standard notation
- Metronome with multiple built-in click sounds and custom sound import
- Rhythm grader with real-time timing feedback and note accuracy validation
- Progression mode: structured multi-exercise plans with automatic BPM and duration ramping
- Session templates: build custom exercise sequences with per-exercise settings
- Guided First Week program for new players
- Trophies and achievements for practice milestones
- Saved presets for quick-launching favorite exercise configurations
- Practice history with detailed session logs
- Weekly goal tracking
- Left-handed mode with full fretboard mirroring
- Three dot-label modes: finger numbers, fret numbers, or note names
- Key-of-the-Day notification for varied practice
- 6-string guitar and 4-string bass support
- Custom tuning support
- Custom metronome sound import
- iCloud sync across Apple devices (optional)
- Dropbox backup for cross-platform data portability (optional)
- Privacy-first: no accounts, no tracking, no analytics, audio processed on-device
