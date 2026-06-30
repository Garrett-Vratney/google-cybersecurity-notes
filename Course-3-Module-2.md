# Course 3 — Module 2
# Network Protocols & Secure Network Communication

## Overview

This module introduces the core network protocols that power modern networking and cybersecurity. It covers:

- Network protocols
- Communication, management, and security protocols
- Common TCP/IP protocols
- VPNs
- Wireless security standards
- Firewalls
- Network segmentation
- Security zones
- Proxy servers
- Subnetting

---

# Network Protocols

## Definition

A **network protocol** is a set of rules that defines how devices communicate across a network.

Protocols specify:

- How data is formatted
- When data is sent
- Where data is delivered
- How receiving devices process incoming packets

Think of protocols as the instructions attached to every packet that tell devices how to communicate.

---

# Categories of Network Protocols

Network protocols generally fall into three categories:

## 1. Communication Protocols

Govern how devices exchange information.

Examples:

- TCP
- UDP
- HTTP
- DNS
- SMTP

---

## 2. Management Protocols

Used to monitor, troubleshoot, and manage networks.

Examples:

- ICMP
- SNMP
- DHCP

---

## 3. Security Protocols

Protect data while it is being transmitted.

Examples:

- HTTPS
- IPSec
- SSL/TLS
- SSH
- SFTP

---

# Communication Protocols

## TCP (Transmission Control Protocol)

**Definition**

A reliable transport-layer protocol that establishes a connection before transmitting data.

### Characteristics

- Connection-oriented
- Reliable
- Guarantees packet delivery
- Detects transmission errors
- Operates at the **Transport Layer**

---

## UDP (User Datagram Protocol)

**Definition**

A transport-layer protocol that sends data without establishing a connection.

### Characteristics

- Connectionless
- Faster than TCP
- Lower overhead
- No delivery guarantees
- Commonly used for:
  - Streaming
  - Gaming
  - Voice over IP

---

## HTTP (Hypertext Transfer Protocol)

Application-layer protocol used for communication between web browsers and web servers.

- Port **80**
- Not encrypted
- Used for standard web traffic

---

## HTTPS (Hypertext Transfer Protocol Secure)

Secure version of HTTP.

### Features

- Uses SSL/TLS encryption
- Encrypts all web traffic
- Protects confidentiality and integrity

- Port **443**
- Application Layer

---

## DNS (Domain Name System)

Translates domain names into IP addresses.

Example:

```
google.com
↓

142.250.xxx.xxx
```

Occurs at the Application Layer.

---

# Management Protocols

## SNMP (Simple Network Management Protocol)

Used to monitor and manage network devices.

Capabilities include:

- Monitor bandwidth
- Reset passwords
- Modify configurations
- Monitor device health

Application Layer

---

## ICMP (Internet Control Message Protocol)

Used to report network errors and troubleshoot connectivity.

Common uses:

- Ping
- Traceroute
- Latency testing

Occurs at the Internet Layer.

---

## DHCP (Dynamic Host Configuration Protocol)

Automatically assigns:

- IP addresses
- DNS servers
- Default gateways

Ports:

- UDP 67 (Server)
- UDP 68 (Client)

Application Layer

---

# Security Protocols

## SFTP (Secure File Transfer Protocol)

Securely transfers files using SSH.

- TCP Port 22
- Encrypted
- Frequently used with cloud storage

---

## SSH (Secure Shell)

Secure protocol used to remotely administer systems.

Features:

- Authentication
- Encryption
- Remote command execution

TCP Port 22

---

# Additional Network Protocols

## ARP (Address Resolution Protocol)

Maps an IP address to a MAC address.

Used when:

- IP address is known
- MAC address is unknown

Occurs at the Network Access Layer.

---

## NAT (Network Address Translation)

Allows multiple devices using private IP addresses to share a single public IP address.

Benefits:

- Conserves IPv4 addresses
- Hides internal network structure
- Provides basic security

Typically performed by routers or firewalls.

---

### Private IP Ranges

```
10.0.0.0 – 10.255.255.255

172.16.0.0 – 172.31.255.255

192.168.0.0 – 192.168.255.255
```

---

### Public IP Addresses

Assigned by:

- ISP
- IANA

Unique across the Internet.

---

# Remote Access Protocols

## Telnet

Remote administration protocol.

Characteristics:

- TCP Port 23
- Sends data in plaintext
- Not secure
- Mostly obsolete

---

## SSH

Preferred replacement for Telnet.

Advantages:

- Encrypted
- Authenticated
- Secure remote administration

TCP Port 22

---

# Email Protocols

## POP3

Downloads emails onto a local device.

Characteristics:

- Stores mail locally
- May remove mail from server
- TCP 110 (unencrypted)
- TCP 995 (SSL/TLS)

---

## IMAP

Synchronizes email across multiple devices.

Characteristics:

- Emails remain on the server
- Ideal for phones and multiple devices

Ports:

- TCP 143
- TCP 993 (TLS)

---

## SMTP

Transfers outgoing email.

Responsible for:

- Sending mail
- Routing mail
- DNS lookups for mail servers

Ports:

- TCP 25
- TCP 587 (TLS)

---

# Ports

Port numbers tell a receiving device which service should process incoming data.

Examples:

| Port | Protocol |
|-------|----------|
|22|SSH / SFTP|
|23|Telnet|
|25|SMTP|
|67|DHCP Server|
|68|DHCP Client|
|80|HTTP|
|110|POP3|
|143|IMAP|
|443|HTTPS|
|587|SMTP (TLS)|
|993|IMAP (TLS)|
|995|POP3 (TLS)|

Firewalls frequently filter traffic based on these ports.

---

# Wireless Networking

## IEEE 802.11 (Wi-Fi)

Defines wireless networking standards for LANs.

---

# Wi-Fi Security Standards

## WEP

- Released 1999
- Obsolete
- Easily cracked
- No longer recommended

---

## WPA

Released 2003.

Improvements:

- TKIP encryption
- Better key management
- Message Integrity Checks

Still vulnerable to KRACK attacks.

---

## WPA2

Current industry standard.

Uses:

- AES encryption
- CCMP

Available in:

- Personal
- Enterprise

Still susceptible to KRACK.

---

## WPA3

Newest Wi-Fi security protocol.

Advantages:

- SAE authentication
- Stronger encryption
- Resistant to KRACK attacks
- 128-bit encryption
- Enterprise supports 192-bit encryption

---

# Firewalls

## Definition

A firewall monitors and filters incoming and outgoing network traffic.

---

## Hardware Firewall

- Physical appliance
- Protects an entire network

---

## Software Firewall

- Installed on a computer
- Protects individual devices

---

## Cloud Firewall

Firewall hosted by a cloud provider.

---

## Stateful Firewall

Tracks active connections.

Can:

- Detect suspicious behavior
- Filter based on connection state

---

## Stateless Firewall

Uses predefined rules only.

Characteristics:

- Faster
- Less intelligent
- Less secure

---

## Next-Generation Firewall (NGFW)

Adds advanced capabilities including:

- Deep Packet Inspection (DPI)
- Intrusion Prevention Systems (IPS)
- Threat Intelligence
- Stateful inspection

---

# Virtual Private Networks (VPN)

## Definition

A VPN encrypts network traffic and hides a user's public IP address.

Benefits:

- Privacy
- Secure communication
- Safe use of public Wi-Fi

---

## Encapsulation

VPNs wrap encrypted packets inside additional packets so routers can forward them while keeping the contents private.

---

## VPN Types

### Remote Access VPN

Connects an individual user to a VPN server.

Ideal for:

- Remote employees
- Personal VPN services

---

### Site-to-Site VPN

Connects entire networks together.

Commonly uses:

- IPSec

Best for organizations with multiple offices.

---

## WireGuard vs IPSec

### WireGuard

- Faster
- Lightweight
- Modern encryption
- Simpler configuration

### IPSec

- Older
- Widely supported
- More complex
- Common in enterprise networks

---

# Security Zones

Security zones divide networks into isolated sections.

Benefits:

- Prevent lateral movement
- Limit damage
- Improve access control

---

## Uncontrolled Zone

External networks outside organizational control.

Example:

- Internet

---

## Controlled Zone

Protected internal network.

Includes:

- DMZ
- Internal Network
- Restricted Network

---

## DMZ (Demilitarized Zone)

Hosts public-facing services such as:

- Web servers
- DNS servers
- Email servers
- Proxy servers

---

## Restricted Zone

Contains highly sensitive resources.

Accessible only by authorized users.

---

# Network Segmentation

Divides a large network into smaller secure subnetworks.

Benefits:

- Improved security
- Better performance
- Easier incident containment

Example:

Student network separated from faculty network.

---

# Subnetting

Creates smaller subnetworks from one large network.

Benefits:

- Better organization
- Reduced broadcast traffic
- Improved performance

---

## CIDR (Classless Inter-Domain Routing)

Modern subnet addressing method.

Example:

```
192.168.1.0/24
```

Benefits:

- Conserves IP addresses
- Smaller routing tables
- Flexible subnet creation

---

# Proxy Servers

A proxy server sits between users and the Internet.

Functions:

- Filters traffic
- Hides IP addresses
- Caches frequently requested data
- Blocks malicious websites

---

## Forward Proxy

Protects users.

Used for:

- Web filtering
- Internet access control
- Hiding client IP addresses

---

## Reverse Proxy

Protects servers.

Benefits:

- Hides internal servers
- Filters incoming requests
- Improves security

---

## Email Proxy

Filters:

- Spam
- Spoofed email
- Phishing attempts

---

# Key Takeaways

- Network protocols define how devices communicate.
- Communication, management, and security protocols each serve different purposes.
- Port numbers determine which services receive incoming traffic.
- HTTPS encrypts web traffic using SSL/TLS.
- VPNs encrypt all network traffic and hide a user's IP address.
- Firewalls inspect and filter network traffic.
- WPA3 is the most secure modern Wi-Fi standard.
- Network segmentation and subnetting improve both security and performance.
- Proxy servers help filter traffic and protect internal systems.
