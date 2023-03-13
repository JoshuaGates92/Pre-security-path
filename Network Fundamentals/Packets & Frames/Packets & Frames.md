
## What are packets and frames?

Packets and frames are ==small pieces of data== that are combined to make a larger piece of data.
In the OSI Model, a ==frame is layer 2, data link==, where there is no IP address information. This is the ==encapsulation== process that was mentioned previously in [[OSI Model]].

When encapsulating information is stripped from a packet, a frame is left.

![[packet-headers.png]]


## TCP/IP (Three-Way Handshake)

This protocol has four layers:
1. Application
2. Transport
3. Internet
4. Network Interface

TCP is connection-based so devices connect between client/server before any data sends.

![[tcp-summary.png]]

Common TCP headers:
![[tcp-headers.png]]

### Three-Way Handshake

![[three-way-handshake.png]]


## UDP/IP

Stateless protocol not requiring a constant connection.
Shares some common headers with TCP:
![[Pasted image 20230312132741.png]]

Stateless refers to the server not checking if data is being received by the client, just sends indiscriminantly.
