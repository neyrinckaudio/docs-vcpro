## Version 3.3

Version 3.3 is the first public release of version 3.3. It includes D-Control Basic and all the changes from version 3.2.

#### Added
- Added [D-Control Basic](./d-control.md) for Pro Tools. A D-Control Main and up to two D-Control Fader Modules provide up to 32 channels of control. See the 3.3.0.14 notes below for details.
- Added automatic updates. V-Control Pro checks for a new version once a day and can install it for you. A new `Check for Updates...` menu item checks immediately.
- Added a `What's New` window that describes what changed in the version you just installed, with a `Read More` button that opens the online release notes. It opens once after an update, and any time from the `What's New...` menu item.
- Added `Help / Create Customer Support Ticket...` on macOS and Windows. It sends a system report to Neyrinck and opens a support request in your web browser, filled in with your computer details and with the report attached. Add your name, email, and a description, then send it. If you do not send the request, the report is deleted after 7 days.
- Added `Help / Create System Report...` on macOS and Windows. It saves the same report to your Desktop to attach to a support ticket yourself. The report contains your V-Control Pro and computer details, license status, setups, Pro Tools MIDI settings, and the last two days of the log. It replaces the `Show Log File` item.
- Added a `License` menu with `Activate License...` and `Deactivate License...`, and Activate and Deactivate buttons in the About box. Sign in to iLok in your browser, then activate a license to this computer or to an iLok key, or deactivate it to move it to another computer.
- Added a `Help` menu with `Open User Guide`, `Open Troubleshooting Guide`, `Create Customer Support Ticket...`, and `Create System Report...`.
- Added a `User Guide` button to the details for each surface, DAW, and setup. It opens the guide in your default web browser, replacing the built-in `Setup Guide` tab, which could not display modern pages. V-Window and V-Control MIDI Mode now have a `User Guide` button as well.
- The Setups window now marks surfaces, DAWs, and setups that are offline with `(offline)`.
- The Windows installer now offers to launch V-Control Pro when it finishes.

#### Changed
- V-Control Pro has a new look. The Setups window, Preferences, About box, and dialogs use a new design with updated colors and controls, roomier detail pages, and the `User Guide` button at the top right.
- The V-Control Pro menu is reordered: Setups, Preferences, About, License, Help, Check for Updates, What's New.
- V-Control Pro now requires macOS 12.0 (Monterey) or later. The installer will not install on earlier macOS versions.
- Help and setup guide links now open the current online documentation. Setups saved with earlier versions are updated to the new links.
- The startup notice that V-Control Pro runs in the menu bar now appears on every launch until you select `Don't show this again`.

#### Fixed
- Fixed an issue where V-Control Pro could fail to launch, or start up unlicensed, when set to open automatically at login.
- FaderPort 8, FaderPort 16, FaderPort V2, and ioStation 24c with Pro Tools: holding `Rewind` or `Fast Forward` did not rewind or fast forward. Pressing `Rewind` and `Fast Forward` together still returns to zero.
- ProControl Fader Pack with Cubase and Nuendo: the fader pack now releases properly to MIDI Mode. Previously controls drove both MIDI Mode and the Cubase mixer, and faders and displays were left stale when leaving MIDI Mode.
- macOS: V-Control Pro could quit unexpectedly when an Ethernet controller's network adapter was removed, such as unplugging a USB or Thunderbolt Ethernet adapter. This affects ProControl, D-Command, D-Control, and C24.
- macOS and Windows: installers could leave files locked by a V-Control Pro that did not quit. They now wait for it to exit.
- Windows: fixed a crash when quitting V-Control Pro.
- C24, Control 24, D-Command, and D-Control help now open their own guides, and the V-Control MIDI Mode guide link works for setups saved with earlier versions.
