# Network Topologies

## Overview

A network topology describes the physical or logical arrangement of devices within a network.

It defines how devices are connected, how data travels, and how failures affect the network.

Common network topologies include:

- Star Topology
- Bus Topology
- Ring Topology

---

# Star Topology

## Overview

A star topology connects each device individually to a central networking device, usually a switch.

Example:

```
        PC
        |
PC ---- Switch ---- PC
        |
        PC
```

Most modern networks use star topology because of its reliability and scalability.

---

## Advantages

### Easy to Expand

Additional devices can be connected by adding more ports or switches.

### Easier Troubleshooting

Because devices have individual connections, faults can often be isolated quickly.

### Reduced Impact of Device Failure

If one computer fails, other devices can continue communicating.

---

## Disadvantages

### Cost

Star topology requires:

- More cabling
- Dedicated networking equipment such as switches

This makes it more expensive compared to simpler topologies.

### Central Device Dependency

If the central switch or hub fails, connected devices may lose network access.

### Maintenance

Larger star networks require more management and maintenance.

---

# Bus Topology

## Overview

A bus topology uses a single connection known as a **backbone cable**.

All devices connect to this main cable and data travels along the same communication path.

Example:

```
PC ---- PC ---- PC ---- PC
        |
    Backbone Cable
```

Bus topology is similar to branches connected to a single tree trunk.

---

## Advantages

### Low Cost

Bus topology requires:

- Less cabling
- Less networking equipment

This makes it inexpensive compared to other topologies.

---

## Disadvantages

### Network Bottlenecks

Because all devices share the same communication cable, heavy traffic can cause:

- Slow performance
- Data collisions
- Reduced network efficiency

### Difficult Troubleshooting

Since all communication uses the same cable, locating faults can be difficult.

### Single Point of Failure

If the backbone cable fails, devices may no longer be able to communicate.

### Limited Scalability

Adding more devices increases traffic and reduces performance.

---

# Ring Topology

## Overview

A ring topology connects devices together to form a circular network.

Each device connects directly to two other devices, creating a loop.

Example:

```
PC → PC → PC → PC
↑             ↓
└─────────────┘
```

Ring topology is sometimes called a **token topology** because some ring networks use token passing to control access to the network.

---

## How Ring Topology Works

Data travels around the loop until it reaches its intended destination.

Each device forwards data to the next device.

If a device has its own data to send, it sends its data before forwarding other traffic.

---

## Advantages

### Predictable Traffic

Because data travels in one direction, there is less chance of collisions compared to bus topology.

### Easier Fault Detection

A break in the ring can help identify where a failure has occurred.

### Less Hardware Required

Ring networks require less cabling and less dedicated equipment compared to star topology.

---

## Disadvantages

### Single Failure Impact

A damaged cable or failed device can interrupt communication across the entire network.

### Slower Communication

Data may need to travel through multiple devices before reaching its destination.

### Limited Scalability

Adding more devices increases the distance data must travel.

---

# Topology Comparison

| Topology | Advantages | Disadvantages |
|---|---|---|
| Star | Reliable, scalable, easy troubleshooting | Expensive, central device failure affects network |
| Bus | Cheap, simple design | Slow under heavy traffic, backbone failure affects network |
| Ring | Predictable traffic, fewer collisions | Device/cable failure can break network |

---

# Cybersecurity Relevance

Understanding network topology helps security professionals understand:

- How data flows through a network
- Where single points of failure exist
- Where security controls should be placed
- How attackers may move through a network

For example:

- A star topology may have a critical switch that needs protection.
- A bus topology may allow easier traffic interception because communication shares one medium.
- A poorly secured network design can increase the impact of attacks.