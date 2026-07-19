# TCP vs UDP

## Overview

TCP and UDP are two protocols used at the **Transport Layer (Layer 4)** of the OSI model.

Both protocols are responsible for transporting data between devices, but they handle communication differently.

The main difference is:

- **TCP focuses on reliability**
- **UDP focuses on speed**

---

# TCP (Transmission Control Protocol)

## Overview

TCP is a connection-based protocol designed to provide reliable communication between two devices.

Before data is transmitted, TCP establishes a connection between the sender and receiver.

This ensures that data is:

- Delivered successfully
- Received in the correct order
- Checked for errors

---

# How TCP Works

TCP uses a process called a:

```
Three-Way Handshake
```

The handshake establishes a connection between two devices.

The process:

```
Client              Server

 SYN  ------------>

      <------------ SYN ACK

 ACK  ------------>

Connection Established
```

After the connection is created, data can be transmitted.

---

# TCP Features

## Reliability

TCP confirms that data has successfully arrived.

If data is missing or corrupted, it can be retransmitted.

---

## Data Ordering

TCP ensures packets are reconstructed in the correct order.

Example:

Data sent:

```
Packet 1
Packet 2
Packet 3
```

The receiver receives:

```
Packet 1
Packet 2
Packet 3
```

---

## Error Checking

TCP checks whether data has been damaged during transmission.

---

## Flow Control

TCP manages the amount of data being sent to prevent overwhelming the receiving device.

---

# Advantages of TCP

- Reliable delivery
- Error checking
- Data arrives in the correct order
- Prevents packet loss

---

# Disadvantages of TCP

- Slower than UDP
- Requires more processing
- Requires an established connection
- More overhead due to additional checks

---

# TCP Uses

TCP is commonly used when accuracy is more important than speed.

Examples:

| Protocol | Usage |
|-|-|
|HTTPS|Secure web browsing|
|HTTP|Web communication|
|SMTP|Email sending|
|FTP|File transfers|
|SSH|Remote administration|

---

# UDP (User Datagram Protocol)

## Overview

UDP is a connectionless protocol designed for speed and efficiency.

Unlike TCP, UDP does not establish a connection before sending data.

It sends packets without checking whether they arrive successfully.

---

# How UDP Works

UDP simply sends data to the destination.

Example:

```
Sender
 |
 |
 v

Packet Sent

 |
 |
 v

Receiver
```

There is no handshake or confirmation process.

---

# UDP Features

## No Connection Required

UDP does not create a session between devices.

This reduces delay.

---

## No Guaranteed Delivery

UDP does not confirm whether packets arrive.

If packets are lost, they are not automatically resent.

---

## Faster Communication

Because UDP performs fewer checks, it can transmit data faster than TCP.

---

# Advantages of UDP

- Faster than TCP
- Lower overhead
- Good for real-time communication
- Does not require a constant connection

---

# Disadvantages of UDP

- No guarantee data arrives
- No packet ordering
- No error correction
- Packet loss can affect performance

---

# UDP Uses

UDP is commonly used where speed is more important than perfect accuracy.

Examples:

| Protocol/Application | Usage |
|-|-|
|DNS|Domain name lookups|
|Online gaming|Fast real-time communication|
|Video streaming|Low latency media|
|VoIP|Voice communication|

---

# TCP vs UDP Comparison

| Feature | TCP | UDP |
|-|-|-|
|Connection | Connection-based | Connectionless |
|Speed | Slower | Faster |
|Reliability | Reliable | No guarantee |
|Error checking | Yes | Minimal |
|Ordering | Yes | No |
|Overhead | Higher | Lower |
|Use case | Accuracy required | Speed required |

---

# Real-World Example

## Downloading a File

TCP is used because every part of the file must arrive correctly.

Example:

Downloading an operating system update.

Missing data could corrupt the file.

---

## Video Call

UDP is often preferred because speed matters more than perfect delivery.

A small amount of lost data is better than delays.

---

# Cybersecurity Relevance

Understanding TCP and UDP is essential for cybersecurity because security professionals analyse network traffic based on:

- Protocol type
- Ports
- Connections
- Packet behaviour

---

# Ports

TCP and UDP use port numbers to identify services.

Examples:

| Port | Protocol | Service |
|-|-|-|
|22|TCP|SSH|
|80|TCP|HTTP|
|443|TCP|HTTPS|
|53|UDP/TCP|DNS|

---

# Security Considerations

## TCP

Security professionals may analyse:

- Suspicious TCP connections
- Open ports
- Unusual network sessions

Example:

An unexpected SSH connection could indicate unauthorised access.

---

## UDP

Security professionals may analyse:

- Large amounts of UDP traffic
- Unusual DNS activity
- Possible scanning activity

---

# Key Takeaways

- TCP and UDP operate at Layer 4 of the OSI model.
- TCP prioritises reliability.
- UDP prioritises speed.
- TCP uses handshakes and confirms delivery.
- UDP sends data without confirmation.
- The correct protocol depends on the purpose of the communication.
- Understanding TCP and UDP is essential for network analysis and cybersecurity.