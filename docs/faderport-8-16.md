# FaderPort 8/16

V-Control Pro supercharges the FaderPort 8/16 for use with Pro Tools.

!!! info "Important Pro Tools Version Information"
    FaderPort 8/16 support has changed for Pro Tool 2023 and later. For Pro Tools 2022 and earlier, the M-Audio Keyboard protocol was used in Pro Tools. But Avid removed M-Audio Keyboard protocol in Pro Tools 2023. You must carefully configure V-Control Pro and Pro Tools depending on what version of Pro Tools you are using. 

!!! warning "Set FaderPort Mode To Studio One Mode"
    It is VERY important the FaderPort 8 / 16 is in Studio One Operation mode and NOT in HUI mode. This allows V-Control Pro to customize how FaderPort 8 / 16 maps to Pro Tools.

!!! warning "Disable FaderPort MIDI Input"
    In the Pro Tools MIDI Input Devices Window, disable the FaderPort. It is used by V-control Pro and can cause conflict if enabled in Pro Tools as well.

!!! info "Control Features For Pro Tools 2022 And Earlier"
    Please see the FaderPort 8/16 feature charts online at [Feature Charts](./feature-charts.md/#faderport-8-16).

!!! info "Control Features For Pro Tools 2023 And Later"
    Please see the latest info for the [FaderPort 8/16 Beta](#faderport-beta).


### Setup

#### FaderPort 8
* Add the device as a controller in the V-Control Pro Setups window as described in [Setting Up MIDI Controllers](./midi-controllers.md).
* Set Up Pro Tools MIDI Peripherals
    * Pro Tools 2022 And Earlier
        * Set up Pro Tools for 1 M-Audio Keyboard bank as described in [Setting Up Pro Tools](./pro-tools.md).
    * Pro Tools 2023 And Later
        * Set up Pro Tools for 1 HUI bank as described in [Setting Up Pro Tools](./pro-tools.md).


#### FaderPort 16

* Add the device as a controller in the V-Control Pro Setups window as described in [Setting Up MIDI Controllers](./midi-controllers.md).
* Set Up Pro Tools MIDI Peripherals
    * Pro Tools 2022 And Earlier
        * Set up Pro Tools for 1 M-Audio Keyboard bank and 1 HUI bank as described in [Setting Up Pro Tools](./pro-tools.md).
    * Pro Tools 2023 And Later
        * Set up Pro Tools for 2 HUI banks as described in [Setting Up Pro Tools](./pro-tools.md).

<a id="faderport-beta"></a>
#### Version 3.2 For FaderPort 8/16

Pro Tools removed the M-Audio Keyboard Protocol which was previously required for FaderPort 8/16 to be supercharged by V-Control Pro for Pro Tools 2022 and earlier. Version 3.2 features a new supercharged implementation for FaderPort 8/16 with Pro Tools 2023 and later.

##### Track Browser

The new Track Browser makes it fast and easy to bank to any track in your Pro Tools session. No more hunting and pecking. Patent pending.

Tired of banking through dozens of channels to find that one vocal track? The Track Browser puts your entire Pro Tools session at your fingertips. Instead of endless button pressing to hunt down tracks, you get a smart overview that lets you jump directly to any track in seconds.

Here's how simple it is: Press the Track button twice to enter Track Browser mode, and suddenly your control surface becomes a session navigator. Your track displays transform into organized lists showing all your tracks by banks, with Select buttons glowing in their actual Pro Tools colors. Just spin the navigation knob to scroll through your session, spot the track you need by its color, and press its Select button—boom, you're there instantly.

* Start in Track Mode.
* Press Track button to change to Track Browser mode (Track button will blink)
* Now the track displays will show lists of tracks, organized by banks.
* Use the navigation encoder at the right to scroll through banks of tracks for any number of tracks. Note that the Select buttons show the track colors.
* Press a Select button to automatically bank and select that track.

##### Track Color

The Select buttons are set to use the same color as the corresponding Pro Tools tracks

##### Mixer Modes

* Track Mode
    * Fader, Solo, Mute, Select
    * ARM - Press ARM to use Select buttons to record enable/disable tracks
    * Adjust Pan of the selected track with the upper left encoder. Push down to switch between Pan L and Pan R modes.
    * Use Shift + Track to enable/disable timecode display.
* Pan Mode
    * Use the faders to edit the pan. Use the Pan button to toggle between pan left/right. Note that channels will display Pan L / Pan R if they are stereo, mono channels will display Pan only, and non-pannable channels will not display anything.
* Sends Mode
* Edit Plugins Mode

##### Memory Locations

Now you can access all locations by name from a list displayed on FaderPort. I encourage you to create Show/Hide locations that let you quickly see groups of tracks.

* Press the Marker button. Note that the right-most display lists all markers.
* Use the right-side knob/encoder to scroll through the list.
* Press the right-side knob/encoder to select the location.

##### Hot Locations

The `Audio`, `VI`, `Bus`, `VCA`, `All`, and `Master` buttons are programmed to select certain memory locations. This lets you implement custom workflows. Pro Tools memory locations can be configured to change track visibility, for example, so you can instantly show and hide tracks.

* You will need to have at least one memory location that you want to be your *HOME* location to return to when exiting a hot location. Any location can be used as *HOME*.
* Create a memory location that is named to match the button, but all capitalized. *AUDIO*, for example, that shows just audio tracks.
* Press the `Markers` button to enter the Location Browser and select your *HOME* location.
* Now press any hot location button to activate it.
* Press the active hot location to return to the *HOME* location.


##### Configure Native Mode

The FaderPort 8/16 device must be configured for “native” mode. To set the mode, press and hold the Select buttons of channel 1 and 2, and then power on the device.

##### Setup A Single Device

You must configure Pro Tools MIDI Peripherals for one (FaderPort 8) or two (FaderPort 16) HUI devices.

* For FaderPort 8 and 16 Bank 1
    * Type:HUI
    * Receive From: V-Control
    * Send To: V-Control

* For FaderPort 16 bank 2
    * Type:HUI
    * Receive From: V-Control XT2
    * Send To: V-Control XT2

##### Setup Multiple Devices

You can configure Pro Tools MIDI Peripherals for up to 32 channels (four HUI banks of 8).

When setting up multiple FaderPorts, add up the number of banks: one per FaderPort 8 and two per FaderPort 16.

Then configure MIDI Peripiherals:

* Bank 1
    * Type:HUI
    * Receive From: V-Control
    * Send To: V-Control

* Bank 2
    * Type:HUI
    * Receive From: V-Control XT2
    * Send To: V-Control XT2

* Bank 3
    * Type:HUI
    * Receive From: V-Control XT2
    * Send To: V-Control XT2

* Bank 4
    * Type:HUI
    * Receive From: V-Control XT3
    * Send To: V-Control XT3

Then you must configure the layout in V-Control Pro Setups window.

* Configure V-Control Pro Setups
    * Open V-Control Pro Setups window
    * Select each FaderPort surface that is set up with Pro Tools.
    * Click the Bank dropdown menu.
    * Select the bank layout for teh device.
