# MIDI Chart


Learn more about [MIDI Mode here](https://neyrinck.com/midimode/).

### MIDI Out From Surface
All buttons, encoders, and faders send CC messages that range from 0 to 127.

### MIDI Feedback
LEDs
LEDs respond to CC messages . OFF = less than 40. ON = greater than or equal to 40.

### Faders
Faders respond to CC messages. 0 to 127

### Encoder LED Rings
Encoder LED rings respond to CC messages. 0 to 127

### Meters
Track and output meters respond to CC messages. 0 to 127
### Scribbles
Scribble text can be set using system exclusive messages.

#### SysEx Message

| F0 13 40 40 0 | Start Of Header                     |
| ----------- | ------------------------------------ |
| `ss`        | Surface ID. Control24=1, C24=2, ProControl=3, D-Command=4  |
| `zz`        | Zone ID |
| `xx`        | Control ID |
| `ss`        | ASCII Text |
| `F7`        | End Of SysEx |

|              |	Decimal      |	Hex         |
| ----------- | ---------------- | ---------------- |
| sysex header	|	19,64,64,0,4 | 13,40,40,0,4 |
| sysex address	|	             |              |
| dcommand/main/mixer/strips/0/track/encoder/0/scribble | sysex	| 5 1	| 05 01 |

dcommand/main/mixer/strips/0/track/encoder/1/scribble
sysex	6 1	06 01
dcommand/main/mixer/strips/0/track/name	sysex	7 1	07 01
dcommand/main/mixer/strips/1/track/encoder/0/scribble
sysex	5 2	05 02
dcommand/main/mixer/strips/1/track/encoder/1/scribble
sysex	6 2	06 02
dcommand/main/mixer/strips/1/track/name	sysex	7 2	07 02
dcommand/main/mixer/strips/2/track/encoder/0/scribble
sysex	5 3	05 03
dcommand/main/mixer/strips/2/track/encoder/1/scribble
sysex	6 3	06 03
dcommand/main/mixer/strips/2/track/name	sysex	7 3	07 03
dcommand/main/mixer/strips/3/track/encoder/0/scribble
sysex	5 4	05 04
dcommand/main/mixer/strips/3/track/encoder/1/scribble
sysex	6 4	06 04
dcommand/main/mixer/strips/3/track/name	sysex	7 4	07 04
dcommand/main/mixer/strips/4/track/encoder/0/scribble
sysex	5 5	05 05
dcommand/main/mixer/strips/4/track/encoder/1/scribble
sysex	6 5	06 05
dcommand/main/mixer/strips/4/track/name	sysex	7 5	07 05
dcommand/main/mixer/strips/5/track/encoder/0/scribble
sysex	5 6	05 06
dcommand/main/mixer/strips/5/track/encoder/1/scribble
sysex	6 6	06 06
dcommand/main/mixer/strips/5/track/name	sysex	7 6	07 06
dcommand/main/mixer/strips/6/track/encoder/0/scribble
sysex	5 7	05 07
dcommand/main/mixer/strips/6/track/encoder/1/scribble
sysex	6 7	06 07
dcommand/main/mixer/strips/6/track/name	sysex	7 7	07 07
dcommand/main/mixer/strips/7/track/encoder/0/scribble
sysex	5 8	05 08
dcommand/main/mixer/strips/7/track/encoder/1/scribble
sysex	6 8	06 08
dcommand/main/mixer/strips/7/track/name	sysex	7 8	07 08
dcommand/main/customfaders/focuschannel	sysex	4 39	04 27
dcommand/main/dynamics/scribble	sysex	1 38	01 26
dcommand/main/eq/scribble	sysex	2 38	02 26
dcommand/main/softkeys/scribble/0	sysex	5 21	05 15
dcommand/main/softkeys/scribble/1	sysex	5 22	05 16
dcommand/main/softkeys/scribble/2	sysex	5 23	05 17
dcommand/main/softkeys/scribble/3	sysex	5 24	05 18
dcommand/main/softkeys/scribble/4	sysex	5 25	05 19
dcommand/main/softkeys/scribble/5	sysex	5 26	05 1a
dcommand/main/softkeys/scribble/6	sysex	5 27	05 1b
dcommand/main/softkeys/scribble/7	sysex	5 28	05 1c
dcommand/main/softkeys/scribble/8	sysex	5 29	05 1d
dcommand/main/softkeys/scribble/9	sysex	5 30	05 1e
dcommand/main/softkeys/scribble/10	sysex	5 31	05 1f
dcommand/main/softkeys/scribble/11	sysex	5 32	05 20

