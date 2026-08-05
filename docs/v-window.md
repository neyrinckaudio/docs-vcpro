# Using V-Window

V-Control Pro's V-Window feature helps view and remotely control parts of a DAW.

### Hardware Fader
* Remotely adjust a plug-in parameter with a hardware fader.

### iPad
* View a plug-in window on the iPad using V-Console.
* Remotely adjust a plug-in parameter with an iPad using V-Console.
* Focus on any window in the media application.

## macOS Privacy Permissions

V-Window works by moving the mouse pointer inside a plug-in window for you, and — for the iPad apps — by capturing a picture of that window and sending it to the iPad. macOS treats both of those as privacy-protected actions and blocks them until you allow them, so **V-Window will not work on macOS until V-Control Pro is granted permission**.

Grant these permissions to the **V-Control Pro** application, on the Mac that runs your DAW:

| Permission | Needed for |
|---|---|
| **Accessibility** | Remote mouse and keyboard control — required for all V-Window use, including a hardware fader |
| **Screen & System Audio Recording** (called **Screen Recording** before macOS Sequoia) | Viewing a plug-in window on the iPad with [V-Console](./v-console.md) or the legacy [V-Control Pro iPad App](./v-control-pro-ipad.md) |

!!! note "Windows"
    Windows has no equivalent permission. This setup applies to macOS only.

### Accessibility — Remote Mouse Control

When you move a fader or touch a control on the iPad, V-Control Pro moves the Mac's pointer and clicks inside the plug-in window on your behalf. macOS blocks one application from controlling another that way until you grant Accessibility permission.

**macOS Ventura, Sonoma, Sequoia, and newer:**

1. Open **System Settings** from the Apple menu or the Dock.
2. Click **Privacy & Security** in the left sidebar.
3. Scroll down and select **Accessibility** from the list on the right.
4. Locate **V-Control Pro** in the list and turn the switch **ON**.
5. If V-Control Pro isn't listed, click the **+** button at the bottom of the list, authenticate with your administrator password or Touch ID, and select **V-Control Pro** from your Applications folder.
6. Quit and relaunch V-Control Pro.

**macOS Monterey and earlier:**

1. Open **System Preferences → Security & Privacy** and click the **Privacy** tab.
2. Select **Accessibility** in the list on the left.
3. Click the lock at the bottom and authenticate.
4. Check the box next to **V-Control Pro**, adding it with **+** if it isn't listed.
5. Quit and relaunch V-Control Pro.

### Screen Recording — Viewing A Window On The iPad

To show a plug-in window on the iPad, V-Control Pro captures the picture of that window and streams it to the iPad app. Capturing any window belonging to another application requires screen recording permission.

**macOS Ventura, Sonoma, Sequoia, and newer:**

1. Open **System Settings → Privacy & Security**.
2. Click **Screen & System Audio Recording** (**Screen Recording** on macOS Sonoma and earlier).
3. Turn the switch **ON** for **V-Control Pro**, adding it with **+** if it isn't listed.
4. Relaunch V-Control Pro when prompted — the change does not take effect until it restarts.

**macOS Catalina through Monterey:**

1. Open **System Preferences → Security & Privacy** and click the **Privacy** tab.
2. Select **Screen Recording** in the list on the left.
3. Click the lock at the bottom and authenticate.
4. Check the box next to **V-Control Pro**.
5. Quit and relaunch V-Control Pro.

!!! note "macOS Mojave and earlier"
    Screen recording permission was introduced in macOS Catalina. Earlier versions do not need it.

This permission is only needed to see a window on the iPad. Controlling a plug-in parameter with a hardware fader needs Accessibility only.

### Verifying And Troubleshooting

V-Control Pro reports a missing permission itself the first time V-Window needs it. Use what you see to tell which permission is missing:

* **The iPad's list of applications shows "Privacy - Not Allowed"**, and V-Control Pro displays *"A V-Window device is trying to access the screen..."* — screen recording permission is missing.
* **The iPad shows an empty, black, or frozen V-Window** — screen recording permission is missing or was granted without relaunching V-Control Pro.
* **The window appears on the iPad, or a fader is moved, but nothing responds**, and V-Control Pro displays *"A V-Window device is trying to control your screen..."* — Accessibility permission is missing.
* **It worked before and stopped after an update** — macOS sometimes invalidates a permission when the application changes. Turn the switch **OFF** and back **ON** for V-Control Pro (or remove it with **−** and add it again with **+**), then relaunch.

!!! warning "Relaunch after granting permission"
    macOS applies screen recording permission only when the application launches, and V-Control Pro checks both permissions once per session. Always quit V-Control Pro completely and start it again after changing either switch — otherwise the setting looks correct in System Settings while V-Window still fails.
