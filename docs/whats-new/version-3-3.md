# What's New In Version 3.3

Version 3.3 adds D-Control Basic, so you can use an Avid D-Control console with Pro Tools. It lets you use more than one Command 8 with Pro Tools, and it makes V-Control Pro easier to start, set up, and troubleshoot.

!!! warning "macOS 12.0 Or Later Required"
    Version 3.3 requires macOS 12.0 (Monterey) or later. The installer will not install on earlier macOS versions.

## D-Control Basic

D-Control Basic gets you basic Pro Tools control from a D-Control console, including on Apple Silicon computers. It provides the same features V-Control Pro provides for D-Command with Pro Tools.

* Use a D-Control Main and up to two D-Control Fader Modules for up to 32 channels of control.
* Each Fader Module provides 16 channel strips. Choose `Bank 1-16` or `Bank 17-32` for each Fader Module.
* Channel strips provide faders, mute, solo, record, select, scribble strips, meters, and the bottom two encoder rows for pan, sends, inserts, and plug-in editing.
* The D-Control Main provides transport, scrub/shuttle, counter, automation modes, window buttons, bank and nudge navigation, zoom, global keys, save, undo, and redo.
* The Main Focus Strip provides a fader, select, solo, mute, record, name display, meters, and a pan/send encoder.
* Fader Module `Shift`, `Control`, `Option`, and `Command` keys act as Pro Tools keyboard modifiers.

!!! info "D-Control Basic Is Not Full Console Integration"
    V-Control Pro communicates with Pro Tools using the HUI protocol, which limits how much of a D-Control console can be used. Some controls and displays stay inactive. See [D-Control Basic](../d-control.md) for what to expect.

To get started, see [D-Control Basic](../d-control.md) for setup and the [Feature Charts](../feature-charts.md) for the complete list of controls.

## More Than One Command 8 With Pro Tools

Command 8 now has bank choices with Pro Tools: `Bank 1-8`, `Bank 9-16`, `Bank 17-24`, and `Bank 25-32`. Previously every Command 8 controlled Pro Tools tracks 1-8. See [Command 8](../command8.md) and [Multiple HUI Controllers With Pro Tools](../hui-device.md).

## Reliable Launch At Login

V-Control Pro could fail to launch, or start up unlicensed, when it was set to open automatically at login. It now waits for the iLok licensing service to be ready before checking your license.

!!! tip "Removed V-Control Pro From Login Items?"
    If you removed V-Control Pro from your Login Items to work around this problem, as described in [V-Control Pro Won't Launch](../troubleshooting.md#macos-troubleshooting), you can add it back after updating.

## User Guide Button

Each surface, DAW, and setup in the Setups window now has a `User Guide` button. It opens the guide in your default web browser.

* The `User Guide` button replaces the built-in `Setup Guide` tab, which could not display modern pages.
* Guide links go to the current online documentation. Setups saved with earlier versions are updated to the new links automatically.
* C24, Control 24, D-Command, and D-Control open their own guides.

## Offline Items In The Setups Window

Surfaces, DAWs, and setups that are not connected are marked `(offline)` in the Setups window, so you can see at a glance what is not connected.

## Easier Device Discovery

* Some D-Control Main units were shown as `Unknown` in `Add Ethernet Device` and were not found again after a restart. They are now recognized.
* `Add Ethernet Device` shows the type of unrecognized devices, for example `Unknown (0x1f)`, and discovery is written to the log file to help customer support diagnose them.

## Troubleshooting And Support

* `Open Troubleshooting Guide` now opens the [Troubleshooting Guide](../troubleshooting.md). Previously it opened the log file.
* A new `Show Log File` menu item on macOS and Windows reveals the log file so you can send it to customer support.
* The log file no longer grows without limit.

## Startup Notice

The notice that V-Control Pro runs in the menu bar now appears on every launch until you select `Don't show this again`.

## Release Notes

See the [Release Notes](../release-notes.md) for the complete list of changes in version 3.3.
