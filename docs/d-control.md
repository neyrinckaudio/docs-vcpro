# Avid D-Control Basic

V-Control Pro supports D-Control consoles with a feature set called D-Control Basic. It provides the same features V-Control Pro provides for [D-Command](./d-command.md) with Pro Tools.

The goal is a practical one. If you are running Pro Tools on an Apple Silicon computer, D-Control Basic gets you basic Pro Tools control from the console instead of a dark desk.

!!! info "Pro Tools Only"
    At this time, D-Control Basic is for Pro Tools. Other DAWs and media applications are not supported with a D-Control console.

!!! warning "D-Control Basic Is Not Full Console Integration"
    The name says so on purpose. V-Control Pro communicates using the HUI protocol, and HUI sets the ceiling on how much of a console this size can be reached. As a result, a large part of a D-Control frame stays inactive.

## What To Expect

* The available features are the same ones V-Control Pro provides for a D-Command console with Pro Tools.
* Channel strip control, transport, navigation, automation modes, sends, plug-in editing, and [V-Window](./v-window.md) work as they do on D-Command. See the feature chart for the complete list.
* Only two rows of encoders are active. They are the bottom two rows of a D-Control channel strip, and they provide what the two rows of a D-Command channel strip provide. In the feature chart they are the `Upper Edit Row` and the `Lower Edit Row`. The top four encoder rows are inactive.
* Controls that the HUI protocol does not reach do not respond, and their displays and indicators stay dark. This is a limit of the protocol, not a setup problem.

!!! info "Control Features"
    Please see the D-Control Basic feature chart online at [Feature Charts – D-Control Basic](./feature-charts.md/#d-control-basic).

V-Control Pro supports D-Control Main and Fader Module devices. Up to one main device and two fader module devices can be used for 32 channels of control. First, you must add the D-Control devices as controllers in the V-Control Pro Setups window as described in [Setting Up Ethernet Controllers](./ethernet-controllers.md).

### Setup

#### Pro Tools
Set up Pro Tools for 2 or 4 HUI banks as described in [Setting Up Pro Tools](./pro-tools.md). A D-Control Fader Module device counts as two 8-channel banks.
