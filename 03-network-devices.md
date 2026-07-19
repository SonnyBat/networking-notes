# Network Devices

## Overview

Network devices are hardware components that allow computers, servers, and other systems to communicate with each other.

Different network devices operate at different layers of the OSI model and perform different roles within a network.

Common network devices include:

- Network Interface Cards (NICs)
- Hubs
- Switches
- Routers

---

# Network Interface Card (NIC)

## Overview

A Network Interface Card (NIC) is a hardware component that allows a device to connect to a network.

Every NIC has a unique:

```
MAC Address
```

which acts as the physical identifier of the device on a network.

---

## MAC Addresses

MAC stands for:

**Media Access Control**

A MAC address is assigned to a NIC by the manufacturer.

Example:

```
00:1A:2B:3C:4D:5E
```

MAC addresses operate at:

```
Layer 2 - Data Link Layer
```

of the OSI model.

---

## Cybersecurity Relevance

MAC addresses are important when:

- Identifying devices on a network
- Investigating network traffic
- Analysing ARP communications

MAC addresses can also be spoofed, meaning attackers may impersonate another device.

---

# Hub

## Overview

A hub is a basic networking device that connects multiple devices together.

When a hub receives data, it broadcasts the data to every connected device.

Example:

```
Computer
   |
  Hub
 / | \
PC PC PC
```

---

## Disadvantages

### Increased Network Traffic

Because hubs send data to every connected device, unnecessary traffic is created.

### Security Issues

All devices receive the transmitted data, making traffic easier to intercept.

### No Intelligence

A hub does not know which device should receive the data.

---

## Hub vs Switch

| Hub | Switch |
|-|-|
| Sends data to every device | Sends data only to intended device |
| Less efficient | More efficient |
| Creates more traffic | Reduces network traffic |
| Older technology | Common in modern networks |

---

# Switch

## Overview

A switch is a networking device that connects multiple devices together using Ethernet connections.

Common devices connected to switches include:

- Computers
- Printers
- Servers
- Access points
- Other networking equipment

Switches are commonly found in:

- Businesses
- Schools
- Data centres

---

## How Switches Work

Unlike hubs, switches keep track of which device is connected to which port.

When a switch receives a packet, it checks its MAC address table and forwards the data only to the intended destination.

This reduces unnecessary network traffic.

---

## Example

A computer connected to:

```
Port 1
```

wants to communicate with a printer connected to:

```
Port 5
```

The switch knows the printer is on port 5 and forwards the data directly there.

---

## Advantages

### Efficiency

Switches reduce network traffic by avoiding unnecessary broadcasts.

### Scalability

Multiple devices can be connected through many available ports.

### Improved Performance

Dedicated communication paths allow devices to communicate more efficiently.

---

## Disadvantages

### Cost

Switches are more expensive than hubs.

### Configuration

Managed switches require administration and maintenance.

---

## OSI Model Layer

Switches primarily operate at:

```
Layer 2 - Data Link Layer
```

because they use MAC addresses to forward traffic.

Some advanced switches can also operate at:

```
Layer 3 - Network Layer
```

using IP addresses.

---

# Router

## Overview

A router is a networking device responsible for connecting different networks together.

Routers forward data between networks using IP addresses.

Example:

```
Home Network
      |
    Router
      |
  Internet
```

---

## Routing

Routing is the process of selecting a path for data to travel between networks.

Routers examine destination IP addresses and determine where data should be sent.

---

## Example

A device on:

```
192.168.1.0
```

wants to communicate with a server on another network.

The router receives the traffic and forwards it towards the destination network.

---

## Router Responsibilities

Routers:

- Connect different networks
- Forward packets
- Choose routes
- Separate network segments

---

## OSI Model Layer

Routers operate at:

```
Layer 3 - Network Layer
```

because they use IP addresses to route traffic.

---

# Switches vs Routers

| Switch | Router |
|-|-|
| Connects devices within the same network | Connects different networks |
| Uses MAC addresses | Uses IP addresses |
| Layer 2 device | Layer 3 device |
| Creates local network connections | Provides communication between networks |

---

# Network Redundancy

Networks can improve reliability by using multiple connections between devices.

For example:

```
Network A
    |
Switch
    |
Network B
```

Multiple paths allow traffic to continue if one connection fails.

However, additional paths can increase complexity and require proper configuration.

---

# Cybersecurity Relevance

Understanding network devices is essential because security professionals need to understand:

- Where traffic flows
- Where security controls are placed
- How attackers move through networks
- Where vulnerabilities may exist

Examples:

- Misconfigured routers can expose networks.
- Poor switch security can allow unauthorised access.
- Unprotected network devices can become entry points for attackers.