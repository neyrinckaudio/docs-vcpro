# Install And Run V-Control Pro

V-Control Pro is a desktop computer application that must be installed on the same computer that runs the DAW or media application to be controlled by a surface.

* Download Installer - Use a web browser to open the [Neyrinck Downloads Page](https://neyrinck.com/downloads/v-control-pro). Download the appropriate installer for your system.

* Launch Installer - Install and launch the V-Control Pro application on your computer as described in the 'Installing V-Control Pro' section.

* Run V-Control Pro - On Mac, use the Finder to go to the Applications folder. Locate V-Control Pro and double-click it. On Windows locate V-Control Pro and double-click it.

* Typically, you will need to activate a license to use V-Control Pro. For more information about getting a trial license or purchasing a license see the [Licensing](./v-control-pro-licensing.md) section.

!!! note "macOS Privacy Permissions"
    Basic surface control does not require any macOS privacy permissions. The [V-Window](./v-window.md#macos-privacy-permissions) feature does — macOS blocks it until V-Control Pro is enabled in `System Settings / Privacy & Security`.

## Launch At Login

V-Control Pro can start automatically when you log in to your computer, so your surfaces are ready without launching it by hand. This is set up in the operating system, not in V-Control Pro.

=== "macOS"

    V-Control Pro runs in the menu bar and has no Dock icon, so add it from System Settings.

    To add it:

    * Open `System Settings / General / Login Items` (named `Login Items & Extensions` in macOS Sequoia and later).
    * Under `Open at Login`, click the `+` button.
    * Select `V-Control Pro` in the `Applications` folder and click `Open`.

    To remove it:

    * Select `V-Control Pro` in the `Open at Login` list.
    * Click the `-` button.

=== "Windows"

    To add it:

    * Press `Windows` + `R`, type `shell:startup`, and press `Enter`. The Startup folder opens.
    * Right-click `V-Control Pro` in the Start menu and select `Open file location`.
    * Right-click the V-Control Pro shortcut, drag it into the Startup folder, and select `Create shortcuts here`.

    To remove it:

    * Press `Windows` + `R`, type `shell:startup`, and press `Enter`.
    * Delete the V-Control Pro shortcut.

    You can also turn it off in `Task Manager / Startup apps`.

!!! warning "Use Version 3.3 Or Later For Launch At Login"
    Earlier versions could fail to launch, or start up unlicensed, when set to open at login. If you see this, see [V-Control Pro Won't Launch](./troubleshooting.md#macos-troubleshooting).
