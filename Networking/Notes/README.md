# README: Introduction to Computer Networks

---

## Introduction to Computer Networks

- A **computer network** is a group of devices connected to each other, allowing them to share information and resources.

### Local Area Network (LAN)
- Covers a small area, like a home or office.  
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
- **Management**: Vital for monitoring and managing infrastructure.  
- **Optimization**: Enhances troubleshooting, performance, and scalability, ensuring smooth data flow between devices.  

---

## Network Basics and Types of Networks

### Types of Networks

#### Local Area Network (LAN)
- Covers a small area, like a home or office.  
- Connects devices to share resources (e.g., printers, computers, internet access in a small area).

#### Wide Area Network (WAN)
- Connects devices across large areas (city, country, or larger region).  
- Connects multiple LANs.  
- **Example:** The internet, which connects devices globally.  

---

## Switches, Routers, and Firewalls

### Switches
- Acts as a manager within a **LAN**.  
- Connects devices within the same network (e.g., computers, printers).  
- Ensures data flows smoothly between devices within the LAN.  

### Routers
- Manages traffic between networks, such as a home network and the internet.  
- Connects different networks (e.g., home network to the internet).  
- Ensures data reaches the correct destination (e.g., while browsing or streaming).  

### Firewalls
- Protects the network from unauthorized access.  
- Monitors and controls incoming and outgoing network traffic based on security rules.  

---

## IP Address (Internet Protocol Address) & MAC Address

### IP Addressing
- An **IP address** uniquely identifies devices on a network, allowing them to locate and communicate with each other.  
- **Types**: IPv4 and IPv6.  

#### IPv4
- **Example:** `192.168.0.5` (32-bit address).  
- Four decimal numbers separated by dots (0–255), with around 4.3 billion unique addresses.  
- High demand has led to IPv4 scarcity, pushing migration to IPv6.  

#### IPv6
- **Example:** `2001:0db8:85a3:0000:0000:8a2e:0370:7334` (128-bit address).  
- Eight groups of four hexadecimal digits separated by colons, providing enhanced security and more unique addresses.  
- Simplifies address assignment.  

### MAC Address (Media Access Control Address)
- A unique identifier for network interfaces, operating at the Data Link layer.  
- **Example:** `00:1A:2B:3C:4D:5E` (48-bit address).  
- Facilitates device identification within a local network.  

---

## Ports & Protocols: TCP, UDP

### What Are Ports?
- **Ports** are logical endpoints for communication, each assigned a specific number for different types of network communication.  
- **Examples**: Port 80 for HTTP, Port 443 for HTTPS.  

### What Are Protocols?
- **Protocols** define rules governing data transmission, ensuring proper communication between devices.  
- **Examples**: HTTP, FTP, SMTP.  

---

## TCP (Transmission Control Protocol)
- Ensures data sent from one device reaches another accurately and in order.  

### Characteristics of TCP
- **Connection-Oriented**: Establishes a connection before data transmission.  
- **Handshake Process**: Devices synchronize and agree to communicate.  
- **Reliable**: Provides error checking and retransmits data if lost or corrupted.  

### Functions/Use Cases of TCP
- Suitable for bidirectional communication (e.g., web browsing, emails, file transfers).  
- Ensures data is delivered in order.  
- Includes error checking and flow control to prevent congestion.  

---

## UDP (User Datagram Protocol)
- A faster, connectionless protocol suitable for real-time applications where speed is prioritized over reliability.  

### Characteristics of UDP
- **Connectionless**: No formal connection between sender and receiver.  
- **Fast but less reliable**: No guarantee packets are delivered in order.  
- **No error checking or flow control**: What you send is what you get (errors included).  

### Functions/Use Cases of UDP
- Used for real-time applications like online gaming, video streaming, and some VPN protocols.  
- **DNS** (operates using UDP behind the scenes).  

---

## TCP vs. UDP  

![TCP vs. UDP](https://github.com/user-attachments/assets/c5123801-6a5e-4ea7-a5ca-9d754b575675)

---

## Introduction to the OSI Model

The **OSI Model** (Open Systems Interconnection) provides a standard framework for understanding how data is shared between devices in seven layers.

### Why We Need a Communication Model
- **Standard Framework**: Ensures devices communicate effectively.  
- **Application Independence**: Applications operate independently of the network.  
- **Simplified Network Management**: Easier upgrades and troubleshooting.  

---

## The 7 Layers of the OSI Model

| Layer | Name | Function |
|---|---|---|
| **7** | Application | Provides network services to applications (e.g., HTTP, FTP, DNS). |
| **6** | Presentation | Translates data into readable formats and handles encryption. |
| **5** | Session | Manages sessions between applications. |
| **4** | Transport | Ensures reliable communication using TCP/UDP. |
| **3** | Network | Handles packet routing and forwarding (e.g., IP, ICMP). |
| **2** | Data Link | Ensures node-to-node transfer and error detection (e.g., MAC addresses). |
| **1** | Physical | Transmits raw data (e.g., cables, wireless signals). |

---

## TCP/IP Model
- A compressed version of the OSI model with only four layers:  
  1. **Application** (e.g., HTTP, TLS, DNS)  
  2. **Transport** (e.g., TCP, UDP)  
  3. **Internet** (IP addressing and routing)  
  4. **Network Access** (Ethernet, wireless)  

---

## DNS (Domain Name System)

- DNS makes IP addresses human-friendly, allowing easy access to websites.  
- **Function**: Translates domain names into IP addresses.  

### DNS Components

#### Name Servers
- **Authoritative Name Servers**: Store actual DNS records.  
- **Recursive Name Servers**: Query other servers on behalf of the client.  

#### Zone Files
- Store domain-related information.  
- Organize DNS data efficiently.  

#### DNS Records
| Type | Function | Example |
|---|---|---|
| **A** | Maps a domain to an IPv4 address | google.com → 216.58.204.79 |
| **AAAA** | Maps a domain to an IPv6 address | google.com → 2a00:1450:4009:81d::200e |
| **CNAME** | Alias for another domain | www.google.com → google.com |
| **MX** | Specifies mail servers for a domain | google.com → mailserver.google.com |
| **TXT** | Stores verification and SPF data | google.com → "v=spf1 include.com ~all" |

---

Your README file is now structured properly in Markdown with clean formatting. 🚀  
