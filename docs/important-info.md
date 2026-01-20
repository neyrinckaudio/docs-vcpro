# Important Setup Information

### Windows Ethernet Surface Users

!!! warning "Required: Npcap Installation"
    Windows systems using Ethernet surfaces (ProControl, Control 24, C|24) **must** install Npcap:
    
    **Download**: [Npcap.org](https://npcap.com/#download)
    
    **Network Requirements**:
    
    - Connect computer's Ethernet directly to surface OR use an Ethernet switch
    - **Do NOT use Wi-Fi** for the connection

### Pro Tools Users

!!! warning "Important HUI Metering Information"
    The HUI protocol provides for stereo track metering. It does not provide for output metering. Surfaces that have output meters will not display any output metering when connected to Pro Tools.

V-Control Pro uses the HUI protocol with Pro Tools Studio/Ultimate to provide for 8, 16, 24, or 32 channels of control. The Pro Tools MIDI Peripherals window must be configured to use V-Control Pro's virtual MIDI ports for Pro Tools to communicate with V-Control Pro.

!!! warning "Enable MIDI Ports In Pro Tools"
    V-Control Pro provides virtual MIDI ports for Pro Tools to use. These ports must be enabled for MIDI input.

!!! warning "FaderPort 8/16 With Pro Tools 2022 And Earlier"
    FaderPort 8/16 setup depends upon which version of Pro Tools you are using. Please see the special setup information for FaderPort 8/16 with Pro Tools 2022 and earlier.

### Logic Pro Users

!!! info "Version Compatibility"
    **V-Control Pro 3**: Compatible with Logic 10.6 and later only
    
    **V-Control Pro 2.7.2**: Required for Logic 10.5 or earlier

!!! warning "Multiple Fader Packs Limitation"
    V-Control Pro 3 does **not** support multiple ProControl Fader Pack devices with Logic Pro 10.6 and later. For multiple Fader Packs:
    
    - Use V-Control Pro 2.7.2 (Intel Macs only)
    - M1 Mac systems do not support multiple Fader Pack units

**Upgrading V-Control Pro with Logic:**
1. Delete surfaces in Logic Pro → Control Surfaces → Setup
2. Quit Logic completely
3. Run V-Control Pro installer
4. Reconfigure surfaces

### Cubase/Nuendo Users

**Upgrading V-Control Pro with Cubase/Nuendo:**
1. Delete surfaces in Studio → Studio Setup
2. Quit Cubase/Nuendo completely  
3. Run V-Control Pro installer
4. Reconfigure surfaces

### Legacy iPad App Users

!!! note "Ney-Fi Migration"
    **Ney-Fi has been renamed to "V-Control Pro"**
    
    - Launch "V-Control Pro" on your computer (not Ney-Fi)
    - Continue using V-Control Pro 1 for iPad
    - **No new purchase required** for existing features

**V-Control Pro 2 New Features** (license required):
- V-Console app for mix and edit control
- 16 tracks of control on single device
- Up to 32 tracks total control
- Multiple controller support
- Smartphone compatibility

