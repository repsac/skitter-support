# Privacy Policy

**Last updated:** May 10, 2026

## What Skitter does with your data

**Nothing.** Skitter is an on-device practice tool. It does not collect, store, or transmit personal data. There is no user account, no analytics backend, no tracking, and no advertising.

## Microphone access

Skitter requests microphone access for two optional features: the **rhythm grader** (which listens for the timing and pitch of your playing) and the **tuner** (which detects your instrument's pitch for tuning). Audio from the microphone is processed entirely on your device, frame by frame, to estimate timing and pitch. **Audio is never recorded, saved, or sent anywhere.** The moment a frame has been analyzed, it is discarded.

If you deny microphone access, every other feature of the app works normally. The rhythm grader and tuner simply won't be available.

## Data stored on your device

Skitter uses Apple's SwiftData framework to persist your data locally:

- Practice sessions (date, exercise, BPM, duration, accuracy scores)
- Progressions and session templates you've created
- Saved exercise presets
- Earned trophies
- App preferences (display mode, metronome sound, starting fret, etc.)

All of this data stays on your device unless you opt in to one of the sync features described below.

## iCloud sync (optional)

If you enable iCloud sync in Skitter's settings and are signed in to iCloud, your practice data and preferences are synchronized across your Apple devices using Apple's CloudKit framework (private database).

- Sync is end-to-end managed by Apple. Skitter does not operate any server.
- The data stored in iCloud is limited to your practice sessions, progressions, templates, presets, trophies, and preferences. No audio, no usage analytics, no identifiers.
- You can disable iCloud sync at any time in Skitter's settings.
- Apple's privacy policy governs iCloud: <https://www.apple.com/legal/privacy/>

## Dropbox backup (optional)

If you connect a Dropbox account in Skitter's settings, your practice data and preferences are backed up to your personal Dropbox App folder using the Dropbox HTTP API v2.

- Data is stored in a private folder within your Dropbox account (`/Apps/Skitter/`). Only Skitter can read and write to this folder.
- Skitter stores an OAuth refresh token in your device's Keychain to maintain the connection. No Dropbox password is ever stored by the app.
- The data backed up is the same as what's stored locally: sessions, progressions, templates, presets, trophies, and preferences. No audio, no usage analytics, no identifiers.
- You can disconnect Dropbox at any time in Skitter's settings, which deletes the stored token from your Keychain.
- Dropbox's privacy policy governs data stored in your Dropbox account: <https://www.dropbox.com/privacy>

## App Store purchase

The one-time Skitter Pro in-app purchase is processed entirely by Apple's App Store. Skitter never sees your payment information. Your purchase is associated with your Apple ID for restore purposes.

## Crash reports and diagnostics

Skitter does not include any third-party crash reporter, analytics SDK, or tracking library. If you choose to share crash logs with Apple via **Settings → Privacy & Security → Analytics & Improvements**, Apple may include Skitter crash data in the reports they send to developers. This is controlled entirely by you through iOS's system settings.

## Children's privacy

Skitter does not knowingly collect data from any user, including children.

## Changes to this policy

If this policy ever changes in a material way, the update will be reflected here and noted in the app's release notes.

## Contact

For privacy questions, email **appstore@edcaspersen.com**.
