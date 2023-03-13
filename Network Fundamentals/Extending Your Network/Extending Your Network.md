## Introduction to Port Forwarding

Port forwarding at this stage is just opening ports to make clients accessible to networks.
	- Configured at the router

## Firewalls 101

Control what addresses (and on which ports) can access a network.

![[Firewall states.png]]

## VPN Basics

Technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the Internet (known as a tunnel). Devices connected within this tunnel form their own private network.

![[VPN Tech.png]]

## LAN Networking Devices

Routing is just data travelling across networks, or layer 3 of the [[OSI Model]]

### What is a Switch?

Connects multiple devices to a network that can operate at OSI layer 2 and 3.
	- Switches can operate at both layer 2 and layer 3 of the OSI model. However, these are exclusive in the sense that Layer 2 switches cannot operate at layer 3.

Take, for example, a layer 2 switch in the diagram below. These switches will forward frames (remember these are no longer packets as the IP protocol has been stripped) onto the connected devices using their MAC address.

Layer 3 switches are more sophisticated than layer 2, as they can perform _some_ of the responsibilities of a router. Namely, these switches will send frames to devices (as layer 2 does) and route packets to other devices using the IP protocol.

