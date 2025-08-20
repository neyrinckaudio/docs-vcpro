# Setting Up Logic Pro X

Logic Pro will not be detected until it has connected to a control surface supported by V-Control Pro with Logic Pro. Follow these steps to connect it to a control surface.

!!! info "Automatic Installation Must Be Enabled"
    Logic Pro will not detect V-Control Pro surfaces unless Automatic Installation is enabled.

!!! info "Enable System Settings / Security / Network"
    Mac OS Sequoia and later require V-Control Pro to be enabled.

!!! info "One Way Communication Issue"
    If Logic Pro has one-way communication with a V-Control Pro surface, try changing the [IPv6 Setting](#ipv6-setting).

* Open the V-Control Pro Setups window and make sure your surface has been added to the Controllers... section and it is actively detected.
* Launch Logic Pro
* Ensure "Automatic Installation" is enabled in the Control Surface setup in Logic.
* Logic automatically detects any controller setup through V-Control Pro. Click Connect when the automatic setup window pops up.
* Select "Add" when the window pops up saying it has detected Control Surface.
* V-Control Pro and Logic Pro should now have bidirectional communication.
* In some cases, Logic Pro will provide one-way communication. If that happens, follow these steps:
    * Quit Logic Pro.
    * Open the V-Control Pro Preferencess window. Toggle the "Logic Pro - Use IPv6" setting.
    * Launch Logic Pro.

<a id="ipv6-setting"></a>

#### IPv6 Settings

V-Control Pro uses UDP networking to communicate with Logic Pro. Users sometime see an issue where communication operates in one direction only. Typically, Logic Pro operates perfectly using IPv4 protocol. Other times it works perfectly using IPv6 protocol. 

##### If You Experience One-Way Communication With Logic Pro

* Quit Logic Pro.
* Select the V-Control Pro Preferences... menu item.
* Toggle the<b>Logic Pro - Use IPv6</b> item.
* Click OK
* Launch Logic Pro

We have demosntrated this problem to the Logic Pro team and they have not acknowledged it.