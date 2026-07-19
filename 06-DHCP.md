# Dynamic Host Configuration Protocol (DHCP)

## Overview

DHCP stands for:

**Dynamic Host Configuration Protocol**

DHCP is a network protocol that automatically assigns IP addresses and other network configuration information to devices.

Without DHCP, every device would need to be manually configured with:

- IP address
- Subnet mask
- Default gateway
- DNS server

---

# Static vs Dynamic IP Addresses

## Static IP Address

A static IP address is manually assigned to a device.

Example uses:

- Servers
- Network devices
- Security systems

Advantages:

- Address stays the same
- Easier to locate important devices

Disadvantages:

- Requires manual configuration
- More difficult to manage on large networks

---

## Dynamic IP Address

A dynamic IP address is automatically assigned by a DHCP server.

Advantages:

- Easier to manage
- Automatically configures new devices
- Reduces configuration errors

This is the most common method used on home and business networks.

---

# DHCP Components

A DHCP process involves:

## DHCP Client

The device requesting network information.

Examples:

- Laptop
- Phone
- Desktop computer

---

## DHCP Server

The device responsible for assigning network configuration.

Examples:

- Router
- Dedicated server

---

# How DHCP Works

DHCP uses a four-step process called:

```
DORA
```

DORA stands for:

1. DHCP Discover
2. DHCP Offer
3. DHCP Request
4. DHCP ACK

---

# 1. DHCP Discover

The device first connects to the network but does not have an IP address.

It sends a broadcast message asking:

```
"Are there any DHCP servers available?"
```

Example:

```
Client → Broadcast → DHCP Server
```

---

# 2. DHCP Offer

The DHCP server receives the request and responds with an available IP address.

Example:

```
DHCP Server:

"You can use 192.168.1.50"
```

The offer may also include:

- Subnet mask
- Default gateway
- DNS server

---

# 3. DHCP Request

The client responds to the DHCP server confirming it wants to use the offered IP address.

Example:

```
Client:

"I would like to use 192.168.1.50"
```

---

# 4. DHCP ACK

ACK stands for:

**Acknowledgement**

The DHCP server sends a final confirmation.

The device can now use the assigned network configuration.

Example:

```
DHCP Server:

"192.168.1.50 has been assigned successfully"
```

---

# DHCP Process Diagram

```
Client

   |
   | DHCP Discover
   v

DHCP Server

   |
   | DHCP Offer
   v

Client

   |
   | DHCP Request
   v

DHCP Server

   |
   | DHCP ACK
   v

Client receives IP address
```

---

# DHCP Leases

DHCP does not usually assign IP addresses permanently.

Instead, devices receive a lease.

A lease means:

"The device can use this IP address for a set amount of time."

Before the lease expires, the device can request to renew the address.

---

# Example Home Network

A home router often acts as a DHCP server.

Example:

Router:

```
DHCP Range:
192.168.1.100 - 192.168.1.200
```

Connected devices receive addresses automatically:

```
Laptop:
192.168.1.101

Phone:
192.168.1.102

Console:
192.168.1.103
```

---

# Cybersecurity Relevance

DHCP is important in cybersecurity because it controls how devices join a network.

Security risks include:

---

# Rogue DHCP Servers

A rogue DHCP server is an unauthorised DHCP server placed on a network.

An attacker could provide false network information such as:

- Incorrect gateway
- Malicious DNS server
- Incorrect IP configuration

This can redirect traffic or interfere with normal network communication.

---

# DHCP Security Controls

Security teams can reduce DHCP risks using:

- DHCP snooping
- Network segmentation
- Monitoring DHCP activity
- Access controls on network ports

---

# Key Takeaways

- DHCP automatically assigns network configuration.
- DHCP removes the need for manual IP configuration.
- The DHCP process follows DORA:
  - Discover
  - Offer
  - Request
  - ACK
- DHCP servers provide IP addresses, gateways, and DNS information.
- Devices receive IP addresses through leases.
- Rogue DHCP servers can be used to attack networks.