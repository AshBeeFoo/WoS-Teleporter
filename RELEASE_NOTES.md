## WoS Quick Teleport 2.5.0

- Added adaptive button detection: calibrated positions remain the fast path, followed by a full-emulator search after 120 ms.
- The app now clicks the detected button itself and automatically learns updated upper- and lower-panel positions.
- An already-open destination panel is reused instead of tapping the map again and closing it.
- Added an adjustable World map tap-height slider and a one-tap position test.
- Added individual Teleport, Advanced, and Confirm point recording.
- Added clearer readiness checks, last success/failure times, **Try again**, and contextual **Send diagnostics** actions.
- Failed actions can save a cropped, redacted emulator screenshot; users choose whether to attach it to a manual report.
- Added Stable and Preview update channels and a proper Windows installer release asset.

### Included from 2.4.4

- The fixed World map target now sits slightly below the screen center.
- This encourages the game to open the Teleport panel above the selected tile, keeping its buttons in a consistent location.
- Calibration and live teleports share the exact same map target to prevent alignment differences.

### Included from 2.4.3

- Teleports no longer open a separate success or failure pop-up.
- The Status tab now shows whether the teleport succeeded or failed, including the failure reason.
- Teleport outcomes automatically return the app to the Status tab so the result is immediately visible.

### Included from 2.4.2

- Replaced the automated calibration test with a guided **Recalibrate clicks** action.
- Calibration performs exactly one automatic map tap and does not replay any saved button clicks.
- After the map tap, the user clicks Teleport, Advanced Teleporter, and Confirm so each position is captured directly.

### Included from 2.4.1

- The app now taps one fixed point on the emulator World map every time, removing destination calibration drift.
- Calibration records only the three response buttons; the destination point is fixed by the app.
- The calibration editor shows the destination marker as fixed and only allows response buttons to move.
- Check for updates is now always visible on Advanced Settings instead of being hidden in expert options.

### Included from 2.4

- Redesigned the interface with softer colors, cleaner cards, and simpler primary actions.
- Added a first-run setup guide and clear emulator, World map, calibration, and item checks.
- Added draggable calibration markers over a live emulator screenshot.
- Added automatic calibration profiles for different emulator resolutions.
- Added a system-wide Ctrl+Shift+Esc emergency stop shortcut.
- Added manual and automatic sanitized Discord diagnostic reports.
- Discord webhook URLs are stored in Windows Credential Manager, not the settings file.
- Added update health checks, automatic rollback, and manual Restore previous version.
- Added optional executable signing in the release workflow when certificate secrets exist.
- Kept the permanent Ko-fi button, fast click path, dark mode, and custom app icon.

Discord diagnostics require a channel webhook configured under Advanced Settings →
Show expert options. Reports exclude the webhook URL and account secrets.
