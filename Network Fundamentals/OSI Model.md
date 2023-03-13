Stands for: Open Systems Interconnection Model

Seven layer model starting with 7 and working down to 1:
![OSI Graphic | 450](https://assets.tryhackme.com/additional/networking-fundamentals/osi-model/osimodel.svg)

As data travels through each layer, more information is added to the data. This process is called ==encapsulation==.


## Layer 7: Application

Where protocols and rules are in place to determine how the user should interact with data sent or received.

## Layer 6: Presentation

Standardisation of data starts to take place here as no matter how various software uses data, it needs to be readable by other devices/software.

This layer acts as a translator both to and from other layers.
==Data encryption is an example of tasks that occur at this layer==.

## Layer 5: Session

Creation of a connection between computers/devices happens here. Data is divided into ==packets== and sent to the connected device.

Note: *sessions are unique — meaning that data cannot travel over different sessions, but in fact, only across each session instead.*

## Layer 4: Transport

Two protocols here: Transmission Control Protocol(TCP) and User Datagram Protocol(UDP)

### TCP
| Advantages                                                                               | Disadvantages                                                                                                                                     |
|------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| Guarantees the accuracy of data.                                                         | Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used. |
| Capable of synchronising two devices to prevent each other from being flooded with data. | A slow connection can bottleneck another device as the connection will be reserved on the receiving computer the whole time.                      |
| Performs a lot more processes for reliability.                                           | TCP is significantly slower than UDP because more work has to be done by the devices using this protocol.                                         |

Used for things such as:
1. File sharing
2. Internet browsing
3. Email

### UDP
No synchronisation of devices here... data is sent, whether it gets to its target or not... up to fate!

| Advantages                                                                                                            | Disadvantages                                                                      |
|-----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| UDP is much faster than TCP.                                                                                          | UDP doesn't care if the data is received.                                          |
| UDP leaves the application layer (user software) to decide if there is any control over how quickly packets are sent. | It is quite flexible to software developers in this sense.                         |
| UDP does not reserve a continuous connection on a device as TCP does.                                                 | This means that unstable connections result in a terrible experience for the user. |


## Layer 3: Network

Routing and re-assembly takes place here.

Which route is taken has three questions to consider:
1. What path is the shortest? I.e. has the least amount of devices that the packet needs to travel across.
2. What path is the most reliable? I.e. have packets been lost on that path before?
3. Which path has the faster physical connection? I.e. is one path using a copper connection (slower) or a fibre (considerably faster)?
==At this layer, everything is dealt with via IP addresses such as 192.168.1.100. Devices such as routers capable of delivering packets using IP addresses are known as Layer 3 devices — because they are capable of working at the third layer of the OSI model.==

Two protocols to be aware of at this point:
1. Open Shortest Path First (OSPF)
2. Routing Information Protocol (RIP)


## Layer 2: Data Link

The data link layer focuses on the physical addressing of the transmission. It receives a packet from the network layer (including the IP address for the remote computer) and adds in the physical **MAC** (Media Access Control) address of the receiving endpoint.

MAC addresses can't be changed, but they can be spoofed. When information is sent across a network, it's actually the physical address that is used to identify where exactly to send the information.

Additionally, it's also the job of the data link layer to present the data in a format suitable for transmission.

All network devices have a Network Interface Card in them with a MAC address literally burn into them set by the manufacturer.

## Layer 1: Physical

Physical components used to connect devices such as ethernet cables



