## Version 3.3

### [3.3.0.15] - Upcoming
Version 3.3.0.15 is the first public release of version 3.3. It includes D-Control Basic and all the changes from version 3.2.

#### Added
- Added a `User Guide` button to the details for each surface, DAW, and setup. It opens the guide in your default web browser, replacing the built-in `Setup Guide` tab, which could not display modern pages.
- Added a `Show Log File` menu item on macOS and Windows to reveal the log file for customer support.
- The Setups window now marks surfaces, DAWs, and setups that are offline with `(offline)`.
- FaderPort V2 with Pro Tools: holding `Rewind` or `Fast Forward` now rewinds or fast forwards until you release the button.
#### Changed
- V-Control Pro now requires macOS 12.0 (Monterey) or later. The installer will not install on earlier macOS versions.
- Help and setup guide links now open the current online documentation. Setups saved with earlier versions are updated to the new links.
- The startup notice that V-Control Pro runs in the menu bar now appears on every launch until you select `Don't show this again`.
- The log file no longer grows without limit.
#### Fixed
- Fixed an issue where V-Control Pro could fail to launch, or start up unlicensed, when set to open automatically at login. It now waits for the iLok licensing service to be ready before checking your license.
- C24, Control 24, D-Command, and D-Control help now open their own guides.
- FaderPort 8 and FaderPort 16 with Pro Tools: holding `Rewind` or `Fast-Forward` did not rewind or fast-forward.
- Includes all fixes from version 3.2.1.18.

### [3.3.0.14] - 2026-09-08 (Beta)
#### Added
- Added [D-Control Basic](./d-control.md) for Pro Tools. D-Control Main and up to two D-Control Fader Modules can be added as Ethernet devices for up to 32 channels of control.
    - Each Fader Module provides 16 channel strips. Choose `Bank 1-16` or `Bank 17-32` for each Fader Module.
    - Channel strips provide faders, mute, solo, record, select, scribble strips, meters, and the bottom two encoder rows for pan, sends, inserts, and plug-in editing.
    - The D-Control Main provides transport, scrub/shuttle, counter, automation modes, window buttons, bank/nudge navigation, zoom, global keys, save, undo, and redo.
    - The Main Focus Strip provides a fader, select, solo, mute, record, name display, meters, and a pan/send encoder.
    - Fader Module `Shift`, `Control`, `Option`, and `Command` keys act as Pro Tools keyboard modifiers.
    - See the [D-Control Basic feature chart](./feature-charts.md) for the complete list.
- Added bank choices for Command 8 with Pro Tools: `Bank 1-8`, `Bank 9-16`, `Bank 17-24`, and `Bank 25-32`. Previously every bank controlled Pro Tools tracks 1-8.
- `Add Ethernet Device` shows the type of unrecognized devices, for example `Unknown (0x1f)`, and discovery packets are written to the log file to help diagnose them.
#### Changed
- Help and setup guide links now open the current online documentation. `Open Troubleshooting Guide` opens the troubleshooting guide, and a new `Show Log File` menu item reveals the log file.
#### Fixed
- Some D-Control Main units were shown as `Unknown` in `Add Ethernet Device` and were not found again after a restart.
