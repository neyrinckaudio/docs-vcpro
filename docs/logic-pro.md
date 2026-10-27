# Setting Up Logic Pro X

Logic Pro will not be detected until it has connected to a control surface supported by V-Control Pro with Logic Pro. Follow these steps to connect it to a control surface.

!!! info "Version Compatibility"
    **V-Control Pro 3**: Compatible with Logic 10.6 and later only
    
    **V-Control Pro 2.7.2**: Required for Logic 10.5 or earlier

!!! info "Automatic Installation Must Be Enabled"
    Logic Pro will not detect V-Control Pro surfaces unless Automatic Installation is enabled.

!!! info "Enable System Settings / Security / Network"
    macOS Sequoia and later require V-Control Pro to be enabled.

!!! info "One Way Communication Issue"
    If Logic Pro has one-way communication with a V-Control Pro surface, try changing the [Logic Protocol Setting](#ipv6-setting).

* Open the V-Control Pro Setups window and make sure your surface has been added to the `Controllers...` section and is actively detected.
* Launch Logic Pro
* Ensure "Automatic Installation" is enabled in the Control Surface setup in Logic.
* Logic automatically detects any controller setup through V-Control Pro. Click Connect when the automatic setup window pops up.
* Select "Add" when the window pops up saying it has detected Control Surface.
* V-Control Pro and Logic Pro should now have bidirectional communication.
* In some cases, Logic Pro will provide one-way communication. If that happens, follow these steps:
    * Quit Logic Pro.
    * Open the V-Control Pro `Preferences` window. Toggle the 'Logic Pro - Use IPv6' setting.
    * Launch Logic Pro.

<a id="grouping-devices"></a>
### Grouping Multiple Devices

Some surfaces use more than one device and need extra setup in Logic:

* **D-Command** Main with a Fader Module
* **ProControl** Main with a Fader Pack

Logic adds each device in its own row as an independent controller, so each device banks and scrolls on its own. To make the devices bank together as one surface, put them in the same row in Logic's Control Surfaces Setup window.

!!! note "Single-Device Surfaces"
    C|24, Control 24, Command|8, and Digi 003 are each a single device. They do not need grouping.

1. Connect all devices to Logic as described above.
2. In Logic, choose `Logic Pro > Control Surfaces > Setup...`.
3. Each device appears in its own row. Drag the device icons into a single row.
4. Arrange the icons left to right in the same order as the hardware on your desk. For example, if the Fader Module is to the left of the D-Command Main, place its icon to the left of the Main's icon.
5. Close the Setup window. Banking now moves all of the devices together.

<!-- TODO: add screenshots of the Control Surfaces Setup window before and after grouping -->

<a id="ipv6-setting"></a>
#### Logic Pro Protocol Settings (new in v 3.0.22)

V-Control Pro uses UDP networking to communicate with Logic Pro. Users sometime see an issue where communication operates in one direction only. Typically, Logic Pro operates perfectly using IPv4 protocol with the Localhost IP address. Other times it works perfectly using IPv6 protocol with the Localhost IP address. With macOS Tahoe, it typically works perfectly using IPv4 protocol with the WiFi IP address. We have contacted Apple about this but they have not responded.

##### If You Experience One-Way Communication With Logic Pro

* Quit Logic Pro.
* Select the V-Control Pro Preferences... menu item.
* Select the `Logic Pro Protocol` popup menu.
    * For macOS Tahoe and later, select `Default`
    * For macOS Sequoia and earlier, select `IPv6`
    * If the other selections do not work, try `IPv4 Localhost`
* Click OK
* Quit V-Control Pro
* Launch V-Control Pro
* Launch Logic Pro

We have demonstrated this problem to the Logic Pro team, and they have not acknowledged it.