## Introducing LAN Topologies

### Star
Devices connected via a central networking device such as a hub or switch.
Good reliability and scalability, but more costly

![Star Topology | 450](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-lan/star.png)

As the network scales more maintenance is required


### Bus
Relies on single connection known as a ==backbone cable== 
Prone to bottlenecks and difficulty with troubleshooting as diagnosing which device is having or causing the problem can be difficult
Also, little to no redunancy if the backbone cable has problems
Cost-efficient

![Bus | 450](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-lan/bus.png)

### Ring (Token)
Data is sent around the loop until it reaches desired device.
Inefficient way to send data as it flows one direction, but easy to troubleshoot
Less prone to bottlenecks

![Ring | 450](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-lan/ring.png)


### What is a switch?
Dedicated device used to aggregate devices, usually found in larger networks, such as a corporate setting


## A Primer on Subnetting
==Subnetting== - Breaking a network down into smaller, networks within a network

Subnets use IP addresses in three ways:
1. identify the host network
2. identify the host address
3. identify the default gateway


## ARP (Address Resolution Protocol) Protocol

Allows devices to identify themselves on a network
In other words, associates a MAC address with an IP address

## DHCP Protocol

Dynamic Host Configuration Protocol assigns IP addresses to devices if not manually done.
 1. Device sends out a ==DHCP Discover== - checks if DHCP networks are active
 2. DHCP server replies with a list of available IP addresses called ==DHCP Offer==
 3. Device sends a request confirming it wants a particular IP ==DHCP Request==
 4. Device can use that IP ==DHCP ACK==
 








