# Troubleshooting

<a id="step-0"></a>
## Update Your Old Version

If you are using an old version of V-Control Pro, it might not support the surface you are trying to use. Installer downloads are available at the [Neyrinck Downloads Page](https://neyrinck.com/downloads/v-control-pro).

<a id="step-1"></a>
## Verify The License

V-Control Pro needs to be licensed for most systems, using either a trial license or a purchased license. [Learn more about Licensing](./v-control-pro-licensing.md)

!!! note "RAVEN Info"
    RAVEN users do not need to use a V-Control Pro license.

!!! note "Legacy iPad App V 1.9 Info"
    The original V-Control Pro iPad app (version 1.9) users do not need to use a V-Control Pro license.

#### Check If V-Control Pro Is Licensed

* Launch V-Control Pro
* Select the <b>About V-Control Pro</b> menu item to open the About window.
* The About window will indicate "Licensed" or "Not Licensed."
* If it is licensed, proceed to [Step 2](#step-2).

#### V-Control Pro Is Not Licensed, What Next?

* Get A License

    * You can get a trial license at the [Neyrinck Trial License Page](https://neyrinck.com/v-control-pro-trial/).
    * You can purchase a license at the [Neyrinck Store](https://neyrinck.com/store/).
    
* Activating A License
    * After getting a license deposited to your iLok user account, you must [activate the license](./v-control-pro-licensing.md/#license-activate).
    * After activating, verify that V-Control Pro is licensed.
        * Quit V-Control Pro.
        * Go back to [Step 1 - Verify The License](#step-1)

<a id="step-2"></a>

## Make Sure Your Surface Is Added To Setups

V-Control Pro will only work if your control surface is added to the Setups window. and is detected to be in the Setups window.

#### Check If Your Control Surface Is Added

* Launch V-Control Pro.
* Select the V-Control Pro <b>Setups...</b> menu item to open the Setups window.
* Look at the <b>Controllers</b> section at the lower left.
    * If your surface is already added, [verify it is connected](#verify-connected)
    * If your surface is not added, [add your control surface](#add-surface)

<a id="add-surface"></a>

#### Add Your Control Surface

* Launch V-Control Pro.
* Select the V-Control Pro <b>Setups...</b> menu item to open the Setups window.
* Click the <b>Add new...</b> button in the Controllers section at the lower left of the Setups window.
* Select the type of surface you are adding. For more information see 

<a id="verify-connected"></a>

## Make Sure Your Surface Is Connected

#### Check If Your Control Surface Is Connected

* Launch V-Control Pro.
* Select the V-Control Pro <b>Setups...</b> menu item to open the Setups window.
* Look at the Controllers section of the Setups window
    * If the control surface name is "grayed out," then it is not connected.
        *  Try looking at 
    * If the control surface name is "bold," then it is connected 

#### Troubleshooting Controllers That Are Not Connected

If the Setups window shows your surface name as "grayed out," then it is indicating the surface is not detected.

* Try [Troubleshooting Ethernet Issues](#ethernet-issues)
* Review the [Ethernet Controllers Section](./ethernet-controllers.md)

<a id="ethernet-issues"></a>

#### Troubleshooting Ethernet

<a id="ethernet-led"></a>

##### Ethernet LED Indicator
Ethernet control surfaces have an LED indicator on the rear panel next to the ethernet cable jack. This LED indicates if an ethernet connection is active.

* Check the rear panel of your control surface to make sure an ethernet cable is connected.
* Check the rear panel of your control surface to make sure the LED indicator at the ethernet connector indicates activity. If the LED does not indicate activity, then there are several possible probelms:
    * The ethernet cable is faulty. Try using a different cable.
    * The ethernet cable is not connected at both ends.
    * The control surface hardware has an issue.

##### The Add Ethernet Device... Window Does Not Show The Surface

When you select the <b>Add Ethernet Device...</b> option in the <b>Add new...</b> controller window, V-Control Pro monitors a network to detect if a surface is available. If no surface is seen, you will need to check a few things:

* Is the [Ethernet LED Indicator](#ethernet-led) on the surface active?
* Is the ethernet port enabled in the computer?
    * For Mac OS, open System Settings / Network. If the ethernet port is colored red, then it is not enabled. Using a low cost network switch between the computer and surface usually solves this. A "self-assigned IP address" is OK because legacy ethernet surfaces do not use TCP/IP networking.
    * For Windows, make sure the "Npcap" utility is installed. Learn more about [Mac OS and Windows Networking](./ethernet-controllers.md/#networking)
    * For Windows, make sure the "Win10Pcap" utility is NOT installed.
* Is a Firewall active?
    * Open System Settings / Network / Firewall
    * Disable Firewall if it is enabled.
    * If you need to use a Firewall you will need to set options to allow your surface to operate on the network.
        * Legacy Ethernet surfaces use Ethernet 2 packets with MAC hardware addressing.
        * iPad apps use IP networking and zero configuration networking.

!!! warning "Symantec Endpoint Protection"
    Some Windows users have seen problems if Symantec Endpoint Protection is enabled. 

#### Troubleshooting Midi Controllers

If a Midi control surface has been added to the Setups window, but it is "greyed out," then V-Control Pro is not detecting it. PLease check the Midi ports assigned to connect to the surface.

##### Check The Midi Ports Assigned To The Midi Controller

* Launch V-Control Pro.
* Select the V-Control Pro <b>Setups...</b> menu item to open the Setups window.
* Look at the Controllers section of the Setups window
    * If the control surface name is "grayed out," then it is not connected.
        * Click the surface name to see the configuration details.
        * Check the Midi Input and Midi Output popup menus to confirm the correct ports are selected.
    * If the control surface name is "bold," then it is connected 

<a id="windows-os"></a>

## Windows OS Issues

Windows OS users have been able to solve problems using one or more of these steps. If you are using Mac OS, go to [Mac OS Issues](#mac-os).

#### I Updated From V-Control Pro 2 To V-Control Pro 3 And It Stopped Working

Some DAWs, especially Pro Tools on Windows, keep track of MIDI ports by number rather than by name. V-Control Pro 3 changed the ports and Pro Tools can get confused if you are updating V-Control Pro.

* Quit Pro Tools
* Trash Pro Tools Prefs
* Launch Pro Tools
* Reset Pro Tools Midi Input Enables.
* Reset Pro Tools Midi Peripherals.

#### V-Control Pro Is Not Launching

* Some users have seen an issue where V-Control Pro is unable to launch when updating a Windows 10 system to Windows 11. At least one user fixed it by installing Windows 11 from scratch.

#### The Control Surface Is Not Controlling The DAW

 * Did you update the BIOS?
    * Open the <b>Device Manager</b> and select <b>Sound Video And Game Controllers</b>
    * Select <b>Show Hidden Devices</b>
    * Delete any V-Control Midi ports that were hidden.
    * Restart your computer and verify the hidden ports have been deleted.

#### Resetting V-Control Pro on Windows:

Some issues with Setup or mapping configuration can be resolved by deleting the V-Control Pro Preference files. Follow the steps to reset the V-Control Pro Settings.

* Quit V-Control Pro and any DAW currently open.
* Open the Windows Explorer
* Enable to view hidden files and folders in Explorer.
* Navigate to C:\Users\{User Account}\AppData\Roaming\Application Support
* Find the V-Control Pro folder send it to the trash bin.
* Empty Trash.
* Launch V-Control Pro.
* Open the Setups window.
* Add your surface(s) again.
* launch the DAW.

<a id="mac-os"></a>

## Mac OS Issues

Mac OS users have been able to solve problems using one or more of these steps. If you are using Windowd OS, go to [Windows OS Issues](#windows-os).

#### V-Control Pro Is Not Launching On Mac OS

* Remove V-Control Pro As A Startup Item.
* Restart the computer.
* Launch V-Control Pro manually.

#### Resetting V-Control Pro on Mac OS:

Some issues with Setup or mapping configuration can be resolved by deleting the V-Control Pro Preference files. Follow the steps to reset the V-Control Pro Settings.

* Quit V-Control Pro and any DAW currently open.
* Go to the Finder Application
* Click on Go in the top menu bar for the Finder and with the Alt/Option key held down select Library.
* In the Finder window navigate to Application Support.
* Find the V-Control Pro folder send it to the trash bin.
* Empty Trash.
* Launch V-Control Pro.
* Open the Setups window.
* Add your surface(s) again.
* launch the DAW.


## Logic Pro Issues

!!! info "Automatic Installation Must Be Enabled"
    Logic Pro will not detect V-Control Pro surfaces unless Automatic Installation is enabled.

#### Common Logic Pro Issues

* Surface not detected by Logic Pro
* One-way communication

For these common issues, please review the [Logic Pro Setup Section](./logic-pro.md)

#### Other Logic Pro Issues

##### Corrupt Surface Configuration

Some users have observed "strange" control behaviors that have been solved by deleting all surfaces set up in Logic and setting it up again.

* Open Logic Pro <b>Control Surfaces / Setup</b> window.
* Delete all surfaces.
* Quit Logic.
* Start Logic and follow the info in the [Logic Pro Setup Section](./logic-pro.md)

## Hardware Fader, Button, Light, And Display Issues

If a control surface feature is not operating correctly, there might be a problem with the surface hardware. Some surfaces have built-in diagnostics that acan help diagnose these problems. Please search for the surface user guide online for more information.

#### Command 8
Press the F1 Utility switch to enter Utility mode.

