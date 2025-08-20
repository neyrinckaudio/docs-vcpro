# Setting Up Ethernet Controllers

Ethernet is a common networking system for connecting devices to a computer's ethernet port. Modern ethernet is very high speed and can manage many devices on a network such as routers, switches, and ethernet-based control surfaces. V-Control Pro supports ethernet control surfaces for fast and reliable connectivity.

!!! warning "Windows 10, 11 Systems - Npcap Utility Required"
    The Windows OS does not provide for Ethernet 2 connectivity. You must install the "Npcap" utility so that V-Control Pro can connect to legacy hardware. V-Control Pro will message you if "Npcap" is not installed and will point you to a free utility for you to install. At the time of this writing, it is available at [NPcap.com](https://npcap.com/#download)

!!! warning "Disable Or Configure Firewall"
    Legacy ethernet surfaces will not be able to connect if a firewall is enabled on your computer. If you need to use a firewall it must be configured to allow Ethernet 2 messages to the hardware MAC address of the surface.

## Ethernet Cables

One confusing thing about ethernet is that an ethernet cable connector uses one wire for transmitting data and one for receiving data. There are two types of ethernet cables.

* Crossover Cables - these cables swap the send and receive wires for each end of the cable.
* Non-crossover Cables - these cables do not swap the send and receive wires for each end of the cable.

Most ethernet hardware automatically detects the type of cable. But older ports do not. Use an ethernet switch for your network so you don't have to worry about what type of ethernet cables you are using.

## Ethernet Switches (Not Hubs)

We recommend you use an ethernet switch in your control surface network. They work with any ethernet cable and and provide fast, efficient connections with both types of ethernet cables. The original ethernet hardware in the 1990s used simple ethernet "hubs" to connect multiple devices to a network. But these hubs were very inefficint because all the devices were physically connected to each other and the computer had to tell devices to "retry" when data "collisons" happened and the type of cable was very important. Ethernet "switches" were invented that solve these problems. The switch automatically connects one device at a time to the network so that no collisions happen with any type of cable. Modern ethernet switches are very low cost and fast. Internet routers also act as switches.

<a id="networking"></a>

## Mac OS and Windows Networking

Legacy Digidesign and Avid ethernet-based surfaces use a fast, non-standard protocol using Ethernet 2 packets. They do not use modern TCP/IP networking.

* Mac OS - For Mac OS, V-Control Pro does not need to use any special drivers for connecting to legacy hardware.
* Windows - The Windows OS does not provide for Ethernet 2 connectivity. You must install the "Npcap" utility so that V-Control Pro can connect to legacy hardware. V-Control Pro will message you if "Npcap" is not installed and will point you to a free utility for you to install. At the time of this writing, it is available at [NPcap.com](https://npcap.com/#download)

## Adding An Ethernet Control Surface

For surfaces that use Ethernet to connect to a computer, follow these instructions to add a surface to V-Control Pro.

* Open the V-Control Pro Setups Window.
* Click on + Add New under the Controllers section and select Add Ethernet Device…
* With the Ethernet Browser window open, ensure the correct Network is selected that the surface is connected to.
* Wait up to ten seconds for the surface to be recognized. When it appears, select it and click Add.
