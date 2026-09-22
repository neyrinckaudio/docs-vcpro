## Version 3.3 Beta
!!! warning "Version 3.3 Is A Beta"
    V-Control Pro 3.3 is a beta release for testing D-Control Basic. It does not yet include the fixes in 3.2.2, including the launch-at-login fix. If you do not use a D-Control console, use version 3.2.

### [3.3.0.14] - 2026-09-08
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
