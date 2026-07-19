\# Address Resolution Protocol (ARP)



\## Overview



ARP stands for:



\*\*Address Resolution Protocol\*\*



ARP is a networking protocol used to map an \*\*IP address\*\* to a \*\*MAC address\*\* on a local network.



Devices use ARP because communication on a local network requires knowing the physical address (MAC address) of the destination device.



\---



\# IP Address vs MAC Address



Devices on a network use two different types of identifiers.



| Identifier | Purpose |

|---|---|

| IP Address | Logical address used to identify a device on a network |

| MAC Address | Physical address used to identify a network interface |



Example:



```

IP Address:

192.168.1.50



MAC Address:

00:1A:2B:3C:4D:5E

```



The IP address identifies \*\*where the device is logically located\*\*, while the MAC address identifies the \*\*physical network interface\*\*.



\---



\# Why ARP Is Needed



When a device wants to communicate with another device on the same network, it knows the destination IP address but may not know the MAC address.



Example:



A computer wants to communicate with:



```

192.168.1.25

```



The computer knows the IP address but needs the MAC address before it can send Ethernet traffic.



ARP solves this problem by discovering the MAC address associated with that IP address.



\---



\# ARP Cache



Every device maintains an ARP cache.



The ARP cache stores previously discovered IP-to-MAC address mappings.



Example:



| IP Address | MAC Address |

|-|-|

|192.168.1.25|00:1A:2B:3C:4D:5E|

|192.168.1.50|00:AA:BB:CC:DD:EE|



This allows devices to communicate faster because they do not need to ask for the MAC address every time.



\---



\# How ARP Works



ARP uses two main message types:



1\. ARP Request

2\. ARP Reply



\---



\# ARP Request



When a device does not know the MAC address for an IP address, it sends an ARP request.



The request is broadcast across the local network.



Example:



```

Who has 192.168.1.25?



Tell 192.168.1.10

```



Every device on the network receives this request.



Only the device with that IP address responds.



\---



\# ARP Reply



The device that owns the requested IP address sends an ARP reply.



Example:



```

192.168.1.25 is at:



00:1A:2B:3C:4D:5E

```



The requesting device stores this information in its ARP cache.



\---



\# ARP Process



The process looks like this:



```

Device A wants to communicate with Device B



&#x20;       |

&#x20;       v



ARP Request:

"What MAC address owns this IP?"



&#x20;       |

&#x20;       v



Device B replies:



"That IP belongs to this MAC address"



&#x20;       |

&#x20;       v



Device A stores the mapping in ARP cache

```



\---



\# ARP Example



A computer:



```

IP:

192.168.1.10

```



wants to communicate with:



```

IP:

192.168.1.20

```



The computer checks its ARP cache.



If no entry exists:



1\. Sends ARP Request

2\. Destination device replies

3\. MAC address is stored

4\. Communication begins



\---



\# Cybersecurity Relevance



ARP is important in cybersecurity because it operates through trust.



Devices generally accept ARP responses without authentication.



This can create security risks.



\---



\# ARP Spoofing



ARP spoofing is an attack where an attacker sends fake ARP messages to associate their MAC address with another device's IP address.



Example:



Normal:



```

192.168.1.1 → Router MAC Address

```



After spoofing:



```

192.168.1.1 → Attacker MAC Address

```



Traffic intended for the router may then be redirected through the attacker.



\---



\# Defending Against ARP Attacks



Security controls include:



\- Dynamic ARP Inspection (DAI)

\- Network segmentation

\- Monitoring ARP activity

\- Using secure network configurations



\---



\# Key Takeaways



\- ARP maps IP addresses to MAC addresses.

\- MAC addresses identify physical network interfaces.

\- ARP requests are broadcast across local networks.

\- ARP replies provide the requested MAC address.

\- Devices store mappings in an ARP cache.

\- ARP does not provide authentication, creating security risks.

\- ARP spoofing can be used to manipulate network traffic.

