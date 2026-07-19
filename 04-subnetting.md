# Subnetting

## Overview

Subnetting is the process of dividing a larger network into smaller networks called **subnets**.

Think of subnetting like dividing a large organisation into different departments.

Instead of every device existing on one large network, subnetting allows networks to be separated into smaller sections.

---

# Why Subnetting Is Used

Subnetting provides several benefits:

- Improved network organisation
- Better performance
- Increased security
- Easier management
- More efficient use of IP addresses

---

# Example: Business Networks

A business may have many different types of devices:

- Employee computers
- Servers
- Printers
- Security cameras
- Guest Wi-Fi devices

Instead of putting everything on one network, subnetting allows separation.

Example:

```
Company Network

        |
 -----------------
 |       |        |
Staff   Servers  Guest Wi-Fi
```

This improves security because different groups of devices can be isolated from each other.

---

# IPv4 Addresses

IPv4 addresses are used to identify devices on a network.

Example:

```
192.168.1.100
```

An IPv4 address contains four sections called **octets**.

Example:

```
192 . 168 . 1 . 100
 |     |    |    |
Octet Octet Octet Octet
```

Each octet represents 8 bits, making IPv4 addresses 32 bits in total.

---

# Subnet Masks

A subnet mask determines which part of an IP address identifies:

- The network
- The host/device

Example:

IP Address:

```
192.168.1.100
```

Subnet Mask:

```
255.255.255.0
```

This means:

Network:

```
192.168.1.0
```

Host:

```
100
```

---

# Network Address

The network address identifies the beginning of a network.

Example:

Device IP:

```
192.168.1.100
```

Network address:

```
192.168.1.0
```

All devices with:

```
192.168.1.x
```

belong to the same network.

---

# Host Address

The host address identifies an individual device inside a network.

Example:

```
192.168.1.100
```

The host portion is:

```
100
```

This identifies the specific device.

Examples:

```
192.168.1.10
192.168.1.20
192.168.1.50
```

Each represents a different host on the same network.

---

# Default Gateway

The default gateway is a device responsible for sending traffic outside of the local network.

Usually, this is a router.

Example:

Local network:

```
192.168.1.0
```

A computer wants to access the internet.

The traffic is sent to the:

```
Default Gateway
```

which forwards it to another network.

---

# Small Home Networks

Most home networks use a single subnet.

Example:

```
192.168.1.0/24
```

A `/24` network provides:

```
254 usable host addresses
```

This is usually enough because homes rarely need hundreds of connected devices.

---

# Business Networks

Businesses often require multiple subnets because they have many devices.

Example:

```
Company Network

192.168.1.0/24
|
├── Employees
|
├── Servers
|
└── Guest Network
```

---

# Security Benefits of Subnetting

Subnetting improves security by separating different parts of a network.

Example:

A café may have two networks:

## Employee Network

Used by:

- Staff computers
- Payment systems
- Internal devices

## Guest Network

Used by:

- Customers
- Public internet access

Subnetting prevents guest devices from directly accessing sensitive internal systems.

---

# Subnetting and Cybersecurity

Understanding subnetting helps security professionals with:

- Network enumeration
- Identifying hosts
- Understanding network boundaries
- Firewall configuration
- Security monitoring
- Attack surface analysis

During penetration testing, knowing the network structure helps identify:

- Available targets
- Segmented networks
- Potential paths for lateral movement

---

# Key Terms

| Term | Meaning |
|-|-|
| IP Address | Logical address used to identify a device |
| MAC Address | Physical address of a network interface |
| Subnet | Smaller network created from a larger network |
| Subnet Mask | Determines network and host portions |
| Network Address | Identifies the network |
| Host Address | Identifies a specific device |
| Default Gateway | Device used to communicate with other networks |

---

# Key Takeaways

- Subnetting divides large networks into smaller networks.
- IP addresses contain network and host information.
- Subnet masks determine which part belongs to each.
- Routers are commonly used as default gateways.
- Businesses use subnetting for organisation, efficiency, and security.
- Network segmentation reduces the impact of security incidents.