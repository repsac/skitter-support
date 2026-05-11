# Troubleshooting

Quick answers to the most common questions. If your issue isn't here, email [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com) with a short description and what device / iOS version you're on.

## The metronome isn't playing

1. Check that your device isn't in silent mode (flip the physical mute switch on the side of your iPhone/iPad).
2. Make sure the volume is up. Skitter uses the media audio channel, not the ringer channel.
3. If you're using a Bluetooth speaker or headphones, confirm they're connected and playing audio from other apps.

## The rhythm grader isn't detecting my playing

1. Check that microphone permission is granted. Open iOS **Settings → Privacy & Security → Microphone** and confirm Skitter is toggled on.
2. In Skitter, go to **Settings → Audio Input** and confirm the "Active Input" reads a real device.
3. Try adjusting **Settings → Timing Sensitivity**. If set to Strict, even small timing deviations register as misses. Try Relaxed to start.
4. If you're using a USB-C audio interface, make sure the input gain is set high enough for Skitter to pick up your playing.

## Rhythm scores seem wrong

- The grader listens for note onsets (the moment you pluck a string) and compares them to the metronome beat. If you're consistently early or late, the score reflects that.
- **Timing Sensitivity** in Settings controls how strict the grading is. Relaxed allows a wider window; Strict expects near-perfect timing.
- If note accuracy is enabled (**Settings → Rhythm Grader → Grade Note Accuracy**), playing the wrong fret or string will also count against you.

## The fretboard looks wrong or mirrored

- If you're left-handed, make sure **Settings → Display → Left-Handed Mode** is on. This mirrors the fretboard so the lowest string appears on the right.
- If the fretboard seems too small or too large, adjust **Settings → Display → Display Size**.

## iCloud sync isn't working across devices

- Confirm both devices are signed in to the same iCloud account.
- Confirm iCloud Drive is enabled: **iOS Settings → your Apple ID → iCloud → iCloud Drive**.
- CloudKit sync can take a few seconds on Wi-Fi, up to a minute on cellular. It's not instant.
- Try closing and relaunching the app on the receiving device.
- After toggling iCloud sync on or off in Skitter settings, the change takes effect the next time you open the app.

## Dropbox sync isn't working

1. Open **Settings → Data & Privacy** and confirm Dropbox shows "Connected."
2. Tap **Sync Now** to force an immediate sync.
3. If you see an error, try disconnecting and reconnecting. Go to **Settings → Data & Privacy → Disconnect**, then tap **Connect** again.
4. Confirm you have an internet connection. Dropbox sync requires network access.
5. If the sync was working and suddenly stopped, your Dropbox token may have expired. Disconnect and reconnect to refresh it.

## A progression or template I created disappeared

Progressions and templates are stored locally and (if enabled) backed up to iCloud and/or Dropbox.

1. Force-quit and relaunch the app. iCloud sync occasionally needs a foreground event to fetch.
2. Check your other devices — if the data is there, a sync will bring it back.
3. If you have Dropbox connected, your data is backed up there as individual JSON files in `/Apps/Skitter/`.

## The app crashes on launch

If a crash happens before the UI appears, the local data store may have been corrupted.

- Force-quit the app and relaunch. SwiftData's recovery path creates a fresh persistent store.
- If the problem persists, uninstall and reinstall. If you have iCloud sync enabled, your data will re-sync on first launch.

## How do I reset everything?

Delete the app and reinstall. All local data is wiped. If iCloud sync is enabled, iCloud data will still be there and resync on first launch. To truly start fresh, turn off iCloud sync first, delete the app, then reinstall.

## Feature requests and bugs

Email [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com) or file an issue on the app's [GitHub issues page](https://github.com/repsac/skitter-ios/issues). Include:

- What you expected to happen
- What actually happened
- Device model and iOS version (**iOS Settings → General → About**)
- Skitter version and build (**Settings → About → Version**)

Short, specific reports are much easier to act on than vague ones. Screenshots help a lot.
