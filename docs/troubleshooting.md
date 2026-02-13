# Troubleshooting

This guide will help you resolve common V-Control Pro issues. Start with the [Quick Checklist](#quick-checklist) for immediate help, then follow the detailed sections as needed.

## Quick Checklist {#quick-checklist}

Before diving into detailed troubleshooting, try these common solutions:

1. **Update to Latest Version**: [Download V-Control Pro 3.X](https://neyrinck.com/download/v-control-pro/)
2. **Verify License**: Check `About V-Control Pro` shows "Licensed"
3. **Check Surface Connection**: Surface should appear "bold" (connected) not "grayed out" (disconnected) in Setups
4. **Restart Both Apps**: Quit both V-Control Pro and your DAW, then relaunch
5. **Review Setup Guide**: Verify your [controller setup](./controllers-overview.md) and [DAW configuration](./pro-tools.md)

---

## Step-by-Step Troubleshooting

### Step 1: Update V-Control Pro {#step-1-update}

Older versions may not support your control surface or operating system.

####Check Your Version:
1. Launch V-Control Pro
2. Select `About V-Control Pro` from the menu
3. Verify you're running V-Control Pro 3.X

**Download Updates:**
- Get the latest version: [Neyrinck Downloads](https://neyrinck.com/download/v-control-pro/)

!!! warning "Windows 11 Compatibility"
    V-Control Pro 2.X is **incompatible** with Windows 11. You must use V-Control Pro 3.X. Existing V-Control Pro 2 Standard licenses work with V-Control Pro 3.

### Step 2: Verify Licensing {#step-2-license}

V-Control Pro requires a valid license for most systems.

####Check License Status:
1. Launch V-Control Pro
2. Select `About V-Control Pro`
3. Look for "Licensed" or "Not Licensed"

####If Not Licensed:
- **Trial License**: [Get 14-day trial](https://neyrinck.com/v-control-pro-trial/)
- **Purchase**: [Neyrinck Store](https://neyrinck.com/store/)
- **Activate**: Follow the [licensing guide](./v-control-pro-licensing.md#license-activate)

!!! note "License Exceptions"
    - **RAVEN users**: No V-Control Pro license required
    - **Legacy iPad App v1.9**: No license required

### Step 3: Add and Connect Your Surface {#step-3-surface}

Your control surface must be properly added and connected in V-Control Pro.

####Check Surface Status:
1. Launch V-Control Pro
2. Open `Setups...` menu
3. Look at the Controllers section (lower left)
   - **Bold text** = Connected ✓
   - **Grayed out** = Not connected ✗

####Add a New Surface:
1. Click `Add new...` button in `Controllers` section
2. Select your surface type
3. Follow the setup prompts
4. See [Controllers Overview](./controllers-overview.md) for detailed instructions

---

## Connection Issues by Controller Type

### Ethernet Controllers {#ethernet-troubleshooting}

####Visual Connection Check
1. Verify Ethernet cable is connected at both ends
2. Check the LED indicator next to the Ethernet port on your surface
3. LED should show activity - if not, try a different cable

####Network Configuration

=== "macOS"
    It is important that the Ethernet port is configured in System Settings -> Network.

    - Open `System Settings / Network` and locate the ethernet port you are using.
    - **Red Ethernet port (Not Connected)**: If the ethernet port is displayed in a red color and/or indicates that it is not connected, use a network switch between computer and surface as described in [Ethernet Switches](./ethernet-controllers.md#ethernet-switches-not-hubs)
    - **Self-assigned IP**: This is normal and OK
    - **Firewall**: `System Settings / Network / Firewall` (disable to test)

=== "Windows"
    - **Required**: Install [Npcap](https://npcap.com/#download)
    - **Remove**: Uninstall Win10Pcap if present
    - **Firewall**: Temporarily disable to test

####If Surface Not Detected
- Confirm Ethernet LED is active (see Visual Connection Check above)
- Check computer's Ethernet port is enabled
- Temporarily disable firewall/antivirus
- Review [Ethernet Controllers guide](./ethernet-controllers.md#networking)

!!! warning "Symantec Endpoint Protection"
    Known to cause issues on Windows. Temporarily disable for testing.

### MIDI Controllers {#midi-troubleshooting}

**Check MIDI Port Assignment:**
1. Open V-Control Pro `Setups...`
2. Click your grayed-out MIDI surface
3. Verify correct MIDI Input/Output ports are selected
4. Ports should match your interface's MIDI connections

**Common MIDI Issues:**
- Wrong ports selected
- MIDI interface driver not installed
- Ports in use by another application

---

## Operating System Specific Issues

### Windows Issues {#windows-troubleshooting}

#### Windows 11 Upgrade Problems

If you upgraded from Windows 10 to Windows 11 and V-Control Pro stopped working:

**Complete Reinstallation Process:**
1. Quit your DAW and V-Control Pro
2. Uninstall V-Control Pro
3. Restart computer
4. [Reset V-Control Pro preferences](#reset-windows-prefs)
5. **For Ethernet surfaces only:**
   - Uninstall Npcap (if installed)
   - Uninstall Win10Pcap completely
   - If uninstall fails: Restart → Reinstall Win10Pcap → Uninstall again
   - Install [Npcap](https://npcap.com/#download)
6. Open Device Manager → View → Show Hidden Items
7. Remove any hidden "V-Control" MIDI ports
8. Install latest [V-Control Pro](https://neyrinck.com/download/v-control-pro/)
9. Restart computer
10. Launch V-Control Pro and add your surface

#### V-Control Pro Won't Launch

If V-Control Pro fails to launch on Windows, try these solutions:

**Check Startup Items:**

V-Control Pro may not launch correctly when set as a startup item.

1. Open Task Manager (Ctrl+Shift+Esc)
2. Select the Startup tab
3. Look for V-Control Pro in the list
4. If present, right-click it and select Disable
5. Restart your computer
6. Launch V-Control Pro manually

**Upgraded from Windows 10 to Windows 11:**

If you upgraded from Windows 10 to Windows 11 and V-Control Pro no longer launches:

1. Uninstall V-Control Pro completely
2. Restart your computer
3. Install the latest [V-Control Pro](https://neyrinck.com/download/v-control-pro/)
4. Restart your computer
5. Launch V-Control Pro

**Check if V-Control Pro is Hanging or Crashing:**

If V-Control Pro appears to launch but doesn't show a window, it may be hanging or crashing.

=== "Check for Hanging Process"
    1. Launch Task Manager (Ctrl+Shift+Esc)
    2. Select `More details` if the `Processes` tab is not showing
    3. Look for "V-Control Pro" under Background processes
    4. If found, right-click it and select `Create dump file`
    5. Send the generated .dmp file to [support@neyrinck.com](mailto:support@neyrinck.com)

=== "Check for Crash"
    If V-Control Pro does not appear in Task Manager, it may be crashing on startup:

    1. Download and configure crash dump generation:
        - Download: [EnableCrashDumps.reg.zip](https://neyrinck.sfo2.digitaloceanspaces.com/EnableCrashDumps.reg.zip)
        - Unzip the file
        - Double-click `EnableCrashDumps.reg` to configure Windows
    2. Launch V-Control Pro and confirm it does not launch correctly
    3. Press `Windows+R` to open the Run dialog
    4. Enter: `%LOCALAPPDATA%` and press `Enter`
    5. Locate the CrashDumps folder
    6. Find the .dmp file for V-Control Pro (most recent file)
    7. Send the .dmp file to [support@neyrinck.com](mailto:support@neyrinck.com)

#### Updating from V-Control Pro 2 to 3
Pro Tools may lose MIDI port connections:
1. Quit Pro Tools
2. [Delete Pro Tools preferences](https://www.sweetwater.com/sweetcare/articles/how-do-i-trash-my-pro-tools-preferences/#Trash-Pro-Tools-Preferences-for-PC)
3. Restart Pro Tools
4. Reconfigure MIDI settings

#### Reset V-Control Pro Preferences {#reset-windows-prefs}
1. Quit V-Control Pro and any DAW
2. Open Windows Explorer
3. Enable "Show hidden files and folders"
4. Navigate to: `C:\Users\{YourUsername}\AppData\Roaming\Application Support`
5. Delete the "V-Control Pro" folder
6. Empty Recycle Bin
7. Launch V-Control Pro and reconfigure

### macOS Issues {#macos-troubleshooting}

#### V-Control Pro Won't Launch

Some users have seen a problem when V-Control Pro is set up to be automatically launched when the computer restarts. These steps will typically solve the problem.

1. Remove V-Control Pro from Login Items
    * Open `System Settings / General`
    * Select `Login Items`
    * Locate V-Control Pro and disable it as a login item
2. Restart computer
3. Launch V-Control Pro manually

#### Reset V-Control Pro Preferences {#reset-macos-prefs}

When upgrading to a new version of V-Control Pro, some issues have been solved by resetting V-Control Pro.
Quit V-Control Pro and any active DAW.

1. Open Finder and select the Go menu at the top of your screen.

2. Hold the Option (Alt) key to reveal the hidden Library folder, then click to open it.

3. Navigate to Application Support and locate the folder named V-Control Pro.

4. Delete the V-Control Pro folder and empty your Trash.

5. Relaunch V-Control Pro and reconfigure your settings as needed.

---

## DAW-Specific Issues

### Logic Pro Issues {#logic-troubleshooting}

!!! info "Critical Setting"
    Logic Pro requires **Automatic Installation** enabled to detect V-Control Pro surfaces.

#### Erratic / Inconsistent Control

Logic Pro has issues where its control assignments for a surface can get corrupted and control partially works, but does work in both directions. This can happen when a V-Control Pro update is installed or a different surface is added. Typically, this can be solved by "resetting" the control surface setup.

* Reset Logic Pro Control Surface Setup
    * Open `Logic Pro Control Surfaces / Setup` window
    * Delete all surfaces
    * Quit Logic Pro
    * Launch Logic Pro and set up your surface as described in [Logic Pro Setup](./logic-pro.md) guide

#### Not Detecting Your Surface

Logic Pro should detect your V-Control Pro surface automatically and add it to the Logic Pro Control Surfaces / Setup... window. If it is not being detected, check the following items.

* Surface not detected by Logic Pro
    * Review the [Logic Pro Setup](./logic-pro.md) guide
    * Enable Automatic Installation in Logic preferences
    * Disable local network firewall.
    * macOS Sequoia and later require V-Control Pro to be enabled in `System Settings / Security / Network`
    * Review the [Logic Pro Protocol](./logic-pro.md#ipv6-setting) settings guide.

#### One-Way Or No Surface Communication

macOS Sonoma and later started to exhibit a problem where Logic Pro automatically adds the surface to its setup, but there is one-way or no communication between the surface and Logic Pro.
Another common problem is one-way communication. We have demonstrated this to Apple, but they have not acknowledged it.

* Review the [Logic Pro Protocol](./logic-pro.md#ipv6-setting) settings guide.


### Pro Tools Issues
- See [Pro Tools Setup](./pro-tools.md) guide
- After Windows upgrades, delete Pro Tools preferences
- Reconfigure MIDI Input Enables and Peripherals

---

## Hardware Diagnostics

If buttons, faders, or displays aren't working properly, the issue may be hardware-related.

### Command 8 Diagnostics
Press the **F1 Utility** switch to enter diagnostic mode.

### General Hardware Troubleshooting
1. Check all cable connections
2. Try different cables
3. Test on another computer if possible
4. Consult your surface's user manual for built-in diagnostics

---

## Still Need Help?

If these steps don't resolve your issue:

1. **Check Documentation**: Review setup guides for your specific [controller](./controllers-overview.md) and [DAW](./pro-tools.md)
2. **Get Support**: Contact [Neyrinck Support](https://neyrinck.com/support/) with:
   - Your V-Control Pro version
   - Operating system details
   - Control surface model
   - DAW application and version
   - Specific symptoms you're experiencing

