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
