## Version 3.2

### [3.2.2] - Upcoming
#### Added
- Added a `User Guide` button to the details for each surface, DAW, and setup. It opens the guide in your default web browser, replacing the built-in `Setup Guide` tab, which could not display modern pages.
- Added a `Show Log File` menu item on macOS and Windows to reveal the log file for customer support.
- The Setups window now marks surfaces, DAWs, and setups that are offline with `(offline)`.
#### Changed
- V-Control Pro now requires macOS 12.0 (Monterey) or later. The installer will not install on earlier macOS versions.
- Help and setup guide links now open the current online documentation. Setups saved with earlier versions are updated to the new links.
- The startup notice that V-Control Pro runs in the menu bar now appears on every launch until you select `Don't show this again`.
- The log file no longer grows without limit.
#### Fixed
- Fixed an issue where V-Control Pro could fail to launch, or start up unlicensed, when set to open automatically at login. It now waits for the iLok licensing service to be ready before checking your license.
- `Open Troubleshooting Guide` opened the log file instead of the troubleshooting guide.
- C24, Control 24, and D-Command help opened the ProControl guide instead of their own guides.

### [3.2.1.18] - 2026-09-18
Version 3.2.1.18 supports all surfaces. Earlier 3.2 pre-releases were for FaderPort 8/16 only.

#### Added
**FaderPort 8/16 with Pro Tools**

- Added plug-in parameter editing in `Plug-in` mode. Parameter names and values appear on the displays, faders control continuous parameters, and `Select` buttons control on/off parameters. FaderPort 16 uses the right eight strips. FaderPort 8 uses all eight strips.
- `Sends` mode shows the send letter and destination (for example `A: Verb`) and shows pre-fader sends in inverted text. `Shift` + `Select` toggles a send between pre and post. The wheel steps to the next or previous send, and the last-used send is remembered.
- `Zoom` is now a navigation mode. Pro Tools HUI zoom is enabled automatically.
- Added bank offset choices so more than one FaderPort can be used at the same time.
- `Shift` + `Marker` opens and closes the Pro Tools Memory Locations window.
- `Shift` + `Touch` / `Write` / `Read` performs Write to Start / Write to All / Write to End.
- `Shift` + `Solo` resets the channel's fader, or its pan in `Pan` mode. `Shift` + encoder push resets the selected track's pan.
- Hold `Shift` while touching a fader for fine fader control.

**Other Surfaces and DAWs**

- Added plug-in editing for D-Command and Command 8 with Pro Tools. Plug-in editing on C24, Control 24, Command 8, ProControl, and D-Command switches encoders to Fixed mode automatically.
- Added `Bank 25-32` for D-Command Fader Modules with Pro Tools.
- Added Flip mode for sends on Command 8 with Pro Tools.
- Added ProControl support for DaVinci Resolve.
- Added support for Fender Studio on macOS and Windows.
- Added Sonar and Reason support for ProControl, ProControl Fader Pack, Control 24, Command 8, and C24.
- Added support for Premiere Pro 2023, 2024, and 2025 and Mixbus 11, 12, and 13 on macOS.
- Added a `Logic Pro Protocol` preference, replacing the IPv6 checkbox. Choose `Default` for macOS Tahoe and later, or `IPv4 Localhost` or `IPv6` for macOS Sequoia and earlier.
- Added `Open Troubleshooting Guide` to the menu on macOS and Windows.

#### Changed
- FaderPort 8/16 mode buttons were reworked for more consistent switching between modes. Navigation now defaults to `Bank`.
- The FaderPort 8/16 `Track Browser` requires Pro Tools 2024 or later. It skips hidden tracks and tracks in closed folders, and banks to the selected track without fader jumps.
- Pro Tools scripting is updated for Pro Tools 2025.10 and is disabled for Pro Tools 2022 and earlier.
- C24 fader taper is recalibrated for Pro Tools and Logic Pro.
- The Windows installer no longer requires a restart, requests administrator privileges so BOME MIDI installs correctly, and offers to open the online user guide when it finishes. Uninstalling removes all V-Control Pro BOME MIDI ports.

#### Fixed
- FaderPort V2 / ioStation 24c V-Window works again.
- The legacy V-Control Pro 1 iPad app works again without a license.
- Raven and the legacy V-Control Pro 1 iPad app showed blank track names.
- FaderPort 8/16: fixed pan display for Routing Folder tracks, mode switching on FaderPort 8, restoring the previous mode after an alert, and the track browser when banked before the first track.
- D-Command MIDI Mode was always active.
- Command 8 with Pro Tools: fixed Bank, Nudge, and Zoom, and improved V-Window mode.
- C24 with Pro Tools: fixed the `Clear Clip` button.
- Logic Pro with C24, Control 24, Command 8, and D-Command: fixed plug-in, send, and channel edit displays and bank mode selection.
- Digital Performer: C24 can switch to MIDI Mode, and Control 24 no longer gets stuck in MIDI Mode.
- Fixed one-way control when used with other HUI devices.
- Pro Tools on Windows: modifier buttons now match Pro Tools, and fixed Pro Tools version detection and plug-in control.
- Windows: user account names with non-ASCII characters work, and the About box shows the correct version.
- Fixed crashes when closing or switching setups and plug-in editors.

## Version 3.2 Pre-release for FaderPort 8/16
!!! warning "Version 3.2 Pre-release Is For FaderPort 8/16 Only"
    V-Control Pro 3.2 pre-release builds 3.2.0.16 and earlier are **incompatible** with all other surfaces.

### [3.2.0.16] - 2025-09-08
#### Changed
- `Hot Locations` restore to new `home` memory location.
- `Hot Locations home` is set by selecting a memory location in `Marker Mode`
#### Added
- Added `Master` button to `Hot Locations.` It will select a memory location named MASTER.
#### Fixed
- Marker Mode - Shorten long names to be readable.
- Fixed incorrect selection issue.
- Fix `Bypass All Inserts`

### [3.2.0.12]
#### Added
- Added `Plug-In Navigation` - `Select` focuses track. Additional `Select` changes to next insert.
- Added show/hide plug-in window
- Added plug-in `Bypass`
- Added plug-in `Compare`
- Added plug-in `Bypass All`
- Added `Marker Mode` to browse and select memory locations
- Added `Hot Locations` - Audio, VI, Bus, VCA, and All buttons will select memory locations with the same name with all letter capitalized
- Added `Mix / Window Button` (Section Button)
### [3.2.0.5]
#### Added
- Added `Track Browser` to browse and auto-bank to selected track
- Added bright track colors to Select buttons
