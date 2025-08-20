#

### ProControl Mixbus

=== "Channel Strips"

    | Channel Strips |  |
    |---|---|
    | Record | Arms the assigned audio track of the Channel. |
    | Solo | Solos the Channel |
    | Mute | Mutes the Channel |
    | Select | Sets the Channel to the Select state. |
    | EQ | Assigns EQ editor to knobs for the selected track. |
    | DYN | Assigns DYN editor to knobs for the selected track. |
    | In/Sends | Assigns Sends to knobs for the selected track. |
    | Knob | Changes the assigned parameter. |
    | Knob Button | Sets assigned parameter to default value |
    |  | When in Plug-In Mode, selects plug-in to edit. |
    | Track Meters | Displays metering for tracks. Currenlty supports one meter per channel. |

=== "Bank Mode"

    | Bank Mode |  |
    |---|---|
    | The assignment buttons are used to assign controls to the Knobs. |  |
    | Pan (Default) | Shows the track names in the LED strip and assigns Knobs to Channel Pan. |
    | Send A,B,C,D,E | Assigns Knobs to Sends for selected track. |
    |  | Use the knob button to toggle the send off/on |
    | Input, Output | Assigns track parameters to the knobs for the selected track. |
    |  | Trim gain, Monitor Mode, Solo Isolate, Solo Safe, and Phase are available to edit in this mode. |
    | Flip | Flips knob assignment to faders. |
    | Master Faders | Toggles last Channel Fader to be Master Fader |

=== "Transport"

    | Transport |  |
    |---|---|
    | Play | Starts playhead at current position in Timeline. |
    | Stop | Stops playhead at current position in Timeline. (Press twice to Return to Zero) |
    | Record | Starts Record Mode for playhead |
    | Rewind | Move playhead backwards in Timeline. |
    | Fast Forward | Moves playhead forward in Timeline. |
    | RTZ | Go to Start of Session. |
    | GTE | Go to End of Session. |
    | Loop Play | Start Looped Playback. |
    | Loop Rec | Punch In |
    | Punch | Punch Out |
    | In | Mark In |
    | Out | Mark Out |
    | Audition | Sets Loop from selection |
    | Pre Roll | Sets Punch from selection |
    | Post Roll | Sets Session Start/End from selection |
    | Ext Trans | Toggles Click |
    | Counter Mode Select | Toggles Counter Display |
    | Counter | Displays Counter for current session. Counter mode can be changed in DAW. |

=== "Automation"

    | Automation |  |
    |---|---|
    | The automation buttons control automation for the selected track |  |
    | Read | Enables Play Automation for the selected track. |
    | Write | Enables Write Automation for the selected track. |
    | Touch | Enables Touch Automation for the selected track. |
    | Off | Enables Off/Manual Automation for the selected track. |

=== "DSP Edit Buttons"

    | DSP Edit Buttons |  |
    |---|---|
    | The DSP Edit buttons change which tracks are in view. |  |
    | Assign 1 | Shows only MIDI tracks. Press again to return to default Mixer view. |
    | Assign 2 | Shows only Audio tracks. Press again to return to default Mixer view. |
    | Assign 3 | Shows only Busses. Press again to return to default Mixer view. |
    | Assign 4 | Shows only Aux tracks. Press again to return to default Mixer view. |
    | Assign 5 | Shows user selected tracks. Press again to return to default Mixer view. |

=== "Navigation"

    | Navigation |  |
    |---|---|
    | Bank Left | Banks tracks left/Scrolls 1 track left in Nudge mode |
    | Bank Right | Banks tracks right/Scrolls 1 track right in Nudge mode |
    | Nudge | Toggles Nudge mode On/Off |
    | The cursor buttons operate in several modes. |  |
    | Zoom | Press once to enable Zoom Mode |
    |  | Press twice to enable Navigation Mode. |
    |  | Press three times to return to normal mode. |
    | Up | Zooms in Vertically when zoom mode is active. |
    |  | Deletes marker at playhead when Navigation mode is active. |
    | Down | Zooms out Vertically when zoom mode is active. |
    |  | Creates Marker  at playhead when Navigation mode is active. |
    | Left | Zooms out Horizontally when zoom mode is active. |
    |  | Moves to Previous marker when Navigation mode is active. |
    | Right | Zooms in Horizontally when zoom mode is active. |
    |  | Moves to Next Marker when Navigation mode is active. |

=== "Utility"

    | Utility |  |
    |---|---|
    | Undo | Press to undo the last edit. |
    | Shift+Undo | Press to redo edit. |
    | Save | Saves Session |
    | Enter | Acts as Enter key. |
    | Escape | Acts as ESC key. |
    | F3 | Select All Tracks. |
    | F4 | Deselect All Tracks. |

=== "Matrix Buttons"

    | Matrix Buttons |  |
    |---|---|
    | Use the Function Keys editor in the MixBus Mackie Control Protocol Settings Window to assign commands |  |
    | Go To | Enables Marker Mode for the cursor arrows. |
    | Matrix Button 1 | F1 |
    | Matrix Button 2 | F2 |
    | Matrix Button 3 | F3 |
    | Matrix Button 4 | F4 |
    | Matrix Button 5 | F5 |
    | Matrix Button 6 | F6 |
    | Matrix Button 7 | F7 |
    | Matrix Button 8 | F8 |

=== "V-Window Mode"

    | V-Window Mode |  |
    |---|---|
    | With the V-Window feature, users can instantly control any plug-ins or controls on screen through their control surface's channel strip with a touch of a button. |  |
    | Master Fader | Press once to enable Master Fader control. Press a second time to enable V-Window mode for the 8th channel fader. Press a 3rd time to cycle back to basic channel control. |
    | Mute | While in V-Window mode, the Mute button on the last channel strip will cycle through the various V-Window Modes which are listed below: |
    |  | VButton: Use this mode to interact with button controls. The mouse will stay in its place and activate a button press when the fader is touched. |
    |  | VButtonSet: Use this mode to create and cycle through different button set points. With the mouse hovering above the on screen button's position press Shift+Solo on the control surface to set a Pin at that location. Using the fader in this mode will cylce between multiple Pins to use with VButton mode. |
    |  | VWKnob: Use this mode when interacting with knob controls on the plug-ins GUI. |
    |  | VWHSlider: Use this mode when interacting with horizontal slider controls on the plug-ins GUI. |
    |  | VWVSlider: Use this mode when interacting with vertically slider controls on the plug-ins GUI. |
    | Solo | While in V-Window Mode, pressing the Solo button will pin the mouse location and revert to that location any time the fader is touched. Once the fader is released, the mouse is also returned to that pin position. This way it is very easy to pin a parameter and instantly control it without having to worry with the mouse cursor is on the screen. |
    | Select | Use the Select button while in V-Window mode to reset the fader position. |

=== "MIDI Mode"

    | MIDI Mode |  |
    |---|---|
    | MIDI Mode converts the surfaces faders, knobs, and buttons into assignable MIDI Controls that can be mapped in the DAW. |  |
    | Mon/0 | Toggles surface between DAW Mode and Midi Mode |