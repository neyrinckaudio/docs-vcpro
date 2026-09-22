# What's New In Version 3.2

Version 3.2 is all about FaderPort 8/16. It brings a new supercharged FaderPort 8/16 for Pro Tools 2023 and later, with a Track Browser, plug-in editing, sends, and memory location control right from the surface. Version 3.2.0.25 also adds plug-in editing on more surfaces and support for more DAWs.

!!! info "All Surfaces Supported In 3.2.0.25 And Later"
    Version 3.2 pre-release builds (3.2.0.16 and earlier) are for FaderPort 8/16 only. They are **incompatible** with all other surfaces. Version 3.2.0.25 and later support all surfaces.

## FaderPort 8/16 For Pro Tools 2023 And Later

Pro Tools 2023 removed the M-Audio Keyboard protocol that V-Control Pro used with FaderPort 8/16 in earlier Pro Tools versions. Version 3.2 rebuilds FaderPort 8/16 support from the ground up to bring those features back and add new ones.

For setup and complete instructions, see [FaderPort 8/16](../faderport-8-16.md#faderport-beta).

### Track Browser

The Track Browser lets you bank to any track in your Pro Tools session in seconds instead of banking through dozens of channels to find it.

* In Track mode, press `Track` to change to Track Browser mode. The `Track` button blinks.
* The track displays show lists of tracks, organized by banks. The `Select` buttons show the Pro Tools track colors.
* Use the navigation encoder at the right to scroll through banks of tracks.
* Press a `Select` button to automatically bank to and select that track.

### Track Colors

The `Select` buttons light in the same colors as the corresponding Pro Tools tracks, so you can find tracks at a glance.

### Plug-In Editing

Edit the parameters of the plug-in on the selected insert directly from the FaderPort in `Plug-in` mode.

* Parameter names and values appear on the displays, along with the plug-in name.
* Faders control continuous parameters.
* `Select` buttons control on/off parameters and light in color.
* Page through the plug-in's parameters.
* FaderPort 16 uses the right eight strips for plug-in editing. FaderPort 8 uses all eight strips.

### Plug-In Navigation

* Press `Select` on an insert to focus its track. Press `Select` again to move to the next insert.
* Show and hide the plug-in window from the surface.
* `Bypass` and `Compare` the focused plug-in, or use `Bypass All` to bypass all inserts.

### Sends Mode

* The displays show the send letter and destination, for example `A: Verb`.
* Pre-fader sends are shown in inverted text.
* Press `Shift` + `Select` to toggle a send between pre and post.
* Turn the wheel to step to the next or previous send. The last-used send is remembered.

### Marker Mode

Browse and select Pro Tools memory locations by name from a list on the FaderPort.

* Press the `Marker` button. The right-most display lists all memory locations. Long names are shortened to be readable.
* Use the right-side encoder to scroll through the list.
* Press the right-side encoder to select the location.

!!! tip "Create Show/Hide Locations"
    Pro Tools memory locations can change track visibility. Create locations that show groups of tracks, then select them from Marker Mode to quickly see just the tracks you need.

### Hot Locations

The `Audio`, `VI`, `Bus`, `VCA`, `All`, and `Master` buttons select memory locations with the same name in capital letters, such as *AUDIO* or *MASTER*. This lets you build custom workflows, such as instantly showing just your audio tracks.

* Create a memory location named to match each button, all capitalized.
* Press `Marker` and select the memory location you want as your *HOME* location. Any location can be used as *HOME*.
* Press a hot location button to activate it.
* Press the active hot location button again to return to *HOME*.

### Mix / Window Button

The section button switches between the Pro Tools Mix and Edit windows.

## Also In Version 3.2

### Plug-In Editing On More Surfaces

* D-Command and Command 8 now support plug-in editing with Pro Tools.
* When editing plug-ins with Pro Tools, C24, Control 24, Command 8, ProControl, and D-Command switch encoders to Fixed mode automatically.
* Command 8 adds Flip mode for sends with Pro Tools.

### More DAWs

* [Fender Studio](../studio-one.md) on macOS and Windows.
* ProControl with [DaVinci Resolve](../davinci-resolve.md).
* [Sonar](../sonar.md) and [Reason](../reason.md) with ProControl, ProControl Fader Pack, Control 24, Command 8, and C24.
* Premiere Pro 2023, 2024, and 2025 on macOS.

### Logic Pro Protocol Setting

A new `Logic Pro Protocol` preference replaces the IPv6 checkbox. It helps when Logic Pro communicates with a surface in one direction only. See [Logic Pro Protocol Settings](../logic-pro.md#ipv6-setting).

### Easier Windows Installation

The Windows installer no longer requires a restart, installs BOME MIDI correctly, and offers to open the online user guide when it finishes.

## Release Notes

See the [Release Notes](../release-notes.md) for the complete list of changes in each 3.2 build.
