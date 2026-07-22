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

# Switching Logic (How a Network Switch Works)

## Introduction

A network switch is a Layer 2 (Data Link Layer) device that connects multiple devices within a Local Area Network (LAN).

Unlike a hub, a switch does not send data to every connected device. Instead, it intelligently forwards data only to the intended destination using MAC Addresses.

This process is known as **Switching Logic**.

---

# Why Do We Need a Switch?

Imagine four computers connected in a network.

```
       +-----------+
PC1 ---|           |
PC2 ---|  Switch   |
PC3 ---|           |
PC4 ---|           |
       +-----------+
```

If PC1 wants to send data to PC3, only PC3 should receive the frame.

The switch makes this possible.

---

# MAC Address Table (CAM Table)

Every switch maintains a table called the **MAC Address Table** (also known as the CAM Table).

It stores:

- MAC Address
- Switch Port

Example:

| MAC Address | Port |
|-------------|------|
| AA:AA:AA:AA:AA:AA | Fa0/1 |
| BB:BB:BB:BB:BB:BB | Fa0/2 |
| CC:CC:CC:CC:CC:CC | Fa0/3 |

The switch uses this table to decide where to send frames.

---

# Step 1 – Learning

When a frame enters the switch, it first checks the **Source MAC Address**.

Example:

```
PC1
MAC = AA:AA:AA:AA:AA:AA
```

The switch learns:

```
AA:AA:AA:AA:AA:AA → Port 1
```

This process is called **MAC Learning**.

---

# Step 2 – Lookup

Now the switch checks the **Destination MAC Address**.

Suppose the destination is:

```
CC:CC:CC:CC:CC:CC
```

The switch searches for this MAC Address in its MAC Address Table.

---

# Case 1 – MAC Address Found

If the destination MAC exists:

```
MAC Found
      ↓
Forward Frame
      ↓
Correct Port
```

Only the destination device receives the frame.

This is called **Unicast Forwarding**.

---

# Case 2 – MAC Address Not Found

If the destination MAC is not in the table:

```
Unknown MAC
      ↓
Flood Frame
```

The switch sends the frame to all ports except the incoming port.

When the destination replies, the switch learns its MAC Address and updates the table.

---

# MAC Learning Example

Initially:

```
MAC Table = Empty
```

PC1 sends data.

```
PC1 → Switch
```

The switch learns:

```
AA:AA:AA:AA:AA:AA → Port 1
```

Later PC2 sends data.

```
BB:BB:BB:BB:BB:BB → Port 2
```

Now the table becomes:

| MAC Address | Port |
|-------------|------|
| AA:AA:AA:AA:AA:AA | Port 1 |
| BB:BB:BB:BB:BB:BB | Port 2 |

As more devices communicate, the switch keeps learning.

---

# MAC Aging

Devices may disconnect or change ports.

To keep the table accurate, switches remove old entries after a certain period.

This process is called **MAC Aging**.

---

# Switching Decisions

A switch follows these simple steps:

1. Receive the Ethernet Frame.
2. Learn the Source MAC Address.
3. Check the Destination MAC Address.
4. Search the MAC Address Table.
5. If found, forward the frame to the correct port.
6. If not found, flood the frame.
7. Learn new MAC Addresses from future communication.

---

# Advantages of Switching

- Faster communication
- Reduced unnecessary traffic
- Better bandwidth utilization
- Improved network performance
- Supports full-duplex communication

---

# Hub vs Switch

| Hub | Switch |
|------|---------|
| Layer 1 Device | Layer 2 Device |
| No MAC Table | Uses MAC Table |
| Sends data to all ports | Sends data to the correct port |
| More collisions | Fewer collisions |
| Lower performance | Better performance |

---

# Key Takeaways

- A switch works at the Data Link Layer (Layer 2).
- It forwards frames using MAC Addresses.
- It learns MAC Addresses automatically.
- It stores MAC Addresses in a MAC Address Table (CAM Table).
- Unknown MAC Addresses are flooded.
- Known MAC Addresses are forwarded only to the correct port.

---

# Summary

A network switch intelligently forwards Ethernet frames by learning and storing MAC Addresses in a MAC Address Table. This makes communication faster, reduces unnecessary traffic, and improves the overall efficiency of a Local Area Network.

# Spanning Tree Protocol (STP)

## Introduction

In a switched network, connecting multiple switches using redundant links improves reliability. If one link fails, another link can continue carrying traffic.

However, redundant links can also create **network loops**.

To prevent these loops, Ethernet networks use the **Spanning Tree Protocol (STP)**.

STP automatically detects loops and blocks unnecessary paths while keeping them available as backup links.

---

# Why Do We Need STP?

Consider three switches connected together.

```
        Switch A
       /        \
      /          \
Switch B ------- Switch C
```

This design provides redundancy because there are multiple paths between the switches.

But if all links remain active, Ethernet frames may circulate forever, creating a switching loop.

---

# Problems Caused by Network Loops

A switching loop can create several serious issues.

### 1. Broadcast Storm

A broadcast frame keeps circulating between switches.

```
Switch A
   ↓
Switch B
   ↓
Switch C
   ↓
Switch A
```

The same frame is forwarded repeatedly.

As more frames are generated, network bandwidth becomes fully occupied.

---

### 2. MAC Address Table Instability

A switch continuously learns the same MAC Address from different ports.

Example:

```
AA:AA:AA → Port 1

After a few milliseconds

AA:AA:AA → Port 2
```

The MAC Address Table keeps changing, making forwarding unreliable.

---

### 3. Duplicate Frames

The destination device may receive the same frame multiple times.

This can lead to incorrect application behavior and unnecessary traffic.

---

# What is STP?

**Spanning Tree Protocol (STP)** is a Layer 2 protocol defined by **IEEE 802.1D**.

Its purpose is to remove switching loops without removing physical redundancy.

Instead of deleting links, STP places unnecessary links into a **Blocking State**.

If the active link fails, the blocked link automatically becomes active.

---

# How STP Works

STP follows three major steps.

---

## Step 1 – Root Bridge Election

All switches exchange **Bridge Protocol Data Units (BPDUs)**.

The switch with the **lowest Bridge ID (BID)** becomes the **Root Bridge**.

```
Switch A
Bridge ID = Lowest

↓

Root Bridge
```

Every network has only **one Root Bridge**.

---

## Step 2 – Path Selection

Each switch calculates the shortest path to the Root Bridge.

The path with the **lowest cost** becomes the preferred path.

---

## Step 3 – Port Roles

STP assigns different roles to switch ports.

### Root Port (RP)

- One Root Port on every non-root switch.
- Provides the shortest path to the Root Bridge.

---

### Designated Port (DP)

- One Designated Port on every network segment.
- Forwards traffic toward that segment.

---

### Blocking Port

Ports that could create loops are placed into the Blocking State.

These ports do not forward normal data traffic.

---

# Port States (Classic STP)

A switch port passes through several states.

| State | Purpose |
|--------|---------|
| Blocking | Prevents loops and does not forward frames |
| Listening | Learns network topology |
| Learning | Learns MAC Addresses but does not forward data |
| Forwarding | Normal traffic forwarding |
| Disabled | Port is administratively down |

---

# BPDU (Bridge Protocol Data Unit)

Switches exchange special messages called **BPDUs**.

BPDUs help switches:

- Elect the Root Bridge
- Detect loops
- Exchange topology information
- Recalculate paths after failures

---

# Link Failure Example

Initial Topology

```
Switch A
 /      \
B        C
 \      /
```

One link is blocked by STP.

If the active link fails:

```
Link Failure
      ↓
STP Recalculates
      ↓
Blocked Link Becomes Active
```

The network continues to operate without manual intervention.

---

# Advantages of STP

- Prevents Layer 2 loops
- Eliminates broadcast storms
- Prevents duplicate frames
- Stabilizes MAC Address Tables
- Supports redundant network design
- Improves network reliability

---

# STP vs No STP

| Without STP | With STP |
|--------------|----------|
| Network Loops | Loop-Free Network |
| Broadcast Storms | Controlled Traffic |
| Duplicate Frames | No Duplicate Frames |
| MAC Table Instability | Stable MAC Table |
| Network Failure | Reliable Redundancy |

---

# Key Takeaways

- STP works at Layer 2.
- It prevents switching loops.
- It elects one Root Bridge.
- Redundant links are blocked instead of removed.
- If an active link fails, a blocked link automatically becomes active.
- Switches exchange BPDUs to build and maintain the spanning tree.

---

# Summary

Spanning Tree Protocol (STP) is a Layer 2 protocol that prevents switching loops in Ethernet networks. It creates a loop-free topology by electing a Root Bridge, selecting the best paths, and blocking redundant links while keeping them available as backup paths.

# VLANs & IEEE 802.1Q Tagging

## Introduction

A **VLAN (Virtual Local Area Network)** is a logical division of a physical network.

Instead of connecting devices using separate switches, VLANs allow multiple logical networks to exist on the same physical switch.

This improves security, performance, and network management.

---

# Why Do We Need VLANs?

Imagine a company with three departments:

- HR
- Finance
- IT

Without VLANs:

```
        Switch

PC1 (HR)
PC2 (Finance)
PC3 (IT)
PC4 (HR)
PC5 (IT)
```

All devices belong to the same network.

Problems:

- Everyone receives broadcast traffic.
- Lower security.
- Higher network congestion.
- Difficult management.

---

# Solution: VLAN

Using VLANs, the same switch can be divided into multiple logical networks.

```
            Switch

VLAN 10 → HR

PC1
PC4

------------------

VLAN 20 → Finance

PC2

------------------

VLAN 30 → IT

PC3
PC5
```

Now each department works like a separate network.

---

# What is a VLAN?

A VLAN groups devices logically instead of physically.

Devices in the same VLAN can communicate directly.

Devices in different VLANs cannot communicate unless routing is configured.

---

# Benefits of VLANs

- Better Security
- Reduced Broadcast Traffic
- Easier Network Management
- Improved Performance
- Logical Network Separation
- Easy Department Management

---

# VLAN ID

Each VLAN has a unique number.

Examples:

| VLAN ID | Department |
|----------|------------|
| 10 | HR |
| 20 | Finance |
| 30 | IT |
| 100 | Guest |

Valid VLAN IDs:

```
1 – 4094
```

---

# Broadcast Domain

Each VLAN creates a separate **Broadcast Domain**.

Example:

```
VLAN 10

PC1 ---- PC2 ---- PC3

Broadcast stays only inside VLAN 10.
```

Broadcast traffic does not enter VLAN 20 or VLAN 30.

---

# Communication Between VLANs

Suppose:

```
PC1 → VLAN 10

PC2 → VLAN 20
```

They **cannot communicate directly**.

To communicate between VLANs, a **Router** or a **Layer 3 Switch** is required.

This process is called:

**Inter-VLAN Routing**

---

# Access Port

An **Access Port** carries traffic for **only one VLAN**.

Example:

```
PC
 │
 │
Access Port
 │
Switch
```

Used for:

- PCs
- Printers
- IP Phones
- Servers

---

# Trunk Port

A **Trunk Port** carries traffic for **multiple VLANs** simultaneously.

Usually used between:

- Switch ↔ Switch
- Switch ↔ Router
- Switch ↔ Layer 3 Switch

Example:

```
Switch A
    │
Trunk Port
    │
Switch B
```

---

# Why Do We Need Trunk Ports?

Suppose Switch A and Switch B both contain:

- VLAN 10
- VLAN 20
- VLAN 30

Instead of using three separate cables, one trunk cable can carry traffic for all VLANs.

---

# IEEE 802.1Q Tagging

When multiple VLANs share the same trunk link, the receiving switch must know which VLAN each frame belongs to.

IEEE **802.1Q** solves this problem.

It inserts a small VLAN Tag into the Ethernet Frame.

---

# VLAN Tag

Normal Ethernet Frame

```
Destination MAC
Source MAC
Type
Data
FCS
```

Tagged Ethernet Frame

```
Destination MAC
Source MAC

VLAN Tag (802.1Q)

Type
Data
FCS
```

The VLAN Tag contains the VLAN ID.

---

# Native VLAN

On a trunk port, one VLAN is called the **Native VLAN**.

Frames belonging to the Native VLAN are usually sent **without an 802.1Q tag**.

By default:

```
Native VLAN = VLAN 1
```

(Administrators often change this for security reasons.)

---

# Access Port vs Trunk Port

| Access Port | Trunk Port |
|--------------|------------|
| One VLAN | Multiple VLANs |
| Connected to End Devices | Connected to Network Devices |
| No VLAN Tag | Uses 802.1Q Tags |
| Simple Configuration | Advanced Configuration |

---

# VLAN Advantages

- Better Security
- Smaller Broadcast Domains
- Higher Performance
- Easier Administration
- Flexible Network Design
- Efficient Resource Utilization

---

# Key Takeaways

- VLAN divides one physical network into multiple logical networks.
- Each VLAN is a separate Broadcast Domain.
- Devices in different VLANs cannot communicate directly.
- Access Ports carry one VLAN.
- Trunk Ports carry multiple VLANs.
- IEEE 802.1Q adds VLAN Tags to Ethernet Frames.
- Inter-VLAN communication requires a Router or Layer 3 Switch.

---

# Summary

A VLAN allows multiple logical networks to exist on a single physical switch, improving security and reducing unnecessary broadcast traffic. IEEE 802.1Q tagging enables multiple VLANs to travel across a single trunk link by adding VLAN identification information to Ethernet Frames.

# Collision Domain & Broadcast Domain

## Introduction

In computer networks, data is transmitted between devices using Ethernet.

When multiple devices communicate at the same time, network traffic must be managed properly to avoid communication problems.

Two important concepts used to understand network traffic are:

- Collision Domain
- Broadcast Domain

Understanding these concepts helps in designing efficient and scalable networks.

---

# What is a Collision Domain?

A **Collision Domain** is a part of the network where two or more devices can attempt to send data at the same time, causing a **collision**.

A collision happens when multiple devices transmit data simultaneously on the same communication channel.

Example:

```
PC1
   \
    \
     Hub
    / | \
PC2  |  PC3
```

If PC1 and PC2 send data at the same time, the signals collide.

This results in:

- Data corruption
- Retransmission
- Reduced network performance

---

# Why Do Collisions Occur?

Collisions mainly occur in **Half-Duplex Ethernet** where devices share the same communication medium.

Modern switched networks using **Full-Duplex** communication eliminate collisions.

---

# Hub and Collision Domain

A Hub does not understand MAC Addresses.

It simply copies incoming data to every connected port.

```
      Hub

PC1  PC2  PC3
```

All connected devices share **one Collision Domain**.

---

# Switch and Collision Domain

A Switch creates a separate Collision Domain for every port.

```
        Switch

PC1   PC2   PC3
```

Each device communicates independently.

Result:

- No collisions
- Better performance
- Higher bandwidth

---

# Collision Domain Comparison

| Device | Collision Domains |
|----------|------------------|
| Hub | One |
| Switch | One per Port |

---

# What is a Broadcast Domain?

A **Broadcast Domain** is the group of devices that receive a broadcast message.

A broadcast frame is sent to **every device** within the same broadcast domain.

Broadcast MAC Address:

```
FF:FF:FF:FF:FF:FF
```

---

# Example

```
       Switch

PC1
PC2
PC3
PC4
```

If PC1 sends a broadcast frame:

```
PC1
 │
 ▼
Switch
 │
 ├──► PC2
 ├──► PC3
 └──► PC4
```

Every device receives the broadcast.

---

# Router and Broadcast Domain

A Router does **not forward broadcast traffic** between different networks.

Example:

```
LAN 1
 PC1
 PC2
   │
 Router
   │
 PC3
 PC4
LAN 2
```

Broadcast from LAN 1 will **not** reach LAN 2.

Each side is a separate Broadcast Domain.

---

# VLAN and Broadcast Domain

Each VLAN creates its own Broadcast Domain.

Example:

```
Switch

VLAN 10
PC1
PC2

------------

VLAN 20
PC3
PC4
```

Broadcast generated in VLAN 10 stays only inside VLAN 10.

It does not reach VLAN 20.

---

# Collision Domain vs Broadcast Domain

| Collision Domain | Broadcast Domain |
|------------------|------------------|
| Data Collision Area | Broadcast Traffic Area |
| Controlled by Switch | Controlled by Router or VLAN |
| Affects Performance | Affects Network Size |
| One per Switch Port | One per Network/VLAN |

---

# Hub vs Switch vs Router

| Device | Collision Domain | Broadcast Domain |
|----------|------------------|------------------|
| Hub | One | One |
| Switch | One per Port | One |
| Router | One per Interface | One per Interface |

---

# Why Are These Concepts Important?

Understanding Collision and Broadcast Domains helps in:

- Improving network performance
- Reducing unnecessary traffic
- Better network segmentation
- Efficient troubleshooting
- Designing scalable enterprise networks

---

# Key Takeaways

- A Collision Domain is where data collisions can occur.
- A Broadcast Domain is where broadcast traffic is received.
- Hubs create a single Collision Domain.
- Switches create one Collision Domain per port.
- Routers separate Broadcast Domains.
- Each VLAN forms a separate Broadcast Domain.

---

# Summary

Collision Domains and Broadcast Domains are fundamental networking concepts used to manage network traffic efficiently. Modern switches reduce collisions by creating separate Collision Domains, while routers and VLANs control broadcast traffic by dividing networks into multiple Broadcast Domains.

# IP Addressing & Subnetting

## Introduction

An **IP Address (Internet Protocol Address)** is a unique logical address assigned to every device connected to a network.

Just as a house has a postal address for receiving letters, every device on a network needs an IP Address to send and receive data.

IP Addresses operate at **Layer 3 (Network Layer)** of the OSI Model.

---

# Why Do We Need an IP Address?

Imagine sending a message to your friend.

Without knowing your friend's address, the message cannot be delivered.

Similarly, routers use IP Addresses to identify the source and destination devices and forward packets correctly.

---

# What is an IP Address?

An IP Address is a numerical address assigned to a device.

Example:

```
192.168.1.10
```

Every device connected to a network should have a unique IP Address.

Examples:

- Computer
- Laptop
- Mobile Phone
- Server
- Printer
- Router

---

# Types of IP Addresses

## 1. IPv4

IPv4 is the most widely used version of IP.

Example:

```
192.168.1.10
```

Features:

- 32-bit Address
- Four Octets
- Written in Decimal

Example:

```
192.168.1.10

192 | 168 | 1 | 10
```

---

## 2. IPv6

IPv6 was introduced because IPv4 addresses are limited.

Example:

```
2001:db8::1
```

Features:

- 128-bit Address
- Much larger address space
- Better scalability

---

# Public IP vs Private IP

## Private IP

Used inside local networks.

Ranges:

```
10.0.0.0 – 10.255.255.255

172.16.0.0 – 172.31.255.255

192.168.0.0 – 192.168.255.255
```

Private IPs cannot be accessed directly from the Internet.

---

## Public IP

Assigned by an Internet Service Provider (ISP).

Public IPs are globally unique and accessible over the Internet.

---

# Static IP vs Dynamic IP

## Static IP

- Fixed Address
- Does not change
- Used for Servers

---

## Dynamic IP

- Assigned automatically by DHCP
- Can change over time
- Common for Home Networks

---

# Network ID and Host ID

Every IPv4 address consists of two parts:

```
Network ID | Host ID
```

Example:

```
192.168.1.25/24
```

Network:

```
192.168.1.0
```

Host:

```
25
```

The Network ID identifies the network, while the Host ID identifies a specific device.

---

# What is a Subnet?

A **Subnet (Subnetwork)** is a smaller network created by dividing a larger network into multiple smaller networks.

Subnetting helps:

- Reduce Broadcast Traffic
- Improve Performance
- Increase Security
- Better Network Management

---

# Example

Without Subnetting:

```
192.168.1.0/24

All devices belong to one network.
```

With Subnetting:

```
192.168.1.0/26

192.168.1.64/26

192.168.1.128/26

192.168.1.192/26
```

Now one large network becomes four smaller networks.

---

# What is a Subnet Mask?

A **Subnet Mask** tells the device which part of the IP Address represents the Network ID and which part represents the Host ID.

Example:

```
IP Address

192.168.1.20

Subnet Mask

255.255.255.0
```

CIDR notation:

```
/24
```

---

# CIDR Notation

CIDR (Classless Inter-Domain Routing) is a shorter way to represent a subnet mask.

Examples:

| CIDR | Subnet Mask |
|------|-------------|
| /8 | 255.0.0.0 |
| /16 | 255.255.0.0 |
| /24 | 255.255.255.0 |
| /30 | 255.255.255.252 |

---

# Why is Subnetting Important?

Subnetting helps to:

- Reduce Broadcast Domains
- Improve Network Performance
- Increase Security
- Efficiently Use IP Addresses
- Simplify Network Management

---

# IP Address vs MAC Address

| IP Address | MAC Address |
|------------|-------------|
| Logical Address | Physical Address |
| Layer 3 | Layer 2 |
| Can Change | Usually Permanent |
| Used by Routers | Used by Switches |

---

# Key Takeaways

- Every network device needs an IP Address.
- IP Address works at Layer 3.
- IPv4 uses 32 bits.
- IPv6 uses 128 bits.
- Private IPs are used inside local networks.
- Public IPs are used on the Internet.
- Subnetting divides a large network into smaller networks.
- CIDR notation is a shorter way to represent subnet masks.

---

# Summary

IP Addressing allows devices to communicate across networks by assigning unique logical addresses. Subnetting divides large networks into smaller and more efficient networks, improving performance, security, and IP address utilization.

# IP Header Fields

## Introduction

Whenever data travels across different networks, it is encapsulated into an **IP Packet**.

Every IP Packet contains two parts:

- IP Header
- Payload (Actual Data)

The **IP Header** contains important information that helps routers deliver packets to the correct destination.

---

# Structure of an IPv4 Header

```

+------------------------------------------------+
| Version | IHL | DSCP | Total Length |
+------------------------------------------------+
| Identification | Flags | Fragment Offset |
+------------------------------------------------+
| TTL | Protocol | Header Checksum |
+------------------------------------------------+
| Source IP Address |
+------------------------------------------------+
| Destination IP Address |
+------------------------------------------------+
| Options (Optional) |
+------------------------------------------------+
| Data (Payload) |
+------------------------------------------------+

```

---

# 1. Version

Indicates which version of IP is being used.

Example:

- IPv4 → Version = 4
- IPv6 → Version = 6

---

# 2. Internet Header Length (IHL)

Specifies the size of the IP Header.

Normally:

```

20 Bytes

```

If optional fields are added, the header becomes larger.

---

# 3. DSCP (Differentiated Services Code Point)

Used for **Quality of Service (QoS)**.

It allows important traffic, such as video calls or VoIP, to receive higher priority than normal traffic.

---

# 4. Total Length

Indicates the total size of the IP Packet.

It includes:

- Header
- Payload

---

# 5. Identification

Each packet is assigned a unique identification number.

If a large packet is divided into multiple fragments, this field helps the receiver identify which fragments belong together.

---

# 6. Flags

Flags control packet fragmentation.

The most common flags are:

- Don't Fragment (DF)
- More Fragments (MF)

---

# 7. Fragment Offset

Indicates the position of a fragment within the original packet.

The receiver uses this information to reassemble all fragments correctly.

---

# 8. Time To Live (TTL)

TTL prevents packets from circulating forever in the network.

Every router decreases the TTL value by **1**.

If TTL becomes **0**, the router discards the packet.

Example:

```

PC
 ↓ TTL = 64

Router 1
 ↓ TTL = 63

Router 2
 ↓ TTL = 62

```

---

# 9. Protocol

This field tells the receiver which Layer 4 protocol is carried inside the IP Packet.

Examples:

| Value | Protocol |
|--------|----------|
| 1 | ICMP |
| 6 | TCP |
| 17 | UDP |

---

# 10. Header Checksum

Used to detect errors in the IP Header.

If the checksum is incorrect, the packet is discarded.

---

# 11. Source IP Address

Contains the IP Address of the sender.

Example:

```

192.168.1.10

```

---

# 12. Destination IP Address

Contains the IP Address of the receiver.

Example:

```

8.8.8.8

```

Routers use this field to forward packets toward the destination.

---

# 13. Options (Optional)

Rarely used.

Can contain additional routing or diagnostic information.

---

# Payload

The Payload contains the actual user data.

Examples:

- HTTP Data
- HTTPS Data
- DNS Query
- Email
- File Data

---

# Packet Flow Example

```

Application Data
↓

TCP Header

↓

IP Header

↓

Ethernet Header

↓

Transmission

```

The IP Header helps routers deliver the packet correctly.

---

# Why is the IP Header Important?

Without the IP Header:

- Routers cannot forward packets.
- Devices cannot identify the sender or receiver.
- TTL cannot prevent routing loops.
- Fragmented packets cannot be reassembled.

---

# Key Takeaways

- Every IPv4 packet contains an IP Header.
- The IP Header controls routing and packet delivery.
- Source and Destination IP Addresses identify the communicating devices.
- TTL prevents packets from looping forever.
- The Protocol field identifies TCP, UDP, ICMP, and other protocols.
- Header Checksum detects errors in the header.

---

# Summary

The IPv4 Header contains all the essential information required for packet delivery across networks. Routers read the header fields to determine where a packet should go, while the receiving device uses them to verify and process the packet correctly.
# IPv6 (Internet Protocol Version 6)

## Introduction

IPv6 (Internet Protocol Version 6) is the latest version of the Internet Protocol.

It was developed to solve the problem of **IPv4 address exhaustion**, as the number of devices connected to the Internet continues to grow.

IPv6 provides a much larger address space, better efficiency, and improved support for modern networks.

---

# Why Do We Need IPv6?

IPv4 uses **32-bit addresses**, which can provide approximately **4.3 billion unique IP addresses**.

With billions of devices such as smartphones, laptops, IoT devices, and servers, IPv4 addresses are no longer sufficient.

IPv6 was introduced to overcome this limitation.

---

# IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|----------|------|------|
| Address Size | 32-bit | 128-bit |
| Format | Decimal | Hexadecimal |
| Example | 192.168.1.1 | 2001:db8::1 |
| Address Space | ~4.3 Billion | 340 Undecillion (Very Large) |
| NAT Required | Usually Yes | Usually No |
| Broadcast | Supported | Not Supported |

---

# IPv6 Address Format

IPv6 addresses contain **128 bits** and are written in **8 groups** of hexadecimal numbers.

Example:

```
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

Each group contains **4 hexadecimal digits**.

---

# Shortened IPv6 Address

Leading zeros can be removed.

Example:

```
2001:0db8:0000:0000:0000:0000:0000:0001

↓

2001:db8::1
```

The symbol `::` can replace one continuous sequence of zero groups.

---

# Types of IPv6 Addresses

## 1. Unicast

One sender communicates with one receiver.

Example:

```
PC A → PC B
```

---

## 2. Multicast

One sender communicates with multiple selected devices.

Example:

```
Server

↓

PC1
PC2
PC3
```

---

## 3. Anycast

Multiple devices share the same IPv6 address.

The packet is delivered to the **nearest available device**.

Used in:

- DNS Servers
- Cloud Services
- CDNs

---

# IPv6 Does Not Use Broadcast

Unlike IPv4, IPv6 does not support broadcast traffic.

Instead, it uses **Multicast**, which is more efficient and reduces unnecessary network traffic.

---

# IPv6 Header

Compared to IPv4, the IPv6 header is:

- Simpler
- Fixed size (40 Bytes)
- Faster to process
- More efficient for routers

---

# Advantages of IPv6

- Huge address space
- Better routing efficiency
- Improved performance
- Built-in support for IPsec
- No broadcast traffic
- Better support for IoT
- Simplified header structure

---

# IPv6 Address Types

| Type | Purpose |
|------|---------|
| Global Unicast | Public communication over the Internet |
| Link-Local | Communication within the same local network |
| Unique Local | Private communication inside an organization |
| Multicast | One-to-many communication |
| Anycast | One-to-nearest communication |

---

# IPv4 vs IPv6 Example

IPv4:

```
192.168.1.10
```

IPv6:

```
2001:db8::10
```

Both identify a device, but IPv6 provides a much larger address space.

---

# Why is IPv6 Important?

Modern technologies rely on IPv6 because:

- The Internet is growing rapidly.
- More devices require unique IP addresses.
- It improves scalability.
- It supports future networking needs.

---

# Key Takeaways

- IPv6 is the successor to IPv4.
- It uses 128-bit addresses.
- Addresses are written in hexadecimal format.
- IPv6 removes broadcast traffic.
- It provides a significantly larger address space.
- It is designed for modern Internet and cloud environments.

---

# Summary

IPv6 is the next-generation Internet Protocol designed to replace IPv4. It provides a massive address space, improved routing efficiency, simplified packet processing, and better support for modern networking technologies, making it essential for the future of the Internet.
