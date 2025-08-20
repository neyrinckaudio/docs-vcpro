# FaderPort V2 / iOStation 24c

V-Control Pro supercharges the single fader FaderPort V2 / iOStation 24c for use with Pro Tools.

!!! warning "Set FaderPort Mode To Studio One Native Mode"
    It is VERY important the Faderport is in Studio One operation mode and NOT in HUI mode. This allows V-Control Pro to customize how FaderPort maps to Pro Tools. 

!!! warning "Disable FaderPort MIDI Input"
    In the Pro Tools MIDI Input Devices Window, disable the Faderport. It is used by V-control Pro and can cause conflict if enabled in Pro Tools as well.

!!! info "Control Features"
    Please see the FaderPort V2 / ioStation 24c feature charts online at [Feature Charts](./feature-charts.md/#faderport-v2--iostation24c).

### Setup

* Set FaderPort to Native Mode using the Select Control menu.
    * Power off the FaderPort 8/16
    * Hold the first and second "Select" buttons on the FaderPort 8/16
    * Power the FaderPort 8/16 back on
    * Once the unit has powered up and displays "Select Control Mode" across the top of the scribble strips you can release the Select buttons
    * Select Native Mode (Studio One)

* Add the device as a controller in the V-Control Pro Setups window as described in [Setting Up MIDI Controllers](./midi-controllers.md).

* Configure V-Control Pro to map the FaderPort V2 / iOStation 24c to 8, 16, 24, or 32 channels.
    * Open the V-Control Pro Setups window.
    * Click on the Faderport/ioStation 24c that is paired with Pro Tools in the Setups column.
    * Select 32 Channels in the Bank selection if using the AVID Control App or Standalone.
    * Select 24 Channels in the Bank selection if using RAVEN or a 24 fader surface.
    * Select 8/16 Channels in the Bank selection if using an 8 or 16 fader surface.

* Set up Pro Tools for 1, 2, 3, or 4 HUI banks as described in [Setting Up Pro Tools](./pro-tools.md). The number of HUI bank channels must match the number of channels configured in the previous steps.

#### Fast Focus and Refocus with FaderPort V2/iOStation 24c

With V-Control Pro, the FaderPort automatically focuses to any track you select. V-Control Pro can widen the bank up to thirty-two tracks for instant focus, and if it loses focus it immediately blinks the Channel button. Simply tap the blinking button to automatically ReFocus. Now you can select any track at any time for a focused FaderPort.
When selecting a track within the controlled bank range, the Faderport will Fast Focus to the selected track for control.
When selecting a track outside of the controlled banks, the Channel button will immediately blink on the Faderport. Press it to ReFocus to that track for control.
When a track is selected within the controlled banks, press the channel button to enable the wheel for navigation.



