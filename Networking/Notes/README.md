Introduction to computer networks
- group of devices connected to each other allowing them to share info and resources

Local area network (LAN)
- samll covers small are
- Example home wifi

Widde area network WAN
- internet is an example

---

### Importance in modern infrastructure

Foundation - enables communication between devices

Resource sharing - Facilitates sharing of files printers and more

Internet functionality - critical for browsing, streaming and communication

Application support - backbone for app connectivity and data transfer


### Netorking in DevOps

Server interation - enables communication between servers and applications

Deployment - critical for launching and updating applicaitons

Management - cruical in monitioning and managing infrastructure

Opimisation - enhances troublue shooting, performance and scalability (data moving smooth and fast between devices)

---

## Network basics and types of networks - LAN & WAN etc

### Types of Networks

LAN
- small area e.g. home or office
- connects devices to share resource
- connects devices in a single locaiton e.g. printers, computers, internet access in a small area

WAN
- best example is internet which connects devices globally
- Large area e.g. citym country, larger region

---
## Switches, routers and firewalls

### Switches
- think of it as a manager of your LAN
- Connect devices within the same network e.g. cpu, printers
- Manage data flow within a LAN
- switches ensures data flows smoothly between these devices


### Routers
- like a traffic warden for a network e.g. router connets home network to internet. ensures data gets to the correct location, whether you are browsing, streaming etc.
- main role is to direct traffic between networks
- connect different networks e.g. home network to internet


### Firewalls
- acts as a bodyguard for your network
- Protect networks from unauthorised access
- monitors and controls incoming and outgoing network traffic based on predetermined security rules
---
## IP address (Internet protocol address) & MAC address

### IP Addressing 
- An IP address - unique for devises on a network
- Allows devices to locate and communicate
- The two types are IPv4 and IPv6

### IP Addressing (IPv4 & IPv6)
#### IPv4
- 192.168.0.5
- 32-bit address
- Format: four decinmal numbers separated by dots
- each group ranges from 0 to 255 providing around 4.3 billion unique addresses (rapid growth means we need IPv6)

#### IPv6
- 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- 128-bit address
- Format: eight groups of four hexadecimal digits separate by colons
- More enhanced: security and simplified address assignment

It is essential to transition into IPv6 due to continual growth of the internet.
Without IP Addresses, devices would not know where to send or receive data

### MAC Address (media access controll address)
- Unique identifer assigned to network interfaces.
- Each device on a network has its own unique MAC address
- importance - essential for network communication and security
- 48-bit address e.g. 00:1A:2B:3C:4D:5E
- operates at the datalink layer (Data link layer is responsibile for node ot node transfer)
- faciliates device identification within a local network (devices can identify each other e.g. your laptop connects to right router and not neighbours)
- without MAC addresses - critical for security and communication; devices would not be able to communicate properly. Help manage and control access to a network, ensuring data pakcets gets sent to the right place.
---
## Ports & Protocols: TCP, UDP

### What are ports?
- Logical end points for communicaiton
- think of it as a logical door on a device, each door is numbered and each number is used for a specific type of network communication e.g. web traffic typically goes through port 80 which is HTTP and port 443 for HTTPs
- these ports help faciliate communication between devices
- When your device wants to send/receive data, it uses ports to make sure the data goes to the right place.

### What are protocols?
- rules governing data transmission
- think of it as rules of the road for data transmission
- they define how data is formatted and transmitted across a network
- common protocols exmaples: HTTP, FTP, SMTP etc
- they ensure devices can communicate effectively by following the same set of rules (think of it as a language devices uses to communicate)

### Why are protocols important?
- faciliates communication between devices
- Ensures data gets to the right app on your device
- Esures data is understandable and properly formatted, they are essential for smooth and efficient communication.
- smooth and efficient communication

### TCP (Transmission contorl protocol)
- It is like the postman of the internet
- ensure data sent from one device reaches another device accurately and in the correct order
- set of rules that devices follow to communicate with eachother

### Characteristics of TCP
- it is connection oriented (a connection must be established before any data is sent between 2 devices e.g. a phone call, you must dial and connect before speaking)
- requires a 'handshake' - a process in which 2 devices agree to communicate
- handshake is a 3 step process to ensure both devices are ready to share data
- reliable data transfer - ensures all data sent is received correctly on the other end
- reliable - If any data is lost/corrupted, it will send it again.

### Function/Use cases of TCP
- Ensures data is delivered in order e.g. sending many messages, you want it to be in order
- error checking and flow control - checks for errors in the data and controls the flow of data to prevent congestion (ensures smooth and error free communicaiton)
- Any biderectional communication - used whenever two devices need to exchange data back and forth e.g. web browsing, emails and file transfers

Handshake is a 3 step process:
- 

### What is UDP (User Datagram Protocol)
- Simple protocol used to send/reecive data
- Unlike TCP, UDP is connectionless

### Characteristics of UDP
- simple protocol to share data (quick and easy to use)
- prior communication not required (can be adouble-edged sword) - Pro: data can be sent immedaitely without waiting to establish a connection. Con: no guarantee data will reach destination
- connectionless - no connection needs to be created between sender and receiver, each packet is sent independently.
- Fast but less reliable - no connection setup and less error checking, UDP is faster than TCP. Speed over accuracy

### Functions and use cases for UDP
- Suitable for real-time apps such as online gaming, videos and streaming (speed is more important than reliability)
- DNS, DNS lookups, DNS queries and anything DNS related uses UDP behind the scenes.
- VPN (Virtual private networks) - some VPN protocols use UDP because it is faster and works better for streaming and real time apps


### TCP vs UDP
![Screenshot 2024-10-22 at 00 33 08](https://github.com/user-attachments/assets/c5123801-6a5e-4ea7-a5ca-9d754b575675)

--- 


  






---
