# Setting Up Ethernet Controllers

Ethernet is a common networking system for connecting devices to a computer's Ethernet port. Modern Ethernet is very high speed and can manage many devices on a network such as routers, switches, and Ethernet-based control surfaces. V-Control Pro supports Ethernet control surfaces for fast and reliable connectivity.

!!! warning "Windows 10, 11 Systems - Npcap Utility Required"
    The Windows OS does not provide for Ethernet 2 connectivity. You must install the "Npcap" utility so that V-Control Pro can connect to legacy hardware. V-Control Pro will message you if "Npcap" is not installed and will point you to a free utility for you to install. At the time of this writing, it is available at [Npcap.com](https://npcap.com/#download)

!!! warning "Disable Or Configure Firewall"
    Legacy Ethernet surfaces will not be able to connect if a firewall is enabled on your computer. If you need to use a firewall it must be configured to allow Ethernet 2 messages to the hardware MAC address of the surface.

!!! warning "Ethernet switch needed for newer Macs with Apple Silicon"
    Newer Macs do not work correctly with an Ethernet cable directly between the surface and Mac. Please use any low-cost Ethernet switch or router between the surface to enable connectivity.

!!! warning "Pro Tools - Do Not Enable Legacy Controllers for Ethernet"
    If you are setting up a surface for Pro Tools, it is important that the `Enable Legacy Controllers' check box is not enabled. The checkbox is located in the Pro Tools Ethernet Controllers tab in the Peripherals window. 


## Disable V-Control Pro Virtual MIDI Ports

* In Pro Tools, select the menu Setup / MIDI / MIDI Input Devices
* Enable the `V-Control, V-Control XT-2, V-Control XT-3, V-Control XT-4` and `V-Pan` ports.
* Do not enable the `V-Control MIDI Mode` port.


## Ethernet Cables

One confusing thing about Ethernet is that an Ethernet cable connector uses one wire for transmitting data and one for receiving data. There are two types of Ethernet cables.

* Crossover Cables - these cables swap the `send` and `receive` wires for each end of the cable.
* Non-crossover Cables - these cables do not swap the `send` and `receive` wires for each end of the cable.

Most Ethernet hardware automatically detects the type of cable. But older ports do not. Use an Ethernet switch for your network so that you don't have to worry about what type of Ethernet cables you are using.

## Ethernet Switches (Not Hubs)

We recommend you use an Ethernet switch in your control surface network. They work with any Ethernet cable and provide fast, efficient connections with both types of Ethernet cables. The original Ethernet hardware in the 1990s used simple Ethernet "hubs" to connect multiple devices to a network. But these hubs were very inefficient because all the devices were physically connected to each other and the computer had to tell devices to "retry" when data "collisions" happened and the type of cable was very important. Ethernet "switches" were invented that solve these problems. The switch automatically connects one device at a time to the network so that no collisions happen with any type of cable. Modern Ethernet switches are very low cost and fast. Internet routers also act as switches.

!!! info "Low Cost Switches Work Great"
    If you are purchasing an Ethernet switch, we recommend you save money and buy the lowest cost one you can find. Most legacy Ethernet surfaces use a speed of just 10 Mbps.

<a id="networking"></a>

## macOS and Windows Networking

Legacy Digidesign and Avid Ethernet-based surfaces use a fast, non-standard protocol using Ethernet 2 packets. They do not use modern TCP/IP networking.

* macOS - For macOS, V-Control Pro does not need to use any special drivers for connecting to legacy hardware.
* Windows - The Windows OS does not provide for Ethernet 2 connectivity. You must install the "Npcap" utility so that V-Control Pro can connect to legacy hardware. V-Control Pro will message you if "Npcap" is not installed and will point you to a free utility for you to install. At the time of this writing, it is available at [Npcap.com](https://npcap.com/#download)

## Adding An Ethernet Control Surface

For surfaces that use Ethernet to connect to a computer, follow these instructions to add a surface to V-Control Pro.

* Open the V-Control Pro Setups Window.
* Click on + Add New under the Controllers section and select Add Ethernet Device…
* With the Ethernet Browser window open, ensure the correct Network is selected that the surface is connected to.
* Wait up to ten seconds for the surface to be recognized. When it appears, select it and click Add.
