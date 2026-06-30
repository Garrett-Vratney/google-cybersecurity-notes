# Google Cybersecurity Professional Certificate
## Course 3 – Module 4
# Security Hardening

---

# Learning Objectives

By the end of this module, you should understand:

- Security hardening fundamentals
- Operating system (OS) hardening
- Network hardening practices
- Cloud network hardening
- Common defensive security controls

---

# Security Hardening

## Definition

**Security Hardening** is the process of strengthening a system to reduce vulnerabilities and minimize its attack surface.

### Attack Surface

The **attack surface** is every possible point where an attacker could exploit a vulnerability.

Security hardening applies to:

- Hardware
- Operating Systems
- Applications
- Computer Networks
- Databases

---

# Common Hardening Procedures

Security teams commonly strengthen systems by:

- Installing software updates and security patches
- Modifying secure configurations
- Removing unused applications and services
- Closing unnecessary network ports
- Limiting user permissions

### Examples

- Enforcing stronger password requirements
- Requiring periodic password changes
- Updating encryption standards
- Restricting unnecessary services

---

# Penetration Testing

## Definition

A **Penetration Test (Pen Test)** is a simulated cyberattack used to identify security weaknesses in:

- Networks
- Systems
- Applications
- Websites
- Security processes

### Purpose

Pen testers:

- Discover vulnerabilities
- Document findings
- Recommend security improvements

---

# Full Disk Encryption

Full disk encryption encrypts all information stored on a device.

Even if someone gains physical access, they cannot read the data without the proper decryption key or password.

---

# Operating System (OS) Hardening

OS hardening involves continuously improving the security of an operating system through:

- Regular patching
- Configuration management
- Password policies
- Access controls
- Security monitoring

---

# Patch Updates

## Definition

A **Patch Update** is a software or operating system update that fixes security vulnerabilities.

### Why Patch Quickly?

Once vendors release a patch:

- Attackers learn what vulnerability was fixed.
- Unpatched systems become easy targets.
- Organizations should update as soon as possible.

---

# Baseline Configuration (Baseline Image)

## Definition

A documented standard configuration used as the reference for future deployments and updates.

### Example

A baseline might define:

- Allowed firewall rules
- Open network ports
- Security configurations

If suspicious activity occurs, administrators compare the current system against the baseline to identify unauthorized changes.

---

# Software & Hardware Disposal

Properly dispose of:

- Old hardware
- Legacy software
- Unsupported applications

Older technology often contains known security vulnerabilities.

---

# Password Policies

Organizations strengthen security by enforcing:

- Strong passwords
- Password expiration
- Password history
- Account lockout thresholds

---

# Brute Force Attacks

## Definition

A brute force attack is a trial-and-error method attackers use to discover passwords or credentials.

### Types

## Simple Brute Force

Attackers repeatedly guess login credentials.

## Dictionary Attack

Attackers use:

- Common passwords
- Password dictionaries
- Credentials leaked during previous breaches

---

# Security Testing Environments

Security analysts often test software inside isolated environments before deploying it.

## Virtual Machines (VMs)

### Definition

Software versions of physical computers.

Benefits:

- Isolated testing
- Safe malware analysis
- Easy rollback
- Disposable environments

---

## Sandboxes

### Definition

A sandbox is an isolated environment used to safely execute software.

Uses include:

- Testing patches
- Finding bugs
- Malware analysis
- Vulnerability testing

---

# Preventing Brute Force Attacks

## Password Hashing

Hashing converts data into a one-way cryptographic value used to verify integrity.

Hashes cannot be reversed.

---

## Salting

Salting adds random data to passwords before hashing.

Benefits:

- Makes identical passwords produce different hashes
- Protects against rainbow table attacks

---

## MFA & 2FA

Multi-Factor Authentication requires multiple forms of verification before granting access.

Examples include:

- Password
- Mobile authentication app
- Hardware token
- Biometrics

---

## CAPTCHA & reCAPTCHA

CAPTCHA verifies that a user is human rather than a bot.

Google's **reCAPTCHA** provides free bot protection for websites.

---

# Network Hardening

## Core Practices

- Port filtering
- Network segmentation
- Access control
- Encryption

---

# Routine Network Maintenance

Security teams regularly perform:

- Firewall rule reviews
- Network log analysis
- Patch management
- Server backups

---

# Network Log Analysis

Network log analysis is the process of reviewing network logs to identify:

- Suspicious behavior
- Security incidents
- Performance issues

---

# Port Filtering

Firewalls allow or block traffic based on:

- Port numbers
- Protocols
- Security rules

This reduces unnecessary communication.

---

# Network Access Privileges

Organizations limit access using:

- Least privilege
- Network segmentation
- User authorization

Only authorized users access required resources.

---

# Firewalls

A firewall:

- Allows or blocks network traffic
- Uses predefined security rules
- Filters packets based on packet header information

---

# Intrusion Detection System (IDS)

An IDS:

- Monitors network activity
- Detects suspicious traffic
- Alerts administrators
- Uses attack signatures

### Limitations

- Detects known attacks
- Cannot automatically stop attacks
- May miss sophisticated threats

---

# Intrusion Prevention System (IPS)

An IPS:

- Detects malicious activity
- Automatically blocks threats
- Stops suspicious network connections

### Limitations

- False positives may interrupt legitimate traffic.

---

# Full Packet Capture

Packet capture devices:

- Record all network traffic
- Help investigate IDS alerts
- Support forensic investigations

---

# Security Information and Event Management (SIEM)

SIEM platforms:

- Collect security logs
- Correlate events
- Monitor critical systems
- Generate alerts
- Assist incident response

---

# Cloud Network Security

## Major Security Concerns

### Identity and Access Management (IAM)

IAM manages:

- Digital identities
- Authentication
- Authorization
- Access permissions

---

### Configuration Management

Cloud environments require precise configurations to maintain:

- Security
- Compliance
- Availability

Proper configuration is especially important during cloud migrations.

---

### Cloud Attack Surface

Using multiple cloud services increases the number of possible entry points.

Proper architecture minimizes this additional risk.

---

# Zero-Day Attacks

A zero-day attack exploits a vulnerability before organizations have deployed a security patch.

Cloud Service Providers (CSPs) often detect and patch these vulnerabilities faster than traditional organizations.

---

# Visibility & Monitoring

Administrators monitor cloud environments using:

- Flow logs
- Packet mirroring
- Monitoring tools

Some CSPs limit direct packet inspection and instead provide logging services or third-party security audits.

---

# Shared Responsibility Model

The Shared Responsibility Model defines security responsibilities between:

- Cloud Service Provider (CSP)
- Customer

Generally:

## CSP Responsibilities

- Physical infrastructure
- Data centers
- Hypervisors
- Host operating systems

## Customer Responsibilities

- Accounts
- Data
- Identity management
- Configurations
- Permissions

---

# Cloud Hardening

## Identity & Access Management (IAM)

Strong IAM policies reduce unauthorized access by managing:

- Users
- Roles
- Permissions

---

## Hypervisors

Hypervisors create and manage virtual machines.

### Type 1 Hypervisor

Runs directly on hardware.

Used by most cloud providers.

### Type 2 Hypervisor

Runs on top of an existing operating system.

---

# Cloud Baselining

Cloud baselines define secure default configurations.

Examples include:

- Restricting admin portal access
- Enforcing password policies
- Enabling encryption
- Monitoring configuration drift

---

# Cryptography in the Cloud

Cloud cryptography protects stored and transmitted information using encryption.

Encrypted information is stored as **ciphertext** and requires the proper key to decrypt.

---

# Cryptographic Erasure

Also called **Crypto Shredding**.

Instead of deleting encrypted data directly, organizations securely destroy the encryption keys, making the data permanently inaccessible.

---

# Key Management

Modern encryption depends on protecting encryption keys.

## Trusted Platform Module (TPM)

A hardware chip that securely stores:

- Passwords
- Encryption keys
- Certificates

---

## Cloud Hardware Security Module (CloudHSM)

CloudHSM provides:

- Secure key storage
- Encryption operations
- Decryption operations
- Cryptographic key management

---

# Key Takeaways

- Security hardening reduces vulnerabilities and minimizes attack surfaces.
- OS hardening includes patching, baselines, password policies, and secure disposal.
- Network hardening relies on firewalls, IDS/IPS, SIEM, encryption, and access control.
- Cloud security follows the Shared Responsibility Model.
- IAM, hypervisors, baselines, encryption, and key management are fundamental cloud security controls.
