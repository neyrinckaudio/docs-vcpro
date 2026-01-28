#

### C24 - Pro Tools

!!! info "Important HUI Metering Information"
    The HUI protocol provides for stereo track metering. It does not provide for output metering. Pro Tools will not provide track metering if Eucon is enabled. Disable Eucon for track metering.

!!! info "Important Insert Editing Information"
    Pro Tools limits HUI device plug-in editing to the first eight channels of the surface. You can bank and scroll a track to the first eight channels and select a plug-in to edit. Thereafter, you can bank and scroll while editing the plug-in. 

=== "Channel Strips"

    | Channel Strip |  |  |
    |---|---|---|
    | `Record` |  | Arms the assigned audio track of the Channel (LED flashes when record-ready, lit when recording). |
    |  | `Option`+ | Record-enables all tracks (when pressed on non-enabled track). |
    |  | `Option`+ | Disables all tracks for recording (when pressed on enabled track). |
    |  | `Option`+`Shift`+ | Record-enables selected tracks only. |
    |  | `Alt`+ | Enables or clears Record Safe mode on channel (LED flashes briefly). |
    |  | `Option`+`Alt`+ | Enables or clears Record Safe on all channels. |
    |  | `Shift`+`Option`+`Alt`+ | Enables or clears Record Safe on selected channels only. |
    | `Insert` |  | Enables insert editor for selected Channel. |
    |  | Double-click | Directly accesses first assigned insert for editing. |
    |  | Multiple double-clicks | Cycles through inserts on channel. |
    |  | `Bypass`+ | Bypasses or enables all plug-ins on all inserts for channel (when Bypass mode enabled). |
    |  | `Bypass`+`Option`+ | Bypasses plug-ins on all channels (when Bypass mode enabled). |
    | `Solo` |  | Solos the Channel (LED lights when enabled). |
    |  | `Option`+ | Enables or clears solos on all channels. |
    |  | `Option`+`Shift`+ | Enables or clears solos on all selected channels. |
    |  | `Alt`+ | Enables or clears Solo Safe mode on channel (LED flashes briefly). |
    |  | `Option`+`Alt`+ | Enables or clears Solo Safe on all channels. |
    |  | `Shift`+`Option`+`Alt`+ | Enables or clears Solo Safe on selected channels only. |
    | `Mute` |  | Mutes the Channel (LED lights when enabled). |
    |  | `Option`+ | Enables or clears mutes on all channels. |
    |  | `Option`+`Shift`+ | Enables or clears mutes on all selected channels. |
    | `Auto` |  | Press to see auto mode displayed in place of track name. |
    |  | +`AUTOMATION MODES` | Hold down and select automation mode (WRITE, TOUCH, LATCH, TRIM, READ, OFF). |
    |  | +`Select` | Hold down and press channel select button to cycle through automation modes. |
    |  | `Option`+`Automation mode` | Changes automation mode on all channels. |
    |  | `Option`+`Shift`+`Automation mode` | Changes automation mode on all selected channels. |
    | `Select` |  | Selects track (LED lights when selected). |
    |  |  | Multiple SELECT presses: Selects multiple channels. |
    |  | `Shift`+ | Deselects single channel OR selects/deselects multiple channels. |
    |  | `Option`+ | Selects or deselects all channels. |
    |  | `Alt`+ | Changes SELECT state of channel and changes all others to opposite state (on lit switch). |
    |  | `Default`+ | Reset fader to 0 db. |
    |  | `Default`+`Option`+ | Reset all faders to 0 db. |
    |  | `Default`+`Option`+`Shift`+ | Reset all selected faders to 0 db. |
    | `Knob` |  | Adjust control assigned for bank mode. |
    | |  | Pan Mode - Adjust stereo pan for mono and stereo tracks. |
    | |  | Send A-E Modes - Adjust send volume. |
    | |  | Flip Send A-E Modes - Adjust send pan for mono/stereo sends.  |
    | |  | Insert Edit Mode - Adjust plugin parameter for strips 1-8. |
    | | `Cmd`+ | Fine mode (fine adjustments). |
    | | `Alt`+ | Fine adjustments for V-POT controls. |
    | `Knob Button` | `Default`+ | Pan Mode - Reset pan to default |
    | |  | Send Mute Mode - Control send mute |
    | |  | Pre/Post Mode - Control send pre/post. |
    | |  | Insert Select Mode - Select insert A-D, E for strips 1-4. |
    | |  | Insert Edit Mode - Adjust discrete parameter for strips 1-4. |
    |  | `Option`+ | Toggles send pre/post for all channels (in Send mode). |
    |  | `Option`+`Shift`+ | Toggles send pre/post for all selected channels (in Send mode). |
    |  | `Default`+ | Returns channel's send level or pan to default. |
    |  | `Default`+`Option`+ | Returns all channel send levels/pans to default. |
    |  | `Default`+`Option`+`Shift`+ | Returns all selected channel send levels/pans to default. |
    | `Fader` |  | Track volume control. |
    |  | `Alt`+ | Displays level in dB on scribble strip (while moving fader). |
    |  | `Ctrl`+ | Clutch mode - disengages faders from Mix groups while held. |
    | `Meters` |  | Displays stereo metering for tracks. |

=== "Bank Modes"

    Buttons are used to set a bank mode which assign controls to the Knobs.

    | `PAN` |  |
    |---|---|
    | `LCR`,`FrontRear`,`Rear`,`Divergence`,`Center`,`LFE`,`LR` | Stereo Pan Mode for mono / stereo tracks |
    | Toggle between Pan L and Pan R for stereo tracks | |
    | Toggle between Pan L and Pan R for stereo sends when in send mode | |
 
    | `SENDS` |  |
    |---|---|
    | `A` | Send A Mode |
    | `B` | Send B Mode |
    | `C` | Send C Mode |
    | `D` | Send D Mode |
    | `E` | Send E Mode |
 

     | `Flip` |  | 
    |---|---|
    | Flip send volume to faders, send pan to knobs. | |


    | `SWITCH FUNCTIONS` |  |
    |---|---|
    | `Pre/Post` | Sets knob buttons to Pre/Post mode when in Sends Mode. |
    | `Send Mute` | Sets knob buttons to Send Mute mode when in Sends Mode. |   

    | `ASSIGN` |  |
    |---|---|
    | `Input` | Shows Channel Inputs across LCD when held down. Enter Assign mode first to change channel input with knobs. |
    | `Output` | Shows Channel Outputs across LCD. Enter Assign mode first to change channel output with knobs. |

=== "Automation"

    | `AUTOMATION MODES` |  |
    |---|---|
    |  | Hold down channel strip `Auto` button to select automation modes. |
    | `Read` | Sets selected Channel in to Read Mode |
    | `Write` | Sets selected Channel to Write Mode |
    | `Touch` | Sets selected Channel to Touch Mode |
    | `Trim` | Enables Trim to selected Channel. |
    | `Latch` | Sets selected Channel to Latch Mode |
    | `Off` | Sets selected Channel to Off Mode |

    | `AUTO ENABLES` |  |
    |---|---|
    | `Volume` | Toggles Enable for Volume Automation |
    | `Pan` | Toggles Enable for Pan Automation |
    | `Mute` | Toggles Enable for Mute Automation |
    | `Send LvL` | Toggles Enable for Send Level Automation |
    | `Plug-In` | Toggles Enable for Plug-In Automation |


    | `AUTO WRITE TO` |  |
    |---|---|
    | `Start` | Enable Write to Start Automation. |
    | `End` | Enable Write to End Automation. |
    | `All` | Enable Write to All Automation. |

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
    | Pre Roll | Enables Pre Roll |
    | Post Roll | Enables Post Roll |
    | Mark In | Sets start point of selection in Timeline. |
    | Mark Out | Sets end point of selection in Timeline. |
    | Loop Play | Enables Loop playback. |
    | Loop Record | Enables Loop Record. |
    | Quick Punch | Enables Punch Mode. |
    | Audition | Enables Audition Mode. |
    | Online | Enables Online Mode for transport. |
    | Scrub | Enables Scrub Mode for the Wheel |
    | Shuttle | Enables Shuttle Mode for the Wheel |
    | Counter | Displays Counter for current session. Counter mode can be changed in DAW. |
    | Master Record | Record Enables all available channels. |

=== "PlugIn Editing"

    | Channel Strip |  |  |
    |---|---|---|
    | `Insert` |  | Normal Mode - Assign track to insert editor |
    |   |  | Insert Bypass Mode - Bypass all inserts on track |

    | `Insert Bypass` |  |
    |---|---|
    |  Toggle Insert Bypass Mode. When enabled, `Insert` button on strip will bypass all plugins on track. |    
 
    | `INSERTS` |  |
    |---|---|
    | Params | Toggle to switch between Insert Select mode and Insert Edit mode. |
    | Master Bypass | Bypass selected plug-in on track. |
    | Compare | Compares current plug-in setting with previous. |

    | `CHANNEL BAR SCROLL` |  |
    |---|---|
    | Left | Previous page of plug-in parameters. |
    | Right | Next page of plug-in parameters. |



=== "Group Buttons"

    | Group Buttons |  |
    |---|---|
    | Create | Creates group of selected tracks. |
    | Suspend | Suspends Group function. |
    | Status | Displays Group Assignment. |

=== "Utility"

    | Utility |  |
    |---|---|
    | Save | Press the Save button to save. |
    |  | Press Shift + Save button to open the Save As dialog. |
    | Undo | Press to undo the last edit. |
    | Cancel | Cancel selection |
    | Solo Clear | Clears all Solos on Channel Strip. |

=== "Navigation"

    | Navigation |  |
    |---|---|
    | Bank Left | Banks tracks left/Scrolls 1 track left in Nudge mode |
    | Bank Right | Banks tracks right/Scrolls 1 track right in Nudge mode |
    | Nudge | Toggles Nudge mode On/Off |
    | Up | Scrolls Up in Edit Window. |
    | Down | Scrolls Down in Edit Window. |
    | Left | Scrolls Left in Edit Window. |
    | Right | Scrolls Right in Edit Window. |
    | Zoom | Enables Zoom mode for the cursor keys. Left/Right zooms horizontal for the Edit window. Up/Down zooms vertical for the Edit window. |

=== "Window Buttons"

    | Window Buttons |  |
    |---|---|
    | Mix | Displays Mixer Window. |
    | Edit | Displays Edit Window. |
    | MemLoc | Displays Marker Window. |
    | Transport | Displays Transport Window. |
    | Plug-In | Displays Plug-In Window. |
    | Status | Displays Setup Window. |

=== "Edit"

    | Edit |  |
    |---|---|
    | Copy | Copy selected region in Edit Window. |
    | Delete | Deletes selected region in Edit Window. |
    | Cut | Cuts selected region in Edit Window. |
    | Paste | Pastes region in Edit Window. |
    | Capture | Captures selected region. |
    | Separate | Separates region at playhead. |
    | Shuffle | Enables Shuffle Mode in Edit Window. |
    | Slip | Enables Slip Mode in Edit Window. |
    | Spot | Enables Spot Mode in Edit Window. |
    | Grid | Enables Grid Mode in Edit Window. |
    | Trim | Enables Trim Tool in Edit Window. |
    | Select | Enables Select Tool in Edit Window. |
    | Grab | Enables Grab Tool in Edit Window. |
    | Pencil | Enables Pencil Tool in Edit Window. |

=== "V-Window Mode"

    | V-Window Mode |  |
    |---|---|
    | With the V-Window feature, users can instantly control any plug-ins or controls on screen through their control surface's channel strip with a touch of a button. |  |
    | Master Fader | Press once to enable V-Window mode for the 24th channel fader. Press a 2nd time to cycle back to basic channel control. |
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
    | Focus | Toggles surface between DAW Mode and MIDI Mode |
