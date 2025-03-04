# README: Introduction to Computer Networks

---

## Introduction to Computer Networks

- A **computer network** is a group of devices connected to each other, allowing them to share information and resources.

### Local Area Network (LAN)

- Covers a small area, like a home or office. Can communicate 
- **Example:** Home Wi-Fi.

### Wide Area Network (WAN)

- Covers a large area, such as a city or country.
- **Example:** The internet.

---

## Importance in Modern Infrastructure

- **Foundation**: Enables communication between devices.
- **Resource Sharing**: Facilitates sharing of files, printers, and more.
- **Internet Functionality**: Essential for browsing, streaming, and communication.
- **Application Support**: Backbone for app connectivity and data transfer.

---

## Networking in DevOps

- **Server Interaction**: Enables communication between servers and applications.
- **Deployment**: Crucial for launching and updating applications.
- **Management**: Vital in monitoring and managing infrastructure.
- **Optimization**: Enhances troubleshooting, performance, and scalability (ensures data moves smoothly between devices).

---

## Network Basics and Types of Networks - LAN & WAN

### Types of Networks

**LAN**  
- Covers a small area, like a home or office.
- Connects devices to share resources (e.g., printers, computers, internet access in small area).

**WAN**  
- Connects devices across large areas (city, country, or larger region).
- Connects multiple LANs
- **Example:** The internet, which connects devices globally.


---

## Switches, Routers, and Firewalls

### Switches
- Acts as a manager within a **LAN**.
- Connects devices within the same network (e.g., computers, printers).
- Ensures data flows smoothly between devices within the LAN.

### Routers
- Manages traffic between networks, such as a home network and the internet.
- Connects different networks e.g. home network to internet.
- Ensures data reaches the correct destination (e.g., while browsing or streaming).
  
### Firewalls
- Protects the network from unauthorized access.
- Monitors and controls incoming and outgoing network traffic based on security rules.
- Monitors network traffic to enhance security

---

## IP Address (Internet Protocol Address) & MAC Address

### IP Addressing
- An **IP address** uniquely identifies devices on a network, allowing them to locate and communicate with each other.
- **Types**: IPv4 and IPv6.

#### IPv4
- **Example:** 192.168.0.5 (32-bit address).
- Four decimal numbers separated by dots (0–255), with around 4.3 billion unique addresses.
- too much demand making IPv4 scarce and moving into IPv6

#### IPv6
- **Example:** 2001:0db8:85a3:0000:0000:8a2e:0370:7334 (128-bit address).
- Eight groups of four hexadecimal digits separated by colons, providing enhanced security and more unique addresses.
- provides simple address assignment

### MAC Address (Media Access Control Address)
- A unique identifier for network interfaces, operating at the Data Link layer.
- **Example:** 00:1A:2B:3C:4D:5E (48-bit address).
- Facilitates device identification within a local network and is essential for security and communication.
- Operate on datalink layer (responsible for node to node transfer)

---

## Ports & Protocols: TCP, UDP

### What Are Ports?
- **Ports** are logical endpoints for communication, each assigned a specific number for different types of network communication.
- **Examples**: Port 80 for HTTP, Port 443 for HTTPS.

### What Are Protocols?
- **Protocols** are rules governing data transmission, ensuring data is formatted and transmitted correctly across a network.
- devices communication effectively by following the same set of rules. (e.g. devices must speak same language to understand eachother)
- **Examples**: HTTP, FTP, SMTP.

### TCP (Transmission Control Protocol)
- Ensures data sent from one device reaches another device accurately and in order.
- Set of rules devices follow to communicate with each other.

### Characteristics of TCP
- **Connection-Oriented**: Establishes a connection before data transmission.
- **hand shake**: the two devices agree to communicate.
- **Reliable**: Provides error checking and retransmits data if lost or corrupted. Ensures data sent gets received.

### Functions/Use Cases of TCP
- Suitable for bidirectional communication (when 2 devices need to exchange data back and forth) e.g. such as web browsing, emails, and file transfers.
- Ensure data is delivered in order.
- Error checking and flow control to prvent congestion.

### UDP (User Datagram Protocol)
- A faster, connectionless protocol suitable for real-time apps where speed is more critical than reliability.

### UDP Characteristics
- Simple protocol to send and receive data
- Priot comminication not required (has cons e.g. data can be sent immediately without establishing a connection, however there is no guarantee data reached desired location)
- connectionaless: no formal connection established between sender and receiver. Each packet is sent independently.
- Fast but less reliable. No guarantee packets are delivered in order.
- No error checking or flow control, what you send is what you get (errors included).

### Functions/Use Cases of UDP
- Used for real time application e.g. in online gaming, video streaming, and some VPN protocols.
- DNS (use udp behind the scenes)
- Some VPN use udp because it is faster and works better for streaming and real time applications

### TCP vs. UDP

![TCP vs. UDP](https://github.com/user-attachments/assets/c5123801-6a5e-4ea7-a5ca-9d754b575675)

---

## Introduction to OSI Model

The **OSI Model** (Open Systems Interconnection) provides a standard framework for understanding how data is shared between devices in seven layers.

---

## The 7 Layers of the OSI Model

### Why We Need a Communication Model

- **Standard Framework**: Simplifies device and app communication over a network (all devices can understand each other)
- **Application Independence**: Applications operate independently of the underlying network.
- **Simplified Network Management**: Facilitates easier upgrades.
- **Decoupled Innovation**: Allows updates on each layer independently.

### OSI Layers

#### Layer 7: Application Layer
- Directly provides network services to applications (e.g., HTTP, FTP, DNS).
- end user layer

#### Layer 6: Presentation Layer
- Translates data into a readable format and handles encryption.
- syntax user layer
- e.g. ssl, ssh, imap, mpeg, jpeg

#### Layer 5: Session Layer
- Manages sessions between applications, establishing and terminating connections.
- sync and send to port
- API's, sockets, winsock

#### Layer 4: Transport Layer
- Ensures end-to-end communication and data integrity (e.g., TCP, UDP).

#### Layer 3: Network Layer
- Manages packet routing and forwarding of data (e.g.IP, ICMP, IPSec, IGMP).

#### Layer 2: Data Link Layer
- Ensures node-to-node data transfer and error detection (e.g., Ethernet, MAC addresses, PPP, Switch, Bridge).
- Frames

#### Layer 1: Physical Layer
- Transmits raw bit streams over a physical medium (e.g., cables, wireless signals).
- Physical structure

---

## Layer Details

### Layer 1: Physical Layer
**Function**:
- Transmit raw bit streams over physical media (e.g., cables, network interface cards).
- No device addressing (all data processed by all devices)

### Layer 2: Data Link Layer
**Function**:
- Ensures node-to-node data transfer and detects errors from the physical layer. Ensures data is transferred correctly between adjacent network nodes.
- Ensures data packets are correctly sent/received between different network nodes.
- puts data packets into frames (like an enevlope with an address ensuring it goes to the right place)
- compnents: mac addresses, switches and bridges

### Layer 3: Network Layer
**Function**:
- How the data is sent to the recepient. 
- Routes data packets to the recipient, managing paths through intermediate routers.
- Manages packet forwarding including routing through intermediate routers.
- Chooses best path for data to travel.
- Components: IP addresses (handles where packets go to), routers
- Data organised into packets (carries data to target)

### Layer 4: Transport Layer
**Function**:
- Provides reliable data transfer services to the upper layers, segmenting and reassembling data as needed.
- End-to-end connextions
- Components: TCP (provides reliable audit and error free data), UDP (less reliable and not guaranteed) 

### Layer 5: Session Layer
**Function**:
- Manages sessions between applications, establishing, maintaining (keeping session alive), and terminating connections.
- Synch and send to port
- API's, Sockets, Winsock
- Components: Session management protocols e.g. RPC, NetBIOS etc

### Layer 6: Presentation Layer
**Function**: 
- Translates data between application layer and network layer
- Ensures data is in a usable format and handles encryption.
- aka syntax layer
- Components: Encryption (ensure data security), data formatting 

### Layer 7: Application Layer
**Function**: 
- Directly provides network services to applications.
- End user layer
- Components: HTTP (for access websites and web services), FTP (for trasferring files between different servers), SMTP (for sending emails)
