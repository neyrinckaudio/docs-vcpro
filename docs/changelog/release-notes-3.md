## Version 3.0

### [3.0.24]

Fender Studio

* Added support for Fender Studio.

Windows

* Fixed BOME Midi installer to provide uninstaller.
* Fixed BOME Midi to create virtual ports with administrator privileges.
* Remapped surface modifier buttons to match Pro Tools incorrect mapping.

D-Command

* Fixed Midi Mode to not always be active.
* Fixed scribble display errors for track names starting with “Bus”

Command 8 With Pro Tools

* Added PlugIn Editing
* Added Flip Mode For Sends

HUI Protocol Device

* Fixed one-way control with HUI devices used in parallel.

### [3.0.23]

C24

* Improved PlugIn editing with Pro Tools
* Fixed Logic Pro displays for plugin, sends, and channel editing

Windows

* Fixed to be compatible with user account names using non-ascii characters.

### [3.0.22]

Logic Pro

* Change Logic Pro for more reliable control.

Digital Performer

* Fix Control 24 to not be stuck in MIDI Mode
* Fix C24 to be able to switch to MIDI Mode

Pro Control

* Change Midi Mode switch to Shift + Monø

Windows

* installer security improved
* Fixed uninstaller to remove MIDI ports

### [3.0.21]

Reason

* Fixed mapping to various surfaces

C24

* Fixed ‘Clear Clip’ button for Pro Tools


### [3.0.20]
#### Fixed
* Command 8 With Pro Tools
	* Fixed Bank, Nudge, Zoom mode 

### [3.0.19]
#### Added
- Sonar mapped to legacy hardware surfaces
- Added Troubleshooting Guide menu option

### [3.0.18]
- ProControl
* Fixed the `mon/phase` button to not switch to MIDI Mode with Pro Tools  
* Function 1 button now switches to MIDI Mode

### [3.0.17]

ProControl

* Basic control for DaVinci Resolve

### [3.0.16]

Logic Pro

* Added a preference to use IPv6 protocol with Logic Pro. This preference helps users experiencing one-way control with Logic Pro. For more information see https://neyrinck.com/help/logic-pro-control-operates-one-way/

### [3.0.15]

C24

* Improved fader calibration for Logic and Pro Tools..

### [3.0.14]

ProControl Main

* Fixed fader 8 operation with Cubase/Nuendo when device was assigned to bank 2, 3, or 4\.

### [3.0.13]

PreSonus FaderPort V2 / ioStation 24c

* Improved Link Mode so that when mouse moves back to its starting point, it does not affect the control being adjusted.

### [3.0.12]

RME TotalMix \- fixed connection  
MIDI Mode Improvements  
	Added meter mappings for D-Command Main  
Added meter mappings for ProControl Main

### [3.0.11]

MIDI Mode Fixes  
	Missing scribbles on D-Command Main  
	ProControl Fader Pack encoder scribble address was wrong

### [3.0.10]

Fixed detection of the DAW on Windows 11\. WMIC no longer needs to be installed.

### [3.0.9]

Fixed crash with Control 24 and Reaper.

### [3.0.8]

Added info to install ‘Npcap’ for Windows 11

### [3.0.7]

Added compatibility for Luna for Windows  
Added compatibility for Luna and V-Control Pro 1 Legacy

### [3.0.6]

Added compatibility for MixBus 10  
Added compatibility for Ableton Live 12 Windows  
Added compatibility for Cubase 13 and V-Control Pro 1 Legacy 

### [3.0.5]

Fixed D-Command send and pan mode switching with Pro Tools.

### [3.0.4]

Improved D-Command metering with Pro Tools.

### [3.0.3]

Fixed D-Command Main stability problems when used with Logic.  
Improved D-Command metering speed.

### [3.0.2]

Fixed D-Command Fader Pack scribble strips for Live and other Mackie Control based DAWs.  
Improved MIDI Mode switching to switch all devices in a setup.  
Added FL Studio support for C|24, Control|24, ProControl, Command|8  
Added Adobe Audition support for C|24, Control|24, ProControl, Command|8

### [3.0.1]

Fixed Transport Return To Zero (RTZ) for Studio One on all supported surfaces.  
Fixed menu not updating if license status changes.  
Fixed Activate License… menu option to look for all types of licenses.

### [3.0]

Added support for FaderPort 8 / 16..

#### Version 2.11.4

Fixed crashing that could happen with Studio One and C24.

#### Version 2.11.3

Added MixBus 32C-9 Support.  
Fixed mapping for ProControl Main and MixBus.

#### Version 2.11.2

Not released.

#### Version 2.11.1

Added a first-time launch message to help users locate the application menu.

#### Version 2.11

C24

* Added support for Pro Tools for use with Pro Tools on macOS Apple Silicon systems.

Command 8

* Added support for Pro Tools for use with Pro Tools on macOS Apple Silicon systems.

#### Version 2.10.1

macOS Ventura

* Fix OS version detection to allow Ethernet features

Digidesign 003 Console

* Added compatibility for Automation Buttons  
  * Logic Pro  
  * Cubase/Nuendo  
  * Studio One  
  * Luna  
  * MixBus  
* Fixes  
  * Logic Pro Track Names and Display Mode  
  * Console Mode Buttons

#### Version 2.10

Digidesign 003 Console

* Added support for Mac DAWs on Intel  
* Added support for Windows DAWs on Windows 10, 11

C24

* Fixed Zoom Preset Buttons For Custom Commands With Cubase / Nuendo

#### Version 2.9.7

D-Command

* Added support for Pro Tools Studio

RAVEN

* Fixed Logic Pro connection issue that started in 2.9.0

#### Version 2.9.6

Command|8

* Fixed Automapping with Reaper

ProControl

* Fixed ProControl and Live automatic mapping.

Steinberg

* Fixed issue where Cubase/Nuendo did not connect.

V-Console

* Fixed issue where V-Console did not connect.

#### Version 2.9.5

C|24

* Fixed communication errors

Command|8

* Fixed Automapping with Digital Performer

FaderPort V2

* Added Redo Button for Pro Tools (Shift+Next)  
* Added Mix/Edit Window Toggle Button for Pro Tools (Shift+Master)

MixBus 32C

* Added support for version 8 with V-Control Pro

RAVEN, V-Control Pro 1.9 For iPad

* Fixed compatibility issue introduced in 2.9.4

#### Version 2.9.4

MIDI Mode Feature added

* ProControl  
* Control|24  
* D-Command  
* C|24

Added V-Window mode for all DAWs

* ProControl  
* Control|24  
* D-Command  
* C|24  
* Command|8

C|24

* Record Button fixed for Steinberg

Merged v 2.8 fixes

D-Command

* DAW Support for Logic, Steinberg, Mackie Control Compatible applications  
* Added D-Command Soft Keys section to MIDI Mode 

ProControl Main

* Fixes with Digital Performer

#### Version 2.9.3

ProControl Edit Pack

* Fixed crash

ProControl Main

* Fixed matrix ordering with Pro Tools


PreSonus FaderPort V2, ioStation 24c

* Changed foot switch to control Pro Tools Record

#### Version 2.9.2

D-Command

* Improved Cubase / Nuendo to access EQ (toggle with Inserts button on channel strip).  
* Added Resolve support. Use Resolve 17.4.6 or later. Connect with HUI. Features are very limited.

ProControl with Pro Tools

* Fixed MIDI Mode on Fader Pack

PreSonus FaderPort V2 ioStation 24c

* Implemented foot switch to control Pro Tools QuickPunch

#### Version 2.9.1

D-Command

* Fixed Logic notification message display

#### Version 2.9

MIDI Mode

* Added MIDI Mode feature for surfaces.

V-Window

* Added V-Window feature for hardware surfaces.

D-Command

* Added DAW support for D-Command Main and one Fader Module  
* Added MIDI Mode. Press “Midi Events List” to toggle MIDI Mode  
* Added V-Window mouse control for all supported DAWs  
* See [Compatibility Chart](https://neyrinck.com/vcpro-compatibility) for supported DAWs  
* Learn more [HERE](https://neyrinck.com/dcommand).

C24

* Improved fader accuracy for Pro Tools  
* Improved fader accuracy for Logic Pro  
* Added V-Window mouse control for all supported DAWs  
* Added MIDI Mode. Press “Focus” to toggle MIDI Mode.  
* See [Compatibility Chart](https://neyrinck.com/vcpro-compatibility) for supported DAWs

Control 24

* Improved fader accuracy for Pro Tools  
* Improved fader accuracy for Logic Pro  
* Command modifier for fine-mode encoder control  
* Added V-Window mouse control for all supported DAWs  
* Added MIDI Mode. Press “Mon 0” to toggle MIDI Mode.  
* See [Compatibility Chart](https://neyrinck.com/vcpro-compatibility) for supported DAWs

ProControl

* Improved fader accuracy for Pro Tools  
* Improved fader accuracy for Logic Pro  
* Added V-Window mouse control for all supported DAWs  
* Added MIDI Mode. Press “Mon 0” to toggle MIDI Mode.  
* See [Compatibility Chart](https://neyrinck.com/vcpro-compatibility) for supported DAWs

Command 8

* Added V-Window mouse control for all supported DAWs  
* See [Compatibility Chart](https://neyrinck.com/vcpro-compatibility) for supported DAWs

macOS

* Apple Silicon Native Compatibility

#### Version 2.8.4

Legacy V-Control Pro 1 for Cubase 12

* Added support V-Control Pro 1.9 on iPad for Cubase 12

ProControl for Reaper

* Fixed LCDs on extender banks to show correct channel info.

#### Version 2.8.3

FaderPort For Pro Tools

* Fixed RTZ function when pressing rewind and fast forward buttons simultaneously.

Digital Performer

* Basic control with C24
* Basic control with Control 24
* Basic control with ProControl

Improved Support For Multiple HUI / Mackie Control Applications

* V-Control Pro now connects to the most recently launched HUI or Mackie Control-based DAW. And now there is a preference to select a preferred DAW to connect to.

#### Version 2.8.2

V-Window

* Fixed to support macOS Monterey and V-Console  
* Fixed issue where V-Window control from V-Console iPad did not control Pro Tools popup menus correctly.

Windows OS

* Fixed issue where file named ‘ncontrol’ was appearing on the desktop

#### Version 2.8.1

LUNA

* Added LUNA Support  
* C24, Control 24, ProControl, Command 8, V-Console

Control 24, C24, ProControl

* Added V-Window Fader Mode For Pro Tools  
* Control 24, C24, ProControl \- Tap Master Fader

FaderPort / ioStation24C

* Added Pan flip mode for FaderPort / ioStation24C.

Logic Pro

* Fixed problem where Raven does not connect to Logic if computer has no Ethernet port and Wi-Fi is turned off.  
* Fixed problem where surface is not updated when connecting to Logic on M1 systems.

#### Version 2.8

PreSonus ioStation 24c

* Added direct support for PreSonus ioStation 24c

FaderPort / ioStation 24c

* Added V-Window mode to control plugin parameters  
* Changed Send A-D select to use Master, Click, Section, Shift+Section

#### Version 2.7.5 CHANGES

Added supercharging PreSonus FaderPort with Pro Tools. neyrinck.com/faderport

**VERSION 2.7.4 CHANGES**

Fixed Command8 for Logic Pro X to display status info at top correctly.  
Fixed V-Console for Logic Pro X to display track names and other text.

Compatibility added for Nuendo 11 legacy V-Control Pro 1.9 for iPad.

**VERSION 2.7.3 CHANGES**

Apple M1 systems now supported for Logic Pro X. Other DAWs probably probably will work, but Cubase/Nuendo will not.

Logic Pro X users must delete their old surfaces in Control Surfaces / Setups… Logic Pro X 10.6 does not properly refresh a new control surface when it is added. Please close and re-open your project.

V-Control Pro 2.7.3 is compatible with Logic Pro X 10.6 and later only. If you are using version 10.5 or earlier, please install V-Control Pro 2.7.2.

For Logic Pro X, V-Control Pro 2.7.3 does not support multiple ProControl Fader Pack devices at this time. If you have multiple Fader Packs, you must use V-Control Pro 2.7.2, which will only work on Intel Macs. At this time, multiple Fader Pack units are not supported on Apple M1 Mac systems.

Add support for Logic Pro X on Apple M1-based systems.  
Fix hanging problem on Mac when computer name is long.

Compatibility with Adobe Premiere Version 15.1

**VERSION 2.7.2 CHANGES**

Fix Zoom Preset and Function button for Control24 and Cubase/Nuendo.  
Compatibility with Mixbus32C Version 7 .

**VERSION 2.7.1 CHANGES**

Basic Reaper Support for ProControl, Control24, C24, and Command 8\.

**VERSION 2.7.0 CHANGES**

Digidesign Command 8 Support  
	MixBus  
	Logic Pro X  
	Ableton Live  
	PreSonus Studio One

Issues Fixed  
	Cubase hanging with C24  
	Windows Uninstaller not removing virtual MIDI ports

**VERSION 2.6.2 CHANGES**

Cubase / Nuendo Improvements For ProControl / Control24, C24  
	Master Fader Control  
	Output Metering \- Stereo and 5.1  
	Auto-Bank Follow Function \- Use Focus button for C24, Shuffle button for Control24, F1 button for ProControl  
	F1 \- F10 Programmable Buttons For Control24

**VERSION 2.6.1 CHANGES**

Added support for MixBus with ProControl / Control24, and C24

Added support for Ableton Live with ProControl / Control24, and C24

Improvements for Logic Pro X and ProControl / Control24, and C24.  
	Assignable inserts  
	Improved assignment of inputs, outputs, and sends  
	Soft keys assignable in Logic Pro X controller assignments window.  
	Stereo output metering

**VERSION 2.6 CHANGES**

Added support for ProControl Edit Pack with Pro Tools. 

**VERSION 2.5.6 CHANGES**

Improved V-Window to be compatible with Catalina security and privacy settings.   
Fixed intermittent bug where an Ethernet surface meters and counter freeze for a second.  
Fixed zoom control of Cubase with cursor keys on ProControl, Control|24, and C|24.

**VERSION 2.5.5 CHANGES**

Fixed Control 24 fader touch messaging for strips 9-24.  
Improved Mac Ethernet permissions handling for Catalina-level security.

**VERSION 2.5.4 CHANGES**

Added support for C|24 Auto Talkback feature.

**VERSION 2.5.3 CHANGES**

Added support for latest Adobe Audition on Windows named Audition.exe.

**VERSION 2.5.2 CHANGES**

Added support for Nuendo 10.0

**VERSION 2.5.1 CHANGES**

macOS installer improved to be compatible with Catalina Gatekeeper.  
Control improvements for Logic Pro X, Cubase/Nuendo, and Studio One.

Website Page Listings Of Control Features:  
[Logic Pro X](https://neyrinck.com/logic-pro-x-control-features/)  
[Cubase / Nuendo](https://neyrinck.com/steinberg-control-features/)  
[Studio One / Fender Studio](https://neyrinck.com/studio-one-control-features/)

**VERSION 2.5 CHANGES**

Added support for the Digidesign C|24 control surface. Compatible DAWs are Logic Pro X, Cubase/Nuendo, and Studio One.

**VERSION 2.4 CHANGES**

Support for PreSonus Studio One on Control24 and ProControl.  
Pro Tools plug-in editing on Control24.  
Logic Pro X enhancements for Control24 and ProControl.