# IP Addressing

## IPv4 Addresses

IPv4 addresses are used to identify devices on a network.

An IPv4 address consists of four sections called **octets**.

Example:
192.168.1.100

Each section represents 8 bits, giving IPv4 addresses a total size of 32 bits.

---

## MAC Address

MAC stands for:

**Media Access Control**

A MAC address is a physical identifier assigned to a network interface card (NIC).

Example:
00:1A:2B:3C:4D:5E

Unlike IP addresses, MAC addresses identify the physical network interface.

---

## IP vs MAC Address

| Address | Purpose |
|-|-|
| IP Address | Logical identifier used for communication across networks |
| MAC Address | Physical identifier used inside local networks |

---

## Ping

Ping is a network utility used to test connectivity between devices.

It uses:

ICMP
(Internet Control Message Protocol)

Example:

```bash
ping 8.8.8.8

Ping can help determine:

If a host is reachable
Network latency
Packet loss

