# Connect and Protect: Networks and Network Security

# Module 1: Network Architecture

# What you'll learn
- Structure of a network
- Standards of networking tools
- Cloud networks
- TCP/IP model

---

# Network

## Definition
A group of connected devices
- Can be wired or wireless, networks communicate with networks in other locations and with the devices on them
- Require addresses which ensures that communications happen between the intended devices.

### Example
A home network may be devices such as your laptop, printers, etc connected to each other.

# Local Area Network

## Definition
A network that spans a small area like an office building, a school, or a home.

### Example
When a personal device like your phone connects to the Wi-Fi in your house they form a LAN, then the LAN connects to the internet.

# Wide Area Network

## Definition
A network which spans a large geographical area like a city, state, or country.

### Example
An example of a WAN could be the internet.

# Hub

## Definition
A network device that broadcasts information to every device on a network
- Provides a common point of connection for all devices driectly connected to it
- Hubs are a security risk, as they can be vulnerable to eavesdropping.

### Example
Hubs are akin to a radio tower that broadcasts a signal to any radio that tunes into the right frequency.

# Switch

## Definition
A device that makes connections betweeen specific devices on a network by sending and receiving data between them
- Switchs forwards packets between devices directly connected to it
- Analyzes the destination addresses of each data packet and sends it to intended devices
- Switches maintain a MAC address table that matches MAC addresses of devices on the network to port numbers on the switch and forwards incoming data packets according to the destination MAC addresses

### Example
A switch only passes data to the intended destination

# Router

## Definition
A network device that connects multiple networks together
- Connecting and directing traffic based on the IP address of the destination network
- Routers allow all devices on different communicate with each other
- Routers work by reading the IP header information and forwards the data packet to the next router on the path to its destination.
- This continues until the packet reaches the destination network.

# Modem

## Definition
A device that connects your router to the internet and brings internet access to the LAN 
- Modems recieve transmissions or digital signals from the internet and convert them into a digital format compatible with the physical connection by your internet service provider

### Internet Service Provider
- Connects the internet via telephone lines, coaxial cables, or fiber optic cables.

# Wireless Access Point

## Def
Sends and recieves digital signals over radio waves creating a wireless network
- Devices with wireless adapters connect to the access point using Wi-Fi
- Wireless access points and the devices connected to them use WiFi protocols to send data through radio waves where they are sent to routers and switches and directed along the path to their final destination.

# Wi-Fi

## Definition
A set of standards used by network devices to communicate wirelessly.

# Virtualization Tools

### Def
Pieces of software that perform network operations

# Firewalls

### Def
A firewall is a network security device which monitors traffic to or from your network.

# Server

### Def
Provide information and services for devices like computers, smart home devices, and smartphones on the network. The devices that connect to a server are called clients.

---

# Cloud Networks

# Cloud Computing

## Def
The practice of using remote servers, applications, and network services that are hosted on the internet instead of on local physical devices.

# Cloud Network

## Def
A collection of servers or computers that store resources and data in remote data centers that can be accessed via the internet.

## Cloud service providers offer
- On demand storage
- Processing power
- Analytics
- Cheaper alternative
- No physical maintenance or renovations

## CSP three main services
- Software as a Service (SAAS) refers to software suites operated by the CSP that a company can use remotely wihtout hosting the software
- Infastructure as a Service (IaaS) refers to use of virtual computer componenets offered by the CSP.
- Platform as a service (PaaS) refers to tools that application developers can use to design custom applications for their company.

### Hybrid Cloud Enviornments
- Organization uses a CSP service in addition to their on premise computers, networks, and storage.

### Software-Defined Networks
- Made up of virtual network devices and services, SDN tools are hosted on servers located at the CSP's data center, and provide virtual switches, routers, etc.

---

# Network Communication

# Data Packet

## Def
A basic unit of information which travels from one device to another within a network.
Contains information about content
Where its coming from and where its going.

### Data Packets Breakdwon
Header
- The IP address, MAC address of the destination device, and the protocol number which tells the recieving device what to do.
Body
- Message which needs to be transmitted
Footer
- Signals to the receiving device that the packet is finished.

# Bandwidth

## Def
The amount of data a device recieves every second
Can be calculated by dividing quantity of data by time time in seconds

# Packet Sniffing

## Def
The practice of capturing and inspecting data packets across a network

# Transmission Control Protocol (TCP)

## Definition
An internet communication protocol that allows two devices to form a connection and stream data.
- TCP protocol includes a set of instructions to organize data, so it can be sent across a network
- Also establishing a connection between two devices which ensures that packets reach their appropriate destination.

# Internet Protocol (IP)

## Definition
A set of standards used for routing and addressing data packets as they travel between devices on a network.
- IP address is included in the internet protocol, and functions as an address for each private network.

# Port 

## Definition
A software based location that organizes the sending and receiving of data between devices on a network.

- Ports divide network traffic into segments based on the service they will perform between two devices.
- The computers sending and receiving these data segments know how to prioritize and process these segments based on their port number.
- Port numbers allow computers to spit the network traffic and prioritize the operations they will perform with the data.

# Common port numbers

- Port 25: Email
- Port 443: Secure Internet Communication
- Port 20: Large File Transfers

## TCP/IP Model Cont.
- A framework used to visualize how data is organized and transmitted across a network

# Layers of TCP/IP model

## 1. Network Access Layer
Deals with creation of data packets and their transmission across networks. This includes physical hardware devices connected to physical cables and switches that direct data to its destination

## 2. Internet Layer
This is where IP addresses are attached to data packets to indicate the location of the sender and receiver. The Internet layer also focuses on how networks connect to each other. 
ICMP internet control message protocol shares error information and status updates of data packets.

Ex. Data packets containing information that determine whether they will stay on the LAN or will be sent to a remote network like the internet.

## 3. Transport Layer
Protocols that control the flow of traffic across a network. These protocols permit or deny communication with other devices and include information about the status of the connection. 
TCP and UDP are the two transport protocols that occur at this layer.
TCP is an internet communication protocol that allows two devices to form a connection and stream data. TCP contains the port number of the intended destination service which resides in the TCP header of a TCP/IP packet.
UDP User Datagram Protocol is a connectionless protocol that does not establish a connection between devices before transmissions. It is used by applications that are not concerned with the reliability of the transmission. UDP does not establish network connection, it's mostly used for performance sensitive applications that operate in real time such as video streaming.

### Example
Activities in the transfer layer include error control, which ensures data is flowing smoothly across the network.

## 4. Application Layer
Protocols determine how the data packets will interact with receiving devices. Functions that are organized at the application layer include file transfers and email services.

### Common application layer protocols
- HTTP - Hypertext transfer protocol
- SMTP - Simple Mail Transfer Protocol
- SSH - Secure Shelll
- FTP - File Transfer Protocol 
- DNS - Domain name system

---

# OSI Model
- Is a standardized concept that describes the 7 layers computers use to communicate and send data over the network.

## Layer 7 Application Layer
- Includes processes that directly involve the everyday user. This layer includes all of the networking protocols that software applications use to connect a user to the internet. 
- Characteristic: User connection to the internet via applications and requests.

### Example 
Using a web browser. The internet browser uses HTTP to send and receive information from the website server.

## Layer 6 Presentation Layer
- Involves data translation and encryption for the network. This layer adds to and replaces data with formats that can be understood by applications on both sending and receiving systems.
- Processes at the presentation layer require use of a standardized format.
- Some formatting functions that occur at layer 6 are encryption, compression and confirmation that the character code set can be interpreted on the receiving system.

### Example 
One example of encryption that takes place at this layer is SSL, which encrypts data between web servers and browsers as part of websites with HTTPS.

## Layer 5 Session Layer
- A session describes when a connection is established between two devices. Open session allows the devices to communicate with each other. Session layer protocols keep the session open while data is being transferred and terminate the session once the transmission is complete.
- Characteristics: Responsible for activities such as authentication, reconnection and setting checkpoints for a data transfer. 

### Example 
Sessions include a request and response between applications. Functions in the session layer respond to requests for services from processes in layer 6 and send requests for services to the transport layer (layer 4).

## Layer 4: Transport Layer
- Responsible for delivering data between devices
- Characteristics; Handles speed of the data transfer, flow of the transfer and breaking down data into smaller segments to make them easier to transport. 

### Example 
TCP and UDP are transport layer protocols

## Layer 3: Network Layer
- Oversees receiving the frames from the data link layer, and delivers them to the intended destination. The intended destination can be found based on the addresses that reside in the frame of the data packets.

## Layer 2: Data Link Layer
- Organizes sending and receiving packets within a single network. 
- Characteristics: home to switches on the local network and network interface cards on local devices.

### Examples 
Protocols include NCP, HDLC, and SDLC are used at data link layer

## Layer 1: Physical Layer
- Corresponds to the physical hardware involved in network transmission. To travel across an ethernet or coaxial cable data packets are translated into a stream of binary. This stream of data is sent across the physical wiring and cables. Then received and passed on to higher levels of the OSI model.

# Two types of IP addresses
- IP version 4
- IP version 6

- IP v4 (older, less characters)
- IP v6 ( Newer, more characters)

## IP addresses can be public and private
- Tied to your geographic location
- All devices on a network share the same public facing address
- Private addresses are only seen and unique to addresses located on your network for your devices.

## MAC address
- A unique alphanumerical identifier that is assigned to each physical device on a network.
- Think of the MAC address table like an address book that the switch uses to direct data packets to the appropriate device.

### Operations at the Network Layer
- Functions at the network layer consists of organizing the addressing and the delivery of data packets across the network from the host device to the destination device.
- Including directing packets from one router to another router across the internet til it reaches the IP address of the destination network
- THe destination IP address is contained within the header of each data packet. 
- A data packet is referred to as an IP packet for TCP and a datagram for UDP connections.
- Header information communicates more than just the destination, including the source IP address, size of packet, and which protocol used for the data portion of the packet.

### Format of IPv4 Packet
- AN IPv4 header format is determined by the IPv4 Protocol and includes the IP routing and information that devices used to direct the packet. The size of the header ranges from 20 to 60 bytes. 
- The first 20 bytes are a fixed set of information containing data such as the source and destination IP address, header length and total length of the packet.
- The length of the data section of an IPv4 can vary in size. Maximum possible size is 65,3535 bytes.
- There are 13 fields within the header of an IPv4 Packet
- Version: This 4 bit component tells receiving devices what protocol the packet is using
- IP header length (HLEN or IHL): HLEN is the packet header length. 
- Type of Service (ToS): Routers prioritize packets for delivery to maintain the quality of service on the network. The ToS field provides the router with this information.
- Total Length: This field communicates the total length of the entire IP packet, including the header and data. The maximum size of an IPv4 packet is 65,535 bytes.
- Identification: IPv4 Packets can be up to 65,535 bytes but most networks have a smaller limit. Typically packets are divided or fragmented into smaller IP packets. Providing a unique identifier for all the fragments of the original IP packet.
- Flags: This field provides the routing device with more information about whether the original  packet has been fragmented and if there are more fragments in transit.
- Fragmentation Offset: The fragment offset field fells routing devices where in the original packet the fragment belongs.
- Time to Live (TTL): Presents data packets from being forwarded by routers indefinitely. When the TTL counter reaches zero, the router currently holding the packet will discard the packet and return an ICMP time exceeded error message to the sender.
- Protocol: Tells the receiving device which protocol will be used for the data portion of the packet.
- Header checksum: The header checksum contains a checksum that can be used to detect corruption of the IP header in transit. Corrupted packets are discarded. 
- Source IP address: The source IP address is the IPv4 address of the sending device
- Destination IP address: THe destination IP address is the IPv4 address of the destination device.
- Options: The options field allow for security options to be applied to the packet if the HLEN value is greater than five. The field communicates these options to the routing devices

---

# Key Takeaways

- Devices send and receive data packets, which provide information about the source and the destination of the data
- Network devices are specialized vehicles which function to manage what is being sent and received over the network.
- Devices such as computers, phones or smart fridges connect to the network via those network devices
- Each device and desktop computer has a unique MAC address and IP address, which identifies it on the network
- CSPS are companies which own large data centers that are providing modern technology services, including compute, storage, and networking all through the internet.
- Irregular speeds and bandwidth may tell a security professional that there may be an attack.
- Both the TCP/IP and OSI models are conceptual models which help network professionals visualize network processes and protocols in data transmission between two or more systems.
- Network Protocols are sets of standards used for network communication/data transmission



