# Setting Up Pro Tools

!!! warning "Important HUI Metering Information"
    The HUI protocol provides for stereo track metering. It does not provide for output metering. Surfaces that have output meters will not display any output metering when connected to Pro Tools.

    Pro Tools will not provide track metering if Eucon is enabled. Disable Eucon for track metering.

V-Control Pro uses the HUI protocol with Pro Tools Studio/Ultimate to provide for 8, 16, 24, or 32 channels of control. The Pro Tools MIDI Peripherals window must be configured to use V-Control Pro's virtual MIDI ports for Pro Tools to communicate with V-Control Pro.

!!! warning "Do Not Enable Ethernet Legacy Controllers In Pro Tools"

!!! warning "Enable MIDI Ports In Pro Tools"
    V-Control Pro provides virtual MIDI ports for Pro Tools to use. These ports must be enabled for MIDI input.

!!! warning "FaderPort 8/16 With Pro Tools 2022 And Earlier"
    FaderPort 8/16 setup depends upon which version of Pro Tools you are using. Please see the special setup information for FaderPort 8/16 with Pro Tools 2022 and earlier.

## Enable V-Control Pro Virtual MIDI Ports

* In Pro Tools, select the menu Setup / MIDI / MIDI Input Devices
* Enable the `V-Control, V-Control XT-2, V-Control XT-3, V-Control XT-4` and `V-Pan` ports.
* Do not enable the `V-Control MIDI Mode` port.

## Setting the MIDI Peripherals

V-Control Pro must be set up in the Pro Tools peripherals window. Depending on how many banks are being used, the configuration will vary. 

* In the Pro Tools top menu bar select: Setup / Peripherals. Select the MIDI Controllers tab

### 8 Channel Surfaces

* D-Command Main
* ProControl Main
* FaderPort 8 (Pro Tools 2023+)
* Command 8
* Digidesign 003
* V-Console (set for 8 channels)
* Legacy V-Control Pro iPad App
![8 Channel Surfaces](./images/ptmidi1.png "8 Channel Surfaces")

### 16 Channel Surfaces

* ProControl Main & ProControl Fader Pack
* FaderPort 16 (Pro Tools 2023+)
* V-Console (set for 16 channels)
![16 Channel Surfaces](./images/ptmidi2.png "16 Channel Surfaces")

### 24 Channel Surfaces

* D-Command Main & D-Command Fader Module
* Control 24
* C24
* ProControl Main & Two ProControl Fader Packs
* RAVEN 24
![24 Channel Surfaces](./images/ptmidi3.png "24 Channel Surfaces")

### 32 Channel Surfaces
* ProControl Main & Three ProControl Fader Packs
* FaderPort V2 / ioStation 24c
* RAVEN 32
![32 Channel Surfaces](./images/ptmidi4.png "32 Channel Surfaces")

### FaderPort 8 With Pro Tools 2022 And Earlier

![FaderPort 8](./images/ptfp8.jpg "aderPort 8")

### FaderPort 16 With Pro Tools 2022 And Earlier

![FaderPort 16](./images/ptfp16.jpg "aderPort 16")

