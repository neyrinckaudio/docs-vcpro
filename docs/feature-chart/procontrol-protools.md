#

### ProControl - Pro Tools

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
    | `Auto` |  | Press to see auto mode. |
    |  | +`AUTOMATION MODES` | Hold down and select automation mode (WRITE, TOUCH, LATCH, TRIM, READ, OFF). |
    |  | +`Select` | Hold down and press channel select button to cycle through automation modes. |
    |  | `Option`+`Automation mode` | Changes automation mode on all channels. |
    |  | `Option`+`Shift`+`Automation mode` | Changes automation mode on all selected channels. |
    | `Select` |  | Selects track (LED lights when selected). |
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
    | | `Alt`+ | Fine adjustments for Knob controls. |
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
    |  | `Ctrl`+ | Clutch mode - disengages faders from Mix groups while held. |
    | `Master Record` |  | Toggles all enabled REC/RDY switches on and off. |
    | `Meters` |  | Displays stereo metering for tracks. |

=== "Bank Modes"

    Buttons are used to set a bank mode which assign controls to the Knobs.

    | `PAN` |  |  |
    |---|---|---|
    | `PAN` |  | Enables pan control on Knobs. |
    |  | Press twice | On stereo channels, edits right channel pan. |
    | `LCR`,`FrontRear`,`Rear`,`Divergence`,`Center`,`LFE`,`LR` |  | Stereo Pan Mode for mono / stereo tracks |
    |  |  | Toggle between Pan L and Pan R for stereo tracks |
    |  |  | Toggle between Pan L and Pan R for stereo sends when in send mode |

    | `SENDS` |  |  |
    |---|---|---|
    | `A` |  | Send A Mode - enables send level control on Knobs for Send A. |
    |  | `Assign`+ | Enters assign mode for send routing. |
    |  | `Insert`+ | Quick access to send level editing. |
    | `B` |  | Send B Mode - enables send level control on Knobs for Send B. |
    | `C` |  | Send C Mode - enables send level control on Knobs for Send C. |
    | `D` |  | Send D Mode - enables send level control on Knobs for Send D. |
    | `E` |  | Send E Mode - enables send level control on Knobs for Send E. |


    | `Flip` |  |  |
    |---|---|---|
    | `Flip` |  | Enters Flip mode (LED flashes). |
    |  |  | Send levels mapped to faders. |
    |  |  | Send pan controls mapped to Knobs. |
    |  |  | Send mutes mapped to MUTE switches. |
    |  |  | V-SEL controls send pre/post operation. |


    | `SWITCH FUNCTIONS` |  |  |
    |---|---|---|
    | `Pre/Post` |  | Sets knob buttons to Pre/Post mode when in Sends Mode. |
    | `Send Mute` |  | Sets knob buttons to Send Mute mode when in Sends Mode. |

    | `ASSIGN` |  |  |
    |---|---|---|
    | `Input` |  | Enters assign mode for input routing. |
    |  | `Assign`+ | Enters assign mode for input routing. |
    | `Output` |  | Enters assign mode for output routing. |
    |  | `Assign`+ | Enters assign mode for output routing. |
    |  | `Ctrl`+`Assign` | Confirms additional output assignment (during output assign). |

    | `INSERT BYPASS` |  |  |
    |---|---|---|
    | `Insert Bypass` |  | Enables Master Bypass mode (INSERT switches become bypass switches). |
    |  | +`Insert` | Toggles bypass for all plug-ins on channel (when Bypass mode enabled). |
    |  | +`Option`+`Insert` | Changes bypass status of all plug-ins on all channels (when Bypass mode enabled). |
    |  | +`Option`+`Shift`+`Insert` | Changes bypass status on all selected channels (when Bypass mode enabled). |

=== "Automation"

    | `AUTOMATION MODES` |  |  |
    |---|---|---|
    |  |  | Hold down channel strip `Auto` button to select automation modes. |
    | `Read` |  | Sets selected Channel to Read Mode (AUTO LED green). |
    |  | `Option`+ | Arms all channels for Read mode. |
    |  | `Option`+`Shift`+ | Arms all selected channels for Read mode. |
    | `Write` |  | Sets selected Channel to Write Mode (AUTO LED red flashing/lit). |
    |  | `Option`+ | Arms all channels for Write mode. |
    |  | `Option`+`Shift`+ | Arms all selected channels for Write mode. |
    | `Touch` |  | Sets selected Channel to Touch Mode (AUTO LED red flashing/lit). |
    |  | `Option`+ | Arms all channels for Touch mode. |
    |  | `Option`+`Shift`+ | Arms all selected channels for Touch mode. |
    | `Latch` |  | Sets selected Channel to Latch Mode (AUTO LED red flashing/lit). |
    |  | `Option`+ | Arms all channels for Latch mode. |
    |  | `Option`+`Shift`+ | Arms all selected channels for Latch mode. |
    | `Trim` |  | Toggles TRIM mode on/off for track (TDM only). |
    |  | `Alt`+ | Displays trim delta value instead of absolute value (while adjusting). |
    |  | `Option`+ | Arms all channels for Trim mode. |
    |  | `Option`+`Shift`+ | Arms all selected channels for Trim mode. |
    | `Off` |  | Disables automation on channel (AUTO LED off). |
    |  | `Option`+ | Disables automation on all channels. |
    |  | `Option`+`Shift`+ | Disables automation on all selected channels. |

    | `AUTO ENABLES` |  |  |
    |---|---|---|
    | `Volume` |  | Enables automation for fader. |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes FADER state and sets other five to opposite. |
    | `Pan` |  | Enables automation for pan (enables both channel and send pan if both disabled). |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes PAN state and sets other five to opposite. |
    | `Mute` |  | Enables automation for mute. |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes MUTE state and sets other five to opposite. |
    | `Send LvL` |  | Enables automation for send. |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes SEND state and sets other five to opposite. |
    | `Plug-In` |  | Enables automation for plug-ins. |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes PLUG IN state and sets other five to opposite. |
    | `Send Mute` |  | Enables automation for send mute. |
    |  | `Option`+ | Toggles all automation parameters to this state. |
    |  | `Alt`+ | Changes SEND MUTE state and sets other five to opposite. |

=== "Transport"

    | Transport |  |  |
    |---|---|---|
    | `Play` |  | Begins playback from current cursor position. |
    |  | `Shift`+ | Initiates half-speed playback. |
    | `Stop` |  | Stops playback or recording. |
    |  | `Shift`+ | Aborts the current record pass. |
    | `Record` |  | Arms Pro Tools for recording (LED flashes). |
    |  | `Ctrl`+ | Cycles through record modes (normal, QuickPunch, Loop). |
    | `Rewind` |  | Rewinds the session from current cursor position (incremental or continuous depending on preferences). |
    |  | `Shift`+ | Return-to-Zero (same as RTZ button). |
    | `Fast Forward` |  | Fast-forwards the session from current cursor position (incremental or continuous). |
    |  | `Shift`+ | Go-To-End (same as END button). |
    | `RTZ` |  | Sets playback cursor to the beginning of the session. |
    |  | `Ctrl`+ | Write to Start (writes automation from insertion point backward to beginning). |
    |  | `Ctrl`+`Shift`+ | Write to All (writes automation to entire selection/track). |
    |  | `Ctrl`+`Option`+ | Suppresses warning dialog for Write to Start. |
    | `GTE` |  | Sets playback cursor to the end of the session. |
    |  | `Ctrl`+ | Write to End (writes automation from insertion point forward to end). |
    |  | `Ctrl`+`Shift`+ | Write to All (writes automation to entire selection/track). |
    |  | `Ctrl`+`Option`+ | Suppresses warning dialog for Write to End. |
    | `Pre Roll` |  | Activates pre-roll. |
    |  | `Alt`+ | Enters pre-roll time value (numeric entry mode). |
    | `Post Roll` |  | Activates post-roll. |
    |  | `Alt`+ | Enters post-roll time value (numeric entry mode). |
    | `Mark In` |  | Marks In edit point during playback / Sets start point of selection in Timeline. |
    |  | `Alt`+ | Manually enters selection start time. |
    |  | `Option`+Left Arrow | Centers left side of waveform selection in Edit Window. |
    | `Mark Out` |  | Marks Out edit point during playback / Sets end point of selection in Timeline. |
    |  | `Alt`+ | Manually enters selection end time. |
    |  | `Option`+Right Arrow | Centers right side of waveform selection in Edit Window. |
    | `Loop Play` |  | Toggles Loop Playback mode (LED lit when enabled). |
    |  | `Ctrl`+ | Places Pro Tools into Loop Record mode. |
    | `Loop Record` |  | Enables Loop Record. |
    | `Quick Punch` |  | Toggles QuickPunch recording mode (LED lit when enabled). |
    | `Audition` |  | Press with PRE/POST/IN/OUT to play audio; playback continues until pressed again. |
    |  | `Alt`+`Option`+PRE | Plays audio from pre-roll point through selection start plus post-roll. |
    |  | `Alt`+`Option`+IN | Plays audio from pre-roll point through selection start plus post-roll. |
    |  | `Alt`+`Option`+OUT | Plays audio from before selection end (pre-roll) through selection end plus post-roll. |
    |  | `Alt`+`Option`+POST | Plays audio from before selection end (pre-roll) through selection end plus post-roll. |
    | `Online` |  | Places Pro Tools online or offline (LED lit when online). |
    |  | `Ctrl`+ | Cycles through available machine master choices (Pro Tools, Serial Machine, ADAT). |
    | `Scrub` |  | Enables Scrub mode (rotate wheel to scrub forward/backward). |
    |  | `Option`+ | Begins scrubbing from selection end point. |
    |  | `Alt`+ | Fixed "fine scrub" resolution regardless of zoom level (while scrubbing). |
    |  | `Shift`+ | Creates selection using scrub wheel (starts at current position). |
    |  | `Shift`+`Option`+ | Modifies end of existing selection. |
    |  | Left/Right Arrow | Moves to selection start/end (during scrub). |
    | `Shuttle` |  | Enables Shuttle mode (rotate wheel to shuttle forward/backward). |
    |  | `Option`+ | Begins shuttling from selection end point. |
    |  | `Shift`+ | Creates selection using shuttle wheel. |
    |  | `Shift`+`Option`+ | Modifies end of existing selection. |
    |  | Left/Right Arrow | Moves to selection start/end (during shuttle). |
    | `Counter` |  | Displays Counter for current session. Counter mode can be changed in DAW. |

=== "DSP Edit"

    | DSP Edit |  |  |
    |---|---|---|
    | `Insert/Params` |  | Toggles between Insert Display mode and Parameter mode. |
    | `Assign 1-8` |  | Enables Assign for Inserts A-E. Use knobs in DSP Edit section to change selection. |
    | `Select 1-8` |  | Selects Insert A-E for editing. Toggles insert parameters. |
    | `Bypass 1-8` |  | Bypasses Inserts A-E. |
    | `Compare` |  | Compares current plug-in setting with previous (must have plug-in visible on-screen). |
    |  | `Default`+ | Returns plug-in to factory/user default setting. |
    | `Master Bypass` |  | Bypass selected plug-in on track. |
    |  |  | In Parameter mode: Engages Master Bypass for selected plug-in (LED lights). |

=== "Matrix"

    | Channel Matrix |  |  |
    |---|---|---|
    | Goto |  | Enables Marker Mode for Channel Matrix. Use Matrix 1-32 to jump to marker points. |
    | 1/A |  | Use to scroll through pages for insert parameters. |
    | 2/B |  | Use to scroll through pages for insert parameters. |

    | Status |  |  |
    |---|---|---|
    | The Status buttons change the assignment for the Channel Matrix. |  |  |
    | Select |  | Assigns the channel matrix buttons to Channel Strip select. |
    | Mute |  | Assigns the channel matrix buttons to Channel strip mute. |
    | Solo |  | Assigns the channel matrix buttons to Channel Strip solo. |
    | Rec/Rdy |  | Assigns the channel matrix buttons to Channel Strip Record Arm. |
    | Param/Pages |  | Assigns the channel matrix buttons 1 and 2 to scroll through insert parameter pages. |

=== "Group"

    | Group Buttons |  |  |
    |---|---|---|
    | `Create` |  | Creates group from selected channels (use `Shift`+`Select` on multiple channels first). |
    | `Suspend` |  | Suspends all Mix groups temporarily (LED flashes when enabled). |
    | `Status` |  | Shows Group ID status. |
    | `Select` |  | Switches the DSP Section from DAW Mode to MIDI Mode. |

=== "Utility"

    | Utility |  |  |
    |---|---|---|
    | `Save` |  | Press once to arm save, press again to complete save (LED flashes when armed). |
    |  | `Shift`+ | Opens Save As dialog. |
    |  | F8/ESC | Aborts the save process. |
    | `Undo` |  | Undo or Redo last edit operation (LED lit when Undo available, flashes when Redo available). |
    | `Cancel` |  | Cancel selection / Serves as Escape to cancel any assignment mode or on-screen modal dialog. |
    | `Solo Clear` |  | Clears all Solos on Channel Strip. |

=== "Keypad"

    | Keypad Buttons |  |  |
    |---|---|---|
    | 0 |  | Start/Stop Playback |
    | 1 |  | Rewind |
    | 2 |  | Fast Forward |
    | 3 |  | Record Enable |
    | 4 |  | Loop Playback |
    | 5 |  | Loop Record |
    | 6 |  | Quick Punch |
    | 7 |  | Click |
    | 8 |  | Count Off |
    | 9 |  | MIDI Merge |
    | . |  | Inputs Decimal Point |
    | + |  | Inputs Plus sign |
    | - |  | Inputs Subtract |
    | * |  | Inputs Asterisk |
    | / |  | Inputs Divide |
    | Enter |  | Creates Marker at current position |
    | Clr |  | Clear numerical input. |

=== "Navigation"

    | Navigation |  |  |
    |---|---|---|
    | `Bank Left` |  | Swaps channels left eight at a time. |
    |  | `Option`+ | Banks to far-left position in session. |
    | `Bank Right` |  | Swaps channels right eight at a time. |
    |  | `Option`+ | Banks to far-right position in session. |
    | `Channel Left` |  | Scrolls channels left one at a time. |
    |  | `Option`+ | Scrolls to far-left position. |
    | `Channel Right` |  | Scrolls channels right one at a time. |
    |  | `Option`+ | Scrolls to far-right position. |
    | `Nudge` |  | Toggles Nudge mode On/Off (Bank Left/Right scroll 1 track when enabled). |
    | `Zoom` |  | Cycles through three modes: Navigation (LED off), Zoom (LED lit), Selection (LED flashing). |
    |  |  | **Navigation Mode (LED off):** |
    | `Up` |  | Moves edit cursor or selection to previous track (marks in/out). |
    |  | `Shift`+ | Extends edit selection to previous track. |
    |  | `Alt`+ | Scrolls frontmost window upward. |
    |  | `Alt`+`Option`+ | Scrolls to top of session (Edit window). |
    | `Down` |  | Moves edit cursor or selection to next track (marks in/out). |
    |  | `Shift`+ | Extends edit selection to next track. |
    |  | `Alt`+ | Scrolls frontmost window downward. |
    |  | `Alt`+`Option`+ | Scrolls to bottom of session (Edit window). |
    | `Left` |  | Moves edit cursor to previous region boundary or sync point. |
    |  | `Shift`+ | Extends selection to preceding region boundary. |
    |  | `Option`+ | Centers left side of waveform selection in Edit Window. |
    |  | `Alt`+ | Scrolls frontmost window to the left (one page). |
    |  | `Alt`+`Option`+ | Scrolls to beginning of session (Edit window). |
    |  | `Ctrl`+ | Selects previous region. |
    |  | `Ctrl`+`Shift`+ | Extends selection to include previous region. |
    | `Right` |  | Moves edit cursor to next region boundary or sync point. |
    |  | `Shift`+ | Extends selection to forward region boundary. |
    |  | `Option`+ | Centers right side of waveform selection in Edit Window. |
    |  | `Alt`+ | Scrolls frontmost window to the right (one page). |
    |  | `Alt`+`Option`+ | Scrolls to end of session (Edit window). |
    |  | `Ctrl`+ | Selects next region. |
    |  | `Ctrl`+`Shift`+ | Extends selection to include next region. |
    |  |  | **Zoom Mode (LED lit):** |
    | `Left` |  | Decreases horizontal zoom. |
    | `Right` |  | Increases horizontal zoom. |
    | `Up` |  | Increases vertical zoom. |
    | `Down` |  | Decreases vertical zoom. |
    |  |  | **Selection Mode (LED flashing):** |
    | `Left` |  | Adjusts selection in-point with Scrub/Shuttle wheel. |
    |  | Double-click | Positions cursor at selection's left edge. |
    |  | +`Right`+Wheel | Adjusts selection time position while retaining duration. |
    | `Right` |  | Adjusts selection out-point with Scrub/Shuttle wheel. |
    |  | Double-click | Positions cursor at selection's right edge. |
    |  | +`Left`+Wheel | Adjusts selection time position while retaining duration. |
    | `Up` |  | Moves selection to previous track. |
    |  | `Shift`+ | Extends selection to previous track. |
    |  | `Option`+ | Removes selection from topmost track. |
    | `Down` |  | Moves selection to next track. |
    |  | `Shift`+ | Extends selection to next track. |
    |  | `Option`+ | Removes selection from bottommost track. |

=== "Window"

    | Window Buttons |  |  |
    |---|---|---|
    | `Mix` |  | Brings Mix window to foreground (LED lights when active). |
    | `Edit` |  | Brings Edit window to foreground (LED lights when active). |
    | `MemLoc` |  | Opens or closes the Memory Locations window. |
    | `Transport` |  | Opens or closes the Transport window. |
    | `Plug-In` |  | Opens or closes the floating window for currently selected plug-in. |
    | `Status` |  | Opens or closes the Session Setup window. |

=== "Edit"

    | Edit |  |  |
    |---|---|---|
    | `Copy` |  | Copy selected region in Edit Window. |
    | `Delete` |  | Deletes selected region in Edit Window. |
    | `Cut` |  | Cuts selected region in Edit Window. |
    | `Paste` |  | Pastes region in Edit Window. |
    | `Capture` |  | Executes capture region function. |
    | `Separate` |  | Executes separate region function / Separates region at playhead. |
    | `Shuffle` |  | Enables Shuffle Mode in Edit Window. |
    | `Slip` |  | Enables Slip Mode in Edit Window. |
    | `Spot` |  | Enables Spot Mode in Edit Window. |
    | `Grid` |  | Enables Grid Mode in Edit Window. |
    | `Edit Mode` |  | Cycles through edit modes (Shuffle, Slip, Spot, Grid). |
    | `Edit Tool` |  | Cycles through main edit tools (Zoom, Trim, Select, Grabber, Smart Tool, Scrub, Pencil). |
    | `Trim` |  | Enables Trim Tool in Edit Window. |
    | `Select` |  | Enables Select Tool in Edit Window. |
    | `Grab` |  | Enables Grabber Tool in Edit Window. |
    | `Pencil` |  | Enables Pencil Tool in Edit Window. |
    | `Zoom` |  | Enables Zoom tool. |
    | `Scrub` |  | Enables Scrub tool (see Transport section for Scrub wheel functions). |
    | `Smart Tool` |  | Enables Smart tool. |

=== "V-Window"

    | V-Window Mode |  |  |
    |---|---|---|
    | With the V-Window feature, users can instantly control any plug-ins or controls on screen through their control surface's channel strip with a touch of a button. |  |  |
    | Master Fader |  | Press once to enable V-Window mode for the 8th channel fader. Press a 2nd time to cycle back to basic channel control. |
    | Mute |  | While in V-Window mode, the Mute button on the last channel strip will cycle through the various V-Window Modes which are listed below: |
    |  |  | VButton: Use this mode to interact with button controls. The mouse will stay in its place and activate a button press when the fader is touched. |
    |  |  | VButtonSet: Use this mode to create and cycle through different button set points. With the mouse hovering above the on screen button's position press Shift+Solo on the control surface to set a Pin at that location. Using the fader in this mode will cylce between multiple Pins to use with VButton mode. |
    |  |  | VWKnob: Use this mode when interacting with knob controls on the plug-ins GUI. |
    |  |  | VWHSlider: Use this mode when interacting with horizontal slider controls on the plug-ins GUI. |
    |  |  | VWVSlider: Use this mode when interacting with vertically slider controls on the plug-ins GUI. |
    | Solo |  | While in V-Window Mode, pressing the Solo button will pin the mouse location and revert to that location any time the fader is touched. Once the fader is released, the mouse is also returned to that pin position. This way it is very easy to pin a parameter and instantly control it without having to worry with the mouse cursor is on the screen. |
    | Select |  | Use the Select button while in V-Window mode to reset the fader position. |

=== "MIDI Mode"

    | MIDI Mode |  |  |
    |---|---|---|
    | MIDI Mode converts the surfaces faders, knobs, and buttons into assignable MIDI Controls that can be mapped in the DAW. |  |  |
    | Mon/0 |  | Toggles surface between DAW Mode and MIDI Mode |
    | Select (Group Button) |  | Toggles the DSP Section between DAW Mode and MIDI Mode. |
