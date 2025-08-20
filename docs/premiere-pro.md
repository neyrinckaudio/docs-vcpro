# Premiere Pro 

* In the Premiere Pro top menu bar select: Premiere Pro/Preferences/Control Surface...
* Select Add for new Device Class
* Select Device Class: Mackie
* Select Settings... to open Device Class settings window
* Select Mackie in the settings window and select Edit
* Configure Mackie Control as the following:
    * Device Type: Mackie Control
    * MIDI Input Device: V-Control
    * MIDI Output Device: V-Control

Here is how to setup additional controllers for up to 32 tracks of control simultaneously.

In the Configure Mackie Controller window, click on Add and set up as:

* Device Type: Mackie Control XT
* MIDI Input Device: V-Control XT2
* MIDI Output Device: V-Control XT2
* Repeat this step replacing V-Control XT2 with V-Control XT3 and V-Control XT4 for 32 tracks total.

!!! note
    Some commands need to be manually mapped in Premiere Pro CC for full use. Go into the Button Assignments window in the Control Surface setup and assign the following:

- Button: Flip - Command: Go To Previous Edit Point
- Button: SMPTE/Beats - Command: Go To Next Edit Point
- Button: Cycle - Command: cmd.audiomixer.loop

!!! note
    For the Channel/Bank select buttons to work, there must be more audio tracks created in the current session than the number of tracks that are controlled by V-Control Pro. For example, if setup for 16 tracks of control, there must be at least 17 created audio tracks in Premiere for the Channel/bank select buttons to function.

