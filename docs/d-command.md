# Avid D-Command

V-Control Pro supports D-Command Main and Fader Module devices. A Main and one Fader Module can be used for 24 channels of control. With Pro Tools, up to three devices (a Main and two Fader Modules) can be used for 32 channels of control. First, you must add the D-Command devices as controllers in the V-Control Pro Setups window as described in [Setting Up Ethernet Controllers](./ethernet-controllers.md).

!!! info "Control Features"
    Please see the D-Command feature charts online at [Feature Charts – D-Command](./feature-charts.md/#d-command).


### Setup

#### Pro Tools
Set up Pro Tools for 1, 3, or 4 HUI banks as described in [Setting Up Pro Tools](./pro-tools.md). A D-Command Main device counts as one 8-channel bank. A Fader module counts as two 8-channel banks.

With Pro Tools, you can use up to two Fader Modules with the D-Command Main device. The maximum is 32 channels of control (4 HUI banks), so with two Fader Modules the last eight channel strips on the second Fader Module are inactive.

| D-Command Configuration | Channel Strips | HUI Banks | Active Channels |
|---|---|---|---|
| Main | 8 | 1 | 8 |
| Main + 1 Fader Module | 24 | 3 | 24 |
| Main + 2 Fader Modules | 40 | 4 | 32 (last 8 strips inactive) |

#### Logic Pro X
Set up Logic Pro X for D-Command as described in [Setting Up Logic Pro](./logic-pro.md).

#### Cubase/Nuendo
Set up Cubase / Nuendo for D-Command as described in [Setting Up Cubase/Nuendo](./cubase-nuendo.md).

#### Mackie Control DAWs

Set up the DAW for D-Command using 1 or 3 Mackie Control banks as described in [Setting Up Mackie Control](./mackie-control.md). Each eight strips counts as one 8-channel bank.

* [Adobe Audition](./adobe-audition.md)
* [Ableton Live](./ableton-live.md)
* [Digital Performer](./digital-performer.md)
* [FMOD](./fmod-studio.md)
* [FL Studio](./fl-studio.md)
* [LUNA](./luna.md)
* [MIO Console](./mio-console.md)
* [MixBus](./mixbus.md)
* [Premiere Pro](./premiere-pro.md)
* [Reaper](./reaper.md)
* [Reason](./reason.md)
* [Sonar](./sonar.md)
* [Studio One / Fender Studio](./studio-one.md)
* [WWise](./wwise.md)