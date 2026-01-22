#

### D-Command - Pro Tools

!!! info "Important HUI Metering Information"
    The HUI protocol provides for stereo track metering. It does not provide for output metering.

!!! info "Important Insert Editing Information"
    Pro Tools limits HUI device plug-in editing to the first eight channels of the surface. You can bank and scroll a track to the first eight channels and select a plug-in to edit. Thereafter, you can bank and scroll while editing the plug-in. 

=== "Channel Strips"

    | Channel Strips |  |
    |---|---|
    | Record | Arms the assigned audio track of the Channel. |
    | Select | Sets the Channel to the Select state. |
    | Solo | Solos the Channel. |
    | Mute | Mutes the Channel. |
    | Auto | Hold down and press a channel select button to cycle through Automation modes for the selected channel. |
    | Track Meters | Displays Stereo metering for tracks. |
    | Pan | Assigns pan control to the knobs for all tracks. Press again to toggle to right channel pan for stereo tracks. |
    | Sends | Assigns Send Mode to bottom edit row for all tracks. Press and hold to display send destination. |
    | Page Up | Cycles through Send A-E assignment. |
    | Page Down | Cycles through Send A-E assignment. |
    | BypMute | Toggles between Send Mute Mode and Send Pre/Post Mode |
    | Inserts | Assign track to upper edit row insert editor. Press again to toggle between Insert Select Mode and Insert Edit Mode |

    | Lower Edit Row | Edit Pan and Sends |
    |---|---|
    | Knob | Adjust track pan, send volume, or send pan for stereo sends |
    | BMP | Send Mute Mode - toggle send mute |
    |  | Send Pre/Post Mode - toggle send pre/post. |
    | Flip | Flips send volume to Fader, send mute to Mute. |
    
    | Upper Edit Row | Edit Inserts A-E. Only available for tracks 1-8. |
    |---|---|
    |  | Insert Select Mode |
    | Select 1-4 | Select insert to edit |
    | Select 5 | Display inserts A-D |
    | Select 6 | Display insert E |
    |  | Insert Edit Mode |
    | Knob 1-8 | Adjust plugin parameter values |
    | Select 1-4 | Cycle through discrete parameter values |
    | Select 7 | Compare |
    | BMP 7 | Bypass |
    | Select 8 | Page Left |
    | BMP 8 | Page Right |
     
=== "Insert Edit"

    Use `Inserts` button on track to select a track to edit. Only available for tracks 1-8.

    | Upper Edit Row |  |
    |---|---|
    |  | Insert Select Mode |
    | `Select` 1-4 | Select insert to edit |
    | `Select` 5 | Display inserts A-D |
    | `Select` 6 | Display insert E |
    |  | Insert Edit Mode |
    | `Knob` 1-8 | Adjust plugin parameter values |
    | `Select` 1-4 | Cycle through discrete parameter values |
    | `Select` 7 | Compare |
    | `BMP` 7 | Bypass |
    | `Select` 8 | Page Left |
    | `BMP` 8 | Page Right |

=== "Automation"

    | Automation |  |
    |---|---|
    | Hold down the Automation Mode and press the channel select button to assign that mode to the channel. |  |
    | Write | Assigns Write mode to selected channel. |
    | Read | Assigns Read mode to selected channel. |
    | Touch | Assigns Touch mode to selected channel. |
    | Latch | Assigns Latch mode to selected channel. |
    | Off | Sets Automation mode to Off |
    | Auto Suspend | Suspends Automation |
    | There is no indication if Automation enables are On/Off |  |
    | Vol | Toggle Enable Volume Automation |
    | Pan | Toggle Enable Pan Automation |
    | Mute | Toggle Enable Mute Automation |
    | Sends | Toggle Enable Sends Automation |
    | EQ | Toggle Enable Send Mute Automation |
    | Plugin | Toggle Enable Plugin Automation |

=== "Transport"

    | Transport |  |
    |---|---|
    | Play | Starts playhead at current position in Timeline. |
    | Stop | Stops playhead at current position in Timeline. |
    | Record | Starts Record Mode for playhead |
    | Rewind | Move playhead backwards in Timeline. |
    | Fast Forward | Moves playhead forward in Timeline. |
    | RTZ | Returns playhead to beginning of Timeline. |
    | GTE | Sends playhead to end of Timeline. |
    | Mark In | Go To Left Locator |
    | Mark Out | Go To Right Locator |
    | Loop Play | Toggles Loop mode for loop selection in Timeline. |
    | Quick Punch | Toggles Punch mode for selection in Timeline. |
    | Counter | Displays Counter for current session. |

=== "Utility"

    | Utility |  |
    |---|---|
    | Save | Press the Save button to save. |
    |  | Press Shift + Save button to open the Save As dialog. |
    | Undo | Press to undo the last edit. |

=== "Window Buttons"

    | Window Buttons |  |
    |---|---|
    | Mix | Opens Mix Window |
    | Edit | Opens Edit Window |
    | Mem Loc | Opens Memory Locations Window |
    | Plug-in | Opens Plug-in Window for plugin selected in plugin editor |
    | Transport | Opens Transport Window |

=== "Navigation"

    | Navigation |  |
    |---|---|
    | Bank Left | Banks 8 tracks left. |
    | Bank Right | Banks 8 tracks right. |
    | Nudge Left | Scrolls 1 track left. |
    | Nudge Right | Scrolls 1 track right. |
    | Scrub | Enables Scrub mode for the wheel. |
    |  | Normal Mode - Use Shift at any time to adjust start or end of a selection with wheel. |
    |  | Edit Start Of Selection - Hold Shift and press Scrub. Use wheel to edit start of selection. |
    |  | Edit End Of Selection - Hold Shift+Option and press Scrub. Use wheel to edit end of selection. |
    | Shuttle | Enables Shuttle Mode for the wheel. |
    | Zoom | Enables Zoom mode for the cursor keys. |

=== "V-Window Mode"

    | V-Window Mode |  |
    |---|---|
    | With the V-Window feature, users can instantly control any plug-ins or controls on screen through their control surface's channel strip with a touch of a button. |  |
    | Master Fader | Press once to enable V-Window mode for the 8th channel fader. Press a 2nd time to cycle back to basic channel control. |
    | Mute | While in V-Window mode, the Mute button on the last channel strip will cycle through the various V-Window Modes which are listed below: |
    |  | VButton: Use this mode to interact with button controls. The mouse will stay in its place and activate a button press when the fader is touched. |
    |  | VButtonSet: Use this mode to create and cycle through different button set points. With the mouse hovering above the on screen button's position press Shift+Solo on the control surface to set a Pin at that location. Using the fader in this mode will cylce between multiple Pins to use with VButton mode. |
    |  | VWKnob: Use this mode when interacting with knob controls on the plug-ins GUI. |
    |  | VWHSlider: Use this mode when interacting with horizontal slider controls on the plug-ins GUI. |
    |  | VWVSlider: Use this mode when interacting with vertically slider controls on the plug-ins GUI. |
    | Solo | While in V-Window Mode, pressing the Solo button will pin the mouse location and revert to that location any time the fader is touched. Once the fader is released, the mouse is also returned to that pin position. This way it is very easy to pin a parameter and instantly control it without having to worry with the mouse cursor is on the screen. |
    | Select | Use the Select button while in V-Window mode to reset the fader position. |

=== "MIDI Mode"

    | MIDI Mode | V-Control MIDI Mode port connects surface as a MIDI controller |
    |---|---|
    | MIDI Events List | Toggles surface between DAW Mode and MIDI Mode |
    | EQ Section | All encoders are assigned to MIDI Mode |
    | Dyn Section | All encoders are assigned to MIDI Mode |
    | Top Row Encoders | All encoders are assigned to MIDI Mode |