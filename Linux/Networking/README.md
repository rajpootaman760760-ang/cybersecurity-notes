# Networking Notes

## IP Address
Unique address assigned to a device.

## MAC Address
Physical hardware address of a network interface.

## DNS
Converts domain names into IP addresses.

## DHCP
Automatically assigns IP addresses.

## TYPES OF NETWORK
-PAN (Personal Area Network) 
 
-CAN (Campus Area Network)
 
-LAN (Local Area Network)
 
-MAN (Metropolitan Area Network)

-WAN (Wide Area Network)


# Data Transfer Terms

## Introduction

Whenever data travels across a network, different terms are used to describe **how fast**, **how efficiently**, and **how reliably** the data is transmitted. These terms are fundamental in Networking and Cyber Security.

---

# 1. Bandwidth

Bandwidth is the **maximum amount of data** that can be transmitted over a network in one second.

It represents the **capacity** of the network, not the actual speed.

Example:
- 100 Mbps Ethernet
- 1 Gbps Fiber Link

Higher bandwidth means more data can travel at the same time.

---

# 2. Throughput

Throughput is the **actual amount of data** successfully transferred over the network.

Example:

Bandwidth = 100 Mbps

Actual Data Transfer = 82 Mbps

Throughput = 82 Mbps

Throughput is usually lower than bandwidth because of congestion and network overhead.

---

# 3. Latency

Latency is the **time taken for a packet to travel from source to destination.**

It is measured in milliseconds (ms).

Lower latency means faster communication.

Examples:
- Online Gaming
- Video Calls
- VoIP

---

# 4. Jitter

Jitter is the **variation in packet delay**.

If packets arrive at inconsistent intervals, jitter increases.

High jitter causes:
- Choppy Voice Calls
- Video Freezing
- Poor Streaming Quality

---

# 5. Packet Loss

Packet Loss occurs when packets fail to reach the destination.

Causes:
- Network Congestion
- Hardware Failure
- Bad Cable
- Wireless Interference

High packet loss reduces network performance.

---

# 6. Goodput

Goodput is the **actual useful data received by the application**.

Unlike throughput, goodput excludes:

- Retransmissions
- Protocol Headers
- Network Overhead

Goodput represents only the useful payload.

---

# Comparison

| Term | Meaning |
|-------|---------|
| Bandwidth | Maximum network capacity |
| Throughput | Actual data transferred |
| Goodput | Useful application data |
| Latency | Time taken to deliver a packet |
| Jitter | Variation in latency |
| Packet Loss | Packets lost during transmission |

---

# Key Takeaways

- Bandwidth is capacity.
- Throughput is actual performance.
- Goodput is useful data.
- Latency measures delay.
- Jitter measures delay variation.
- Packet loss indicates failed delivery.

# Network Topologies

## Introduction

A Network Topology defines how devices are physically or logically connected in a network.

Choosing the correct topology affects performance, reliability, scalability, and maintenance.

---

# 1. Bus Topology

All devices are connected to a single backbone cable.

Advantages:
- Simple
- Low Cost

Disadvantages:
- Backbone failure stops the entire network.
- Difficult troubleshooting.

---

# 2. Star Topology

All devices connect to a central switch or hub.

Advantages:
- Easy management
- Easy troubleshooting
- High performance

Disadvantages:
- Switch failure affects the entire network.

Most modern LANs use Star Topology.

---

# 3. Ring Topology

Each device connects to exactly two neighboring devices, forming a circular path.

Advantages:
- Predictable performance

Disadvantages:
- A single cable failure can disrupt communication unless redundancy exists.

---

# 4. Mesh Topology

Each device is connected to multiple devices.

Types:
- Full Mesh
- Partial Mesh

Advantages:
- High Availability
- Excellent Fault Tolerance

Disadvantages:
- Expensive
- Complex Cabling

Used in:
- ISP Networks
- WAN Infrastructure

---

# 5. Tree Topology

A hierarchical combination of multiple Star Networks.

Advantages:
- Highly Scalable
- Easy Expansion

Disadvantages:
- Backbone failure affects multiple branches.

---

# 6. Hybrid Topology

A combination of two or more topologies.

Example:
- Star + Mesh
- Star + Bus

Used in:
- Enterprise Networks
- Data Centers

---

# Physical vs Logical Topology

Physical Topology:
Describes how devices are physically connected.

Logical Topology:
Describes how data flows inside the network.

---

# Comparison

| Topology | Cost | Reliability | Scalability |
|-----------|------|------------|-------------|
| Bus | Low | Low | Low |
| Star | Medium | High | High |
| Ring | Medium | Medium | Medium |
| Mesh | High | Very High | Medium |
| Tree | Medium | High | High |
| Hybrid | High | Very High | Very High |

---

# Key Takeaways

- Star Topology is the most commonly used LAN topology.
- Mesh provides maximum redundancy.
- Tree is suitable for large organizations.
- Hybrid combines multiple topologies for flexibility.
- Physical topology differs from logical topology.

# Client-Server and Peer-to-Peer (P2P) Architecture

## Introduction

A network architecture defines how devices communicate and share resources within a network.

The two most common network architectures are:

- Client-Server Architecture
- Peer-to-Peer (P2P) Architecture

Understanding these models is important because almost every modern network is built using one of them.

---

# 1. Client-Server Architecture

In a Client-Server network, one device acts as the **Server**, while other devices act as **Clients**.

The client requests services or resources, and the server processes the request and sends the response.

Example:

```
Client --------\
Client ---------> Server
Client --------/
```

Examples:

- Web Browsing
- Email Services
- Cloud Storage
- Online Banking

---

## Characteristics

- Centralized management
- Better security
- Easy backup
- Easy maintenance
- Suitable for medium and large organizations

---

## Advantages

- Centralized data storage
- Strong security
- Easy administration
- Better performance
- Scalable

---

## Disadvantages

- Server failure can affect all clients.
- Higher implementation cost.
- Requires dedicated server hardware.

---

# 2. Peer-to-Peer (P2P) Architecture

In a Peer-to-Peer network, every computer can act as both a client and a server.

There is no dedicated central server.

Example:

```
PC A ------ PC B
 |            |
 |            |
PC C ------ PC D
```

Each computer shares its own resources directly.

---

## Characteristics

- No dedicated server
- Equal privileges for all devices
- Direct communication
- Easy setup

---

## Advantages

- Low cost
- Simple configuration
- No dedicated server required
- Suitable for small networks

---

## Disadvantages

- Weak security
- Difficult management
- Poor scalability
- No centralized backup

---

# Client-Server vs Peer-to-Peer

| Feature | Client-Server | Peer-to-Peer |
|----------|--------------|--------------|
| Server | Dedicated | No Dedicated Server |
| Management | Centralized | Decentralized |
| Security | High | Low |
| Cost | High | Low |
| Scalability | Excellent | Limited |
| Performance | Better | Depends on Peers |
| Backup | Centralized | Individual |

---

# Real-World Examples

### Client-Server

- Google Search
- Gmail
- Facebook
- Netflix
- Online Banking

### Peer-to-Peer

- BitTorrent
- Local File Sharing
- Small Home Networks

---

# Cyber Security Perspective

### Client-Server

Advantages:
- Centralized authentication
- Better access control
- Easier monitoring
- Security policies can be applied from one place

### Peer-to-Peer

Challenges:
- Harder to monitor
- Difficult to enforce security policies
- Greater risk of malware spreading between peers

---

# Key Takeaways

- Client-Server uses a dedicated server to provide services.
- Peer-to-Peer allows devices to communicate directly.
- Client-Server offers better security and scalability.
- P2P is cheaper but harder to manage.
- Most enterprise networks use the Client-Server model.

- # 🫠OSI Model (Open Systems Interconnection Model)

## Introduction

The **OSI (Open Systems Interconnection) Model** is a **conceptual reference model** that explains how data travels from one device to another over a network.

It divides the entire communication process into **7 layers**, where each layer performs a specific task. This layered approach makes networking easier to understand, design, and troubleshoot.

> **Note:** The OSI Model is **not a protocol**. It is a reference model used to understand how network communication works.

---

# Why Do We Need the OSI Model?

Imagine a user says:

> "The internet is not working."

The problem could be related to:
- A damaged network cable
- An incorrect IP address
- A switch failure
- A router issue
- A DNS problem
- An application error

Without a standard model, finding the exact issue would be difficult.

The OSI Model helps engineers troubleshoot problems layer by layer.

---

# The 7 Layers of the OSI Model

| Layer | Name | Main Function |
|-------|----------------|-------------------------------|
| 7 | Application | Provides network services to applications |
| 6 | Presentation | Data formatting, encryption, compression |
| 5 | Session | Establishes, manages, and terminates sessions |
| 4 | Transport | Reliable data delivery and error recovery |
| 3 | Network | Logical addressing and routing |
| 2 | Data Link | Physical addressing (MAC) and frame delivery |
| 1 | Physical | Transmits raw bits over the physical medium |

---

# Data Flow in the OSI Model

## Sender Side (Encapsulation)

```
Application
      ↓
Presentation
      ↓
Session
      ↓
Transport
      ↓
Network
      ↓
Data Link
      ↓
Physical
```

The sender adds protocol information at each layer before transmitting the data.

This process is called **Encapsulation**.

---

## Receiver Side (Decapsulation)

```
Physical
     ↑
Data Link
     ↑
Network
     ↑
Transport
     ↑
Session
     ↑
Presentation
     ↑
Application
```

Each layer removes its corresponding header and passes the data to the next layer.

This process is called **Decapsulation**.

---

# Layer 7 – Application Layer

The Application Layer is the closest layer to the user.

It provides network services that applications use to communicate over the network.

### Examples

- Web Browser
- Email Client
- WhatsApp
- FTP Client

### Common Protocols

- HTTP
- HTTPS
- FTP
- SMTP
- DNS

---

# Layer 6 – Presentation Layer

The Presentation Layer is responsible for preparing data before it reaches the application.

### Functions

- Data Formatting
- Encryption
- Decryption
- Compression
- Decompression

---

# Layer 5 – Session Layer

The Session Layer establishes, manages, and terminates communication sessions between devices.

### Functions

- Session Establishment
- Session Maintenance
- Session Termination
- Synchronization

---

# Layer 4 – Transport Layer

The Transport Layer provides end-to-end communication between devices.

### Functions

- Segmentation
- Error Detection
- Reliable Data Delivery
- Flow Control

### Common Protocols

- TCP
- UDP

---

# Layer 3 – Network Layer

The Network Layer determines the best path for packets to travel between networks.

### Functions

- Logical Addressing
- Routing
- Packet Forwarding

### Device

- Router

### Common Protocol

- IP (IPv4 / IPv6)

---

# Layer 2 – Data Link Layer

The Data Link Layer is responsible for communication within the same local network.

### Functions

- MAC Addressing
- Framing
- Error Detection
- Switching

### Device

- Switch

---

# Layer 1 – Physical Layer

The Physical Layer transmits raw binary data over the physical medium.

### Functions

- Signal Transmission
- Electrical Signals
- Optical Signals
- Radio Signals

### Examples

- Ethernet Cable
- Fiber Optic Cable
- Wi-Fi Signals
- Network Connectors

---

# Memory Trick

From Layer 7 to Layer 1:

**All People Seem To Need Data Processing**

---

# Key Takeaways

- The OSI Model is a conceptual reference model.
- It consists of **7 layers**.
- Each layer has a specific responsibility.
- Data moves from Layer 7 to Layer 1 during transmission (**Encapsulation**).
- Data moves from Layer 1 to Layer 7 at the receiving side (**Decapsulation**).
- The OSI Model simplifies networking and troubleshooting.

---

# Summary

The OSI Model provides a standardized framework for understanding network communication. By dividing communication into seven independent layers, it becomes easier to design networks, troubleshoot problems, and understand how protocols and networking devices interact.

# Encapsulation and Decapsulation

## Introduction

When data is transmitted from one device to another, it passes through different layers of the OSI Model.

During transmission, each layer adds its own information to the data. This process is called **Encapsulation**.

At the receiving device, each layer removes its own information. This process is called **Decapsulation**.

---

# What is Encapsulation?

**Encapsulation** is the process of adding protocol information (headers and sometimes trailers) to data as it moves from the **Application Layer** to the **Physical Layer**.

Each layer adds its own header to help the receiving device understand and process the data correctly.

---

# Encapsulation Process

```
Application Layer
        │
        ▼
      Data
        │
        ▼
Presentation Layer
        │
        ▼
Session Layer
        │
        ▼
Transport Layer
+----------------------+
| TCP/UDP Header |
+----------------------+
        │
        ▼
Network Layer
+----------------------+
| IP Header |
+----------------------+
        │
        ▼
Data Link Layer
+----------------------+
| MAC Header |
|      Data            |
| MAC Trailer |
+----------------------+
        │
        ▼
Physical Layer
        │
        ▼
Binary Bits (0s and 1s)
```

---

# Protocol Data Units (PDU)

As data moves through different layers, its name changes.

| Layer | PDU Name |
|--------|----------|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment (TCP) / Datagram (UDP) |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---

# Encapsulation Example

Suppose you send a message:

```
Hello
```

### Step 1

Application Layer creates the data.

```
Data
```

---

### Step 2

Transport Layer adds a TCP header.

```
TCP Header + Data
```

---

### Step 3

Network Layer adds an IP header.

```
IP Header + TCP Header + Data
```

---

### Step 4

Data Link Layer adds a MAC header and trailer.

```
MAC Header + IP Header + TCP Header + Data + Trailer
```

---

### Step 5

Physical Layer converts everything into binary bits.

```
010101010101...
```

These bits are transmitted over the network.

---

# What is Decapsulation?

**Decapsulation** is the reverse process of Encapsulation.

The receiving device removes headers layer by layer until the original data reaches the application.

---

# Decapsulation Process

```
Bits
   │
   ▼
Physical Layer
   │
   ▼
Frame
(Remove MAC Header/Trailer)
   │
   ▼
Packet
(Remove IP Header)
   │
   ▼
Segment
(Remove TCP/UDP Header)
   │
   ▼
Data
   │
   ▼
Application
```

---

# Example

Sender sends:

```
Hello
```

During transmission:

```
MAC Header
IP Header
TCP Header
Hello
Trailer
```

Receiver removes them one by one:

```
Remove MAC Header
↓
Remove IP Header
↓
Remove TCP Header
↓
Original Message:
Hello
```

---

# Why is Encapsulation Important?

- Enables communication between different devices.
- Provides logical and physical addressing.
- Supports routing and switching.
- Ensures reliable data delivery.
- Makes troubleshooting easier.

---

# Why is Decapsulation Important?

- Removes unnecessary protocol information.
- Restores the original data.
- Delivers the data to the correct application.

---

# Key Takeaways

- Encapsulation occurs on the sender side.
- Decapsulation occurs on the receiver side.
- Every layer adds or removes protocol information.
- The data changes from **Data → Segment → Packet → Frame → Bits** during transmission.
- The reverse process occurs at the receiving device.

---

# Summary

Encapsulation is the process of adding protocol headers as data travels down the OSI layers, while Decapsulation is the process of removing those headers at the receiving device to recover the original data. These two processes form the foundation of network communication.

# TCP/IP Model

## Introduction

The **TCP/IP (Transmission Control Protocol / Internet Protocol) Model** is the standard networking model used on the Internet.

Unlike the OSI Model, which is a conceptual reference model, the TCP/IP Model is a practical model that defines how devices communicate over real networks.

Almost every modern network, including the Internet, uses the TCP/IP Model.

---

# Why Do We Need the TCP/IP Model?

When data is transmitted across a network, different tasks need to be performed, such as:

- Creating data
- Establishing communication
- Routing packets
- Delivering data over the physical network

The TCP/IP Model divides these responsibilities into **4 layers**, making communication efficient and standardized.

---

# Layers of the TCP/IP Model

| Layer | Function |
|---------|----------------------------------------|
| Application | Provides network services to applications |
| Transport | End-to-end communication |
| Internet | Logical addressing and routing |
| Network Access | Physical transmission and local communication |

---

# TCP/IP Communication Process

```
Application Layer
        │
        ▼
Transport Layer
        │
        ▼
Internet Layer
        │
        ▼
Network Access Layer
        │
        ▼
Physical Network
```

---

# 1. Application Layer

The Application Layer is the top layer of the TCP/IP Model.

It provides services that allow applications to communicate over the network.

### Functions

- Web browsing
- Email
- File transfer
- Domain name resolution

### Common Protocols

- HTTP
- HTTPS
- FTP
- SMTP
- POP3
- IMAP
- DNS
- DHCP

---

# 2. Transport Layer

The Transport Layer provides end-to-end communication between devices.

It ensures that data reaches the correct application.

### Functions

- Segmentation
- Error detection
- Flow control
- Reliable communication
- Port numbers

### Protocols

## TCP (Transmission Control Protocol)

Features:

- Connection-oriented
- Reliable
- Error checking
- Ordered delivery
- Retransmission

Used for:

- Web browsing
- Email
- File transfer

---

## UDP (User Datagram Protocol)

Features:

- Connectionless
- Faster
- No guarantee of delivery
- Lower overhead

Used for:

- Video streaming
- Online gaming
- VoIP
- DNS

---

# 3. Internet Layer

The Internet Layer is responsible for moving packets between different networks.

### Functions

- Logical addressing
- Routing
- Packet forwarding

### Protocols

- IPv4
- IPv6
- ICMP
- ARP

---

# 4. Network Access Layer

The Network Access Layer is responsible for transmitting data over the physical network.

### Functions

- MAC Addressing
- Framing
- Physical transmission
- Error detection

### Technologies

- Ethernet
- Wi-Fi
- Fiber Optic

---

# Data Encapsulation

As data moves down the TCP/IP Model:

```
Data
   ↓
Segment
   ↓
Packet
   ↓
Frame
   ↓
Bits
```

At the receiving side, the reverse process takes place.

---

# TCP/IP vs OSI Model

| OSI Model | TCP/IP Model |
|------------|--------------|
| 7 Layers | 4 Layers |
| Reference Model | Practical Model |
| Mostly Educational | Used in Real Networks |
| More Detailed | Simpler |

---

# Layer Mapping

| OSI Layer | TCP/IP Layer |
|------------|--------------|
| Application | Application |
| Presentation | Application |
| Session | Application |
| Transport | Transport |
| Network | Internet |
| Data Link | Network Access |
| Physical | Network Access |

---

# Advantages

- Simple architecture
- Highly scalable
- Widely supported
- Used by the Internet
- Supports different hardware and operating systems

---

# Key Takeaways

- TCP/IP is the networking model used by the Internet.
- It contains 4 layers.
- TCP provides reliable communication.
- UDP provides faster communication with less overhead.
- IP is responsible for logical addressing and routing.
- The Network Access Layer handles physical communication.

---

# Summary

The TCP/IP Model is the foundation of modern networking. It defines how data is transmitted between devices using four layers. Every Internet service, from web browsing to email and cloud computing, relies on the TCP/IP Model for communication.

# Ethernet Frame & MAC Address

## Introduction

Ethernet is the most widely used technology for communication in Local Area Networks (LANs). It defines how devices send and receive data within the same network.

Before data is transmitted over an Ethernet network, it is packed into a structure called an **Ethernet Frame**.

Every device on an Ethernet network is identified using a unique **MAC Address**.

---

# What is Ethernet?

Ethernet is a Layer 2 (Data Link Layer) technology that enables communication between devices connected to the same local network.

Examples:

- Home Wi-Fi Router
- Office LAN
- College Computer Lab
- Data Center Network

---

# What is an Ethernet Frame?

An Ethernet Frame is the format used to transmit data over an Ethernet network.

Think of it like a courier package.

- The package contains your actual item (Data).
- The label contains sender and receiver information.
- Similarly, an Ethernet Frame contains data along with addressing information.

---

# Structure of an Ethernet Frame

```
+---------------------------------------------------------------+
| Destination MAC | Source MAC | Type | Data | FCS |
+---------------------------------------------------------------+
```

Each field has a specific purpose.

---

# 1. Destination MAC Address

This field contains the MAC Address of the receiving device.

Example:

```
00:1A:2B:3C:4D:5E
```

The switch reads this address to decide where to forward the frame.

---

# 2. Source MAC Address

This field contains the MAC Address of the sending device.

Example:

```
F8:9E:94:AA:11:22
```

It identifies who sent the frame.

---

# 3. EtherType

This field tells the receiving device which Layer 3 protocol is carried inside the frame.

Common EtherType values:

| EtherType | Protocol |
|-----------|----------|
| 0x0800 | IPv4 |
| 0x86DD | IPv6 |
| 0x0806 | ARP |

---

# 4. Data (Payload)

This is the actual information being transmitted.

It may contain:

- IP Packet
- ARP Packet
- Other Layer 3 Data

---

# 5. Frame Check Sequence (FCS)

The FCS is used for **error detection**.

Before sending a frame, the sender calculates a checksum.

The receiver performs the same calculation.

If both values match:

```
Frame Accepted
```

Otherwise:

```
Frame Discarded
```

---

# What is a MAC Address?

A MAC (Media Access Control) Address is a unique physical address assigned to every Network Interface Card (NIC).

It is used for communication within the same Local Area Network.

---

# MAC Address Format

Example:

```
00:1A:2B:3C:4D:5E
```

A MAC Address consists of:

- 48 bits
- 6 bytes
- Written in hexadecimal

---

# MAC Address Structure

```
00:1A:2B : 3C:4D:5E
│
│
Manufacturer ID (OUI)

Remaining Part
Unique Device Identifier
```

The first 24 bits identify the manufacturer.

The last 24 bits uniquely identify the device.

---

# Types of MAC Addresses

## Unicast

One sender → One receiver

Example:

```
PC A → PC B
```

---

## Broadcast

One sender → All devices in the LAN

Broadcast MAC:

```
FF:FF:FF:FF:FF:FF
```

---

## Multicast

One sender → A selected group of devices.

---

# MAC Address vs IP Address

| MAC Address | IP Address |
|-------------|------------|
| Physical Address | Logical Address |
| Layer 2 | Layer 3 |
| Permanent (Usually) | Can Change |
| Used Inside LAN | Used Across Networks |

---

# How a Switch Uses MAC Addresses

Suppose PC A wants to send data to PC B.

```
PC A
   │
   ▼
Switch
   │
   ▼
PC B
```

The switch reads the **Destination MAC Address**.

It checks its **MAC Address Table**.

If the MAC exists:

```
Forward Frame
```

If not:

```
Flood Frame
```

After learning the MAC Address, future communication becomes faster.

---

# Why MAC Addresses are Important?

- Identify devices in a LAN.
- Enable frame delivery.
- Used by switches for forwarding.
- Support reliable local communication.

---

# Key Takeaways

- Ethernet is the most common LAN technology.
- Data is transmitted using Ethernet Frames.
- Every Ethernet Frame contains Source MAC and Destination MAC addresses.
- MAC Address is a unique physical address of a network device.
- Switches forward frames based on MAC Addresses.
- FCS is used for error detection.

---

# Summary

Ethernet enables communication within Local Area Networks by transmitting data in the form of Ethernet Frames. Every frame contains source and destination MAC addresses, allowing switches to deliver data to the correct device efficiently.
