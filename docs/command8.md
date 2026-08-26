# Avid/Digidesign Command 8

!!! info "Control Features"
    Please see the Command 8 feature charts online at [Feature Charts](./feature-charts.md/#command-8).

### Setup

#### Command 8 Driver For Windows

Windows systems require a Command 8 driver to be installed. A driver can be downloaded from [HERE](http://akmedia.digidesign.com/support/compressed/Command8_Driver_Pro_Tools%20v90_69592.zip).

#### Windows 11 Blocks The Command 8 Driver {#windows-11-driver-signing}

The April 2026 Windows security update removed default trust for kernel drivers signed through the old cross-signed driver program. It applies to Windows 11 24H2, Windows 11 25H2, Windows 11 26H1, and Windows Server 2025. The Command 8 driver, `c8usb_vistacomp.sys`, is a cross-signed driver from that era, so Windows can now refuse to load it.

Symptoms:

* The Command 8 does not appear as a MIDI device, or appears with a warning triangle in Device Manager.
* V-Control Pro cannot communicate with the Command 8.
* The `Code Integrity / Operational` event log contains Event ID 3077 (driver blocked) or Event ID 3076 (driver audited) for `c8usb_vistacomp.sys`.

To check the log, open Event Viewer and go to `Applications and Services Logs / Microsoft / Windows / CodeIntegrity / Operational`.

!!! info "This Is Not A V-Control Pro Problem"
    The Command 8 driver is an Avid/Digidesign driver. V-Control Pro communicates with the Command 8 using the MIDI ports that driver creates, so V-Control Pro cannot load the driver or change how Windows trusts it. Neyrinck cannot re-sign a driver it does not own. Disabling the memory integrity setting, the vulnerable driver blocklist, or Secure Boot does not help, because this is a separate trust check.

##### User-Reported Workaround

A V-Control Pro user restored Command 8 operation by removing the Windows Code Integrity policy that enforces the new rule. Please read the warning below before you decide to do this.

!!! warning "This Weakens A Windows Security Protection"
    Removing this policy turns off the new kernel driver trust check for the entire system, not only for the Command 8. Every other cross-signed driver becomes loadable again. Neyrinck and Microsoft do not support this procedure and you perform it at your own risk. Back up the policy file first so you can put it back, and do not delete any other Code Integrity policy.

1. Open PowerShell as an Administrator.
2. List the active policies and locate `Microsoft Windows Cross Certificates for Code Integrity Exceptions Policy`. Note its policy ID.

        CiTool --list-policies

    The reported ID is `8f9cb695-5d48-48d6-a329-7202b44607e3`. `CiTool --remove-policy` fails on this policy with error `0x80070005`, even from an elevated PowerShell, which is why the file is removed by hand.

3. Mount the EFI System Partition so you can reach the policy file.

        mountvol S: /S

4. **Back up the policy file.** Copy the `.cip` file that matches the policy ID from `S:\EFI\Microsoft\Boot\CiPolicies\Active\` to a safe location such as your Documents folder.

5. Delete that same `.cip` file from `S:\EFI\Microsoft\Boot\CiPolicies\Active\`. Leave every other file in the folder alone.

6. Restart the computer.

After the restart, the `command8` driver reports `Running` and `OK` with the driver file `C:\Windows\System32\drivers\c8usb_vistacomp.sys`, the Command 8 appears under MIDI devices with no warning triangle, and V-Control Pro communicates with it.

To undo the change, copy the backed up `.cip` file back into `S:\EFI\Microsoft\Boot\CiPolicies\Active\` and restart the computer.

!!! note "A Windows Update May Restore The Policy"
    A later Windows update can install the policy again and block the driver again. Keep your backup copy and check this section again if the Command 8 stops working after an update.

#### Add Command 8 To The Setups Window

First, you must add Command 8 as a controller in the V-Control Pro Setups window as described in [Setting Up MIDI Controllers](./midi-controllers.md).

#### Pro Tools
Set up Pro Tools for one HUI bank as described in [Setting Up Pro Tools](./pro-tools.md).

#### Logic Pro X

Set up Logic Pro X for Command 8 as described in [Setting Up Logic Pro](./logic-pro.md).

#### Cubase/Nuendo

Set up Cubase / Nuendo for Command 8 as described in [Setting Up Cubase/Nuendo](./cubase-nuendo.md).

#### Mackie Control DAWs

Set up the DAW for Command 8 using one Mackie Control bank as described in [Setting Up Mackie Control](./mackie-control.md).

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

