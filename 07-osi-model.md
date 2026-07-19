\# OSI Model (Open Systems Interconnection Model)



\## Overview



The \*\*OSI Model\*\* stands for:



\*\*Open Systems Interconnection Model\*\*



The OSI model is a framework used to describe how data travels across a network.



It explains how devices communicate by separating network communication into seven different layers.



Each layer has a specific responsibility and works together to allow data to be transmitted, received, and understood.



\---



\# Why the OSI Model Is Important



The OSI model provides a standard way for different devices, applications, and networking technologies to communicate.



Benefits include:



\- Easier troubleshooting

\- Better understanding of network communication

\- Standardisation between different systems

\- Clear separation of networking responsibilities



\---



\# The Seven Layers



The OSI model consists of seven layers:



| Layer | Name |

|---|---|

|7|Application|

|6|Presentation|

|5|Session|

|4|Transport|

|3|Network|

|2|Data Link|

|1|Physical|



Data travels down the layers when being sent and moves back up the layers when being received.



\---



\# Encapsulation



\## Overview



Encapsulation is the process where information is added to data as it moves through each layer of the OSI model.



Each layer adds its own information required for communication.



Example:



```

Application Data

&#x20;       ↓

Transport Segment

&#x20;       ↓

Network Packet

&#x20;       ↓

Data Link Frame

&#x20;       ↓

Physical Bits

```



When data reaches the receiving device, the process is reversed. This is called \*\*de-encapsulation\*\*.



\---



\# Layer 1 - Physical Layer



\## Overview



The Physical Layer is the lowest layer of the OSI model.



It is responsible for the physical transmission of data using hardware components.



Data is transmitted as:



```

Binary signals (1s and 0s)

```



\---



\## Examples



Physical components include:



\- Ethernet cables

\- Fibre optic cables

\- Wireless signals

\- Network connectors



\---



\## Cybersecurity Relevance



Security considerations include:



\- Physical access to networking equipment

\- Cable security

\- Device theft

\- Hardware tampering



\---



\# Layer 2 - Data Link Layer



\## Overview



The Data Link Layer focuses on physical addressing and communication between devices on the same network.



This layer uses:



```

MAC Addresses

```



Every network interface card (NIC) has a unique MAC address.



\---



\## Responsibilities



The Data Link Layer:



\- Adds MAC addresses to data

\- Creates frames

\- Controls local network communication

\- Detects transmission errors



\---



\## Example



A computer wants to send data to another device on the same network.



The Data Link Layer adds the destination MAC address so the switch knows where to send the frame.



\---



\## Devices



Common Layer 2 devices:



\- Switches

\- Network Interface Cards



\---



\## Cybersecurity Relevance



Security issues include:



\- MAC spoofing

\- ARP attacks

\- Switch-based attacks



\---



\# Layer 3 - Network Layer



\## Overview



The Network Layer is responsible for routing data between different networks.



This layer uses:



```

IP Addresses

```



\---



\## Responsibilities



The Network Layer handles:



\- Routing

\- Packet forwarding

\- Logical addressing



\---



\## Routing



Routing is the process of selecting the best path for data to travel.



Routers consider factors such as:



\- Shortest path

\- Reliability

\- Connection speed



\---



\## Routing Protocol Examples



Examples include:



\- OSPF (Open Shortest Path First)

\- RIP (Routing Information Protocol)



\---



\## Devices



Layer 3 devices:



\- Routers

\- Layer 3 switches



\---



\## Cybersecurity Relevance



Security considerations include:



\- Firewall rules

\- Network segmentation

\- IP-based attacks

\- Routing manipulation



\---



\# Layer 4 - Transport Layer



\## Overview



The Transport Layer is responsible for delivering data between devices.



The two main protocols are:



\- TCP

\- UDP



\---



\# TCP (Transmission Control Protocol)



\## Overview



TCP focuses on reliability and accuracy.



TCP creates a connection between two devices before sending data.



\---



\## Features



TCP provides:



\- Error checking

\- Guaranteed delivery

\- Data ordering

\- Flow control



\---



\## Advantages



\- Reliable communication

\- Ensures data arrives correctly

\- Prevents data loss



\---



\## Disadvantages



\- Slower than UDP

\- Requires more processing

\- Requires a connection



\---



\## Uses



TCP is commonly used for:



\- Web browsing (HTTPS)

\- Email

\- File transfers



\---



\# UDP (User Datagram Protocol)



\## Overview



UDP focuses on speed rather than reliability.



UDP sends data without creating a connection or confirming delivery.



\---



\## Advantages



\- Faster than TCP

\- Lower overhead

\- Useful for real-time communication



\---



\## Disadvantages



\- No guarantee data arrives

\- No error correction

\- Packet loss can occur



\---



\## Uses



UDP is commonly used for:



\- Online gaming

\- Video streaming

\- Voice communication

\- DNS



\---



\## Cybersecurity Relevance



Understanding TCP and UDP helps security professionals analyse:



\- Network traffic

\- Open ports

\- Firewall rules

\- Suspicious connections



\---



\# Layer 5 - Session Layer



\## Overview



The Session Layer manages communication sessions between applications.



A session is a connection between two devices that allows data exchange.



\---



\## Responsibilities



The Session Layer:



\- Creates sessions

\- Maintains sessions

\- Terminates sessions



It can also create checkpoints so communication can resume if interrupted.



\---



\## Cybersecurity Relevance



Security concerns include:



\- Session hijacking

\- Unauthorised access to active sessions



\---



\# Layer 6 - Presentation Layer



\## Overview



The Presentation Layer is responsible for formatting and translating data.



It ensures that different systems can understand information being exchanged.



\---



\## Responsibilities



The Presentation Layer handles:



\- Data formatting

\- Encryption

\- Compression

\- Translation



\---



\## Example



Different email applications may display messages differently, but the data format must still be understood.



\---



\## Cybersecurity Relevance



Encryption technologies such as:



\- TLS

\- HTTPS



are associated with protecting data during communication.



\---



\# Layer 7 - Application Layer



\## Overview



The Application Layer is the layer closest to the user.



It allows applications to interact with network services.



\---



\## Examples



Applications include:



\- Web browsers

\- Email clients

\- File transfer applications



\---



\## Common Protocols



Examples:



| Protocol | Purpose |

|-|-|

|HTTP/HTTPS|Web communication|

|DNS|Translates domain names into IP addresses|

|FTP|File transfer|

|SMTP|Email|



\---



\## Cybersecurity Relevance



Security issues include:



\- Web vulnerabilities

\- Phishing

\- Application attacks

\- Malicious services



\---



\# OSI Layer Summary



| Layer | Name | Main Function |

|-|-|-|

|7|Application|User applications and services|

|6|Presentation|Formatting and encryption|

|5|Session|Creates and manages connections|

|4|Transport|Reliable data delivery|

|3|Network|Routing and IP addressing|

|2|Data Link|MAC addressing|

|1|Physical|Hardware and signals|



\---



\# Key Takeaways



\- The OSI model explains how network communication works.

\- Each layer has a specific responsibility.

\- Data is encapsulated as it moves through the layers.

\- Lower layers focus on moving data.

\- Higher layers focus on applications and user interaction.

\- Understanding the OSI model is essential for networking, troubleshooting, and cybersecurity.

