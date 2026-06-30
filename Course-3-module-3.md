# Course 3, Module 3: Network Security

## Overview

This module covers common network intrusion tactics, how attackers abuse network traffic, and how security teams use packet analysis tools to detect and investigate suspicious activity.

## Topics Covered

- Network security
- Network intrusion tactics
- Network attack protection
- Packet sniffing and packet analysis
- Denial-of-service attacks
- IP spoofing attacks

## Common Network Intrusion Attacks

Network attacks can directly impact organizations by exposing sensitive information, damaging reputation, disrupting operations, and costing time and money to recover from.

Common network intrusion attacks include:

- **Malware**
- **Spoofing**
- **Packet sniffing**
- **Packet flooding**

## Network Interception Attacks

A **network interception attack** occurs when an attacker intercepts network traffic to steal valuable information, manipulate data, or interfere with the transmission.

### Packet Sniffing

**Packet sniffing** is when malicious actors use hardware or software tools to capture and inspect data while it is in transit across a network.

Attackers may use packet sniffing to:

- Capture sensitive information from network traffic
- Learn details about a target network
- Alter traffic by injecting or modifying malicious code
- Support other attacks, such as spoofing or on-path attacks

## Backdoor Attacks

A **backdoor** is a weakness or hidden access method that bypasses normal authentication or access control mechanisms.

Backdoors may be intentionally created by programmers or administrators, but attackers can also install them after compromising a system. Once installed, a backdoor can help an attacker maintain persistent access to an organizationâs network or systems.

## Denial-of-Service Attacks

A **denial-of-service attack**, or **DoS attack**, targets a network, system, or server by overwhelming it with traffic or requests. The goal is to disrupt normal operations and make the service unavailable to legitimate users.

A **distributed denial-of-service attack**, or **DDoS attack**, is a type of DoS attack that uses multiple devices or servers from different locations to flood the target with unwanted traffic.

## Common Network-Level DoS Attacks

### SYN Flood Attack

A **SYN flood attack** is a DoS attack that abuses the TCP three-way handshake by flooding a server with SYN requests.

The normal TCP handshake works like this:

1. A device sends a **SYN** request to a server.
2. The server responds with a **SYN/ACK** response.
3. The device replies with an **ACK**, and the TCP connection is established.

In a SYN flood attack, the attacker sends many SYN requests but does not complete the handshake. This leaves server resources tied up while waiting for final ACK responses. If the server receives more SYN requests than it can handle, it may slow down or become unavailable.

### Internet Control Message Protocol

**Internet Control Message Protocol**, or **ICMP**, is a network protocol used by devices to communicate data transmission errors and status messages across a network.

A simple way to think of ICMP is that it helps devices send network status updates, such as whether a destination is reachable.

### ICMP Flood Attack

An **ICMP flood attack** is a DoS attack where an attacker repeatedly sends ICMP packets to a network server.

This can force the target to spend resources responding to ICMP requests. Over time, the traffic can consume available bandwidth and cause the server or network to slow down or crash.

### Ping of Death

A **Ping of Death** attack is a DoS attack where an attacker sends an oversized or malformed ICMP packet to a target system.

Because traditional ICMP packets have a maximum size of 64 KB, vulnerable systems may crash or become unstable when they receive packets that exceed what they can properly process.

## Network Protocol Analyzers

A **network protocol analyzer**, sometimes called a **packet sniffer** or **packet analyzer**, is a tool used to capture, inspect, and analyze network traffic.

Security professionals use protocol analyzers to:

- Monitor networks
- Investigate suspicious activity
- Troubleshoot performance issues
- Establish a baseline for normal traffic patterns
- Identify malicious or unauthorized traffic
- Locate unauthorized wireless access points or instant messaging traffic
- Create alerts for network issues or security threats

## Tcpdump

**Tcpdump** is a lightweight, text-based, open-source command-line network protocol analyzer that uses the **libpcap** library.

Tcpdump can capture and display key details about network traffic directly in the terminal, including:

- Source IP address
- Destination IP address
- Source port
- Destination port
- Packet timestamps

## Interpreting Tcpdump Output

Tcpdump prints captured packets in the command line and can optionally save the output to a log file.

Common fields in tcpdump output include:

- **Timestamp:** The time the packet was captured, usually shown in hours, minutes, seconds, and fractions of a second.
- **Source IP:** The IP address where the packet originated.
- **Source port:** The port number where the packet originated.
- **Destination IP:** The IP address where the packet is being sent.
- **Destination port:** The port number where the packet is being sent.

## Packet Sniffing Attacks

Attackers may use packet sniffing or protocol analysis tools to gather information about a network, capture sensitive data, or manipulate traffic.

### Passive Packet Sniffing

**Passive packet sniffing** is when an attacker reads data packets while they are in transit without changing the traffic.

### Active Packet Sniffing

**Active packet sniffing** is when an attacker manipulates or alters data packets while they are in transit.

## Preventing Malicious Packet Sniffing

Ways to reduce the risk of malicious packet sniffing include:

- **Use a VPN:** VPNs encrypt and encapsulate data across networks.
- **Use HTTPS:** HTTPS uses SSL/TLS to help encrypt web traffic.
- **Avoid unprotected networks:** Public or unsecured networks increase the risk of interception.

## IP Spoofing

**IP spoofing** is a network attack where an attacker changes the source IP address of a data packet to impersonate an authorized system and gain access to a network.

## Common IP Spoofing Attacks

### On-Path Attack

An **on-path attack** occurs when a malicious actor places themselves between two authorized devices or systems and intercepts or alters data in transit.

For example, an attacker may position themselves between a userâs device and a web server. By learning the IP and MAC addresses involved, the attacker can attempt to impersonate one or both authorized devices.

### Replay Attack

A **replay attack** occurs when a malicious actor intercepts a data packet in transit and delays it or repeats it later.

Attackers may use replay attacks to disrupt a connection or impersonate an authorized user by resending valid network traffic.

### Smurf Attack

A **Smurf attack** is a network attack where an attacker spoofs a victimâs IP address and floods the victim with ICMP traffic.

## Protecting Against IP Spoofing

Key ways to reduce the risk of IP spoofing include:

- Use VPNs and encryption to protect traffic.
- Configure firewalls to allow traffic only from trusted devices or IP addresses.
- Configure firewalls to reject traffic from external devices using internal local-network IP addresses.

## Key Takeaways

- Network attacks can expose sensitive data, disrupt business operations, and damage an organizations reputation.
- DoS and DDoS attacks attempt to overwhelm systems with traffic or requests.
- Packet sniffing can be used for legitimate network investigation or malicious data theft.
- Tcpdump is a command-line tool used to capture and analyze network traffic.
- IP spoofing allows attackers to impersonate trusted devices by changing the source IP address of packets.
- Encryption, VPNs, HTTPS, firewall rules, and avoiding unsecured networks can help protect against interception and spoofing attacks.

