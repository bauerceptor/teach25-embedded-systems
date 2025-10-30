---
layout: satellite
title: "Exercise Solutions - Computer Networks"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, Computer Networks]
tags: [networking, LAN, WAN, OSI model, TCP/IP, IP addressing, network topology, IoT]
---

# Exercise Solutions: Computer Networks

## Part A: Multiple Choice Questions

### 1. A network that connects devices within a single building is called:
**Answer: b) LAN (Local Area Network)**

**Explanation:** A Local Area Network (LAN) is designed to connect devices within a limited geographical area such as a single building, office, or campus. LANs typically provide high-speed connectivity and are owned and managed by a single organization. Examples include office networks, home networks, and school computer labs.

### 2. Which device operates at the Physical Layer of the OSI model?
**Answer: a) Hub**

**Explanation:** A hub operates at the Physical Layer (Layer 1) of the OSI model. It simply repeats electrical signals received on one port to all other ports without any intelligence about the data content. Hubs do not examine MAC addresses or make forwarding decisions, making them purely physical layer devices. Switches operate at Layer 2, routers at Layer 3, and gateways can operate at multiple layers.

### 3. The maximum cable length for 10Base2 Ethernet is:
**Answer: c) 185 meters**

**Explanation:** 10Base2, also known as Thin Ethernet or Thinnet, uses thin coaxial cable (RG-58) and has a maximum segment length of 185 meters. The "10" represents 10 Mbps speed, "Base" indicates baseband transmission, and "2" originally meant 200 meters but the actual specification limits it to 185 meters due to signal attenuation and timing constraints.

### 4. Which topology provides the highest fault tolerance?
**Answer: d) Mesh**

**Explanation:** Mesh topology provides the highest fault tolerance because it offers multiple redundant paths between devices. In a full mesh topology, every device is connected to every other device, ensuring that if one connection fails, alternative paths are available. This redundancy makes mesh networks highly reliable but also more expensive and complex to implement.

### 5. The IP address 192.168.1.100 belongs to which class?
**Answer: c) Class C**

**Explanation:** IP addresses in the range 192.0.0.0 to 223.255.255.255 belong to Class C. The first octet (192) falls within this range, making 192.168.1.100 a Class C address. Additionally, 192.168.x.x addresses are private IP addresses reserved for internal networks and not routable on the public internet.

### 6. Which protocol is connectionless?
**Answer: b) UDP (User Datagram Protocol)**

**Explanation:** UDP is a connectionless protocol that does not establish a connection before sending data and does not guarantee delivery, ordering, or error correction. It provides fast, low-overhead communication suitable for applications like streaming media, online gaming, and DNS queries where speed is more important than reliability. TCP, in contrast, is connection-oriented and provides reliable delivery.

### 7. The default subnet mask for a Class B network is:
**Answer: b) 255.255.0.0**

**Explanation:** Class B networks use a default subnet mask of 255.255.0.0, which in binary has the first 16 bits set to 1 (network portion) and the last 16 bits set to 0 (host portion). This allows for 16,384 networks with 65,534 hosts each. Class B addresses range from 128.0.0.0 to 191.255.255.255.

### 8. Which layer of the OSI model handles routing?
**Answer: c) Network Layer (Layer 3)**

**Explanation:** The Network Layer (Layer 3) of the OSI model is responsible for routing packets between different networks. It uses logical addressing (IP addresses) to determine the best path for data to travel from source to destination across multiple networks. Routers operate primarily at this layer, making forwarding decisions based on routing tables and protocols.

### 9. What does 'ping' command test?
**Answer: a) Network connectivity**

**Explanation:** The ping command tests network connectivity between two devices by sending ICMP (Internet Control Message Protocol) Echo Request packets to a destination and waiting for Echo Reply packets. It measures round-trip time and packet loss, helping network administrators diagnose connectivity issues and network performance problems.

### 10. Which cable type is immune to electromagnetic interference?
**Answer: c) Fiber optic**

**Explanation:** Fiber optic cables use light signals transmitted through glass or plastic fibers, making them completely immune to electromagnetic interference (EMI). Unlike copper-based cables (coaxial and twisted-pair) that carry electrical signals and can be affected by EMI, fiber optic cables provide superior performance in electrically noisy environments and offer higher bandwidth and longer transmission distances.

## Part B: Short Answer Questions

### 1. Define computer network and list three main benefits.

**Answer:** A computer network is a collection of interconnected devices that can communicate and share resources with each other. These devices include computers, servers, printers, mobile devices, and IoT sensors connected through various communication media.

**Three Main Benefits:**
1. **Resource Sharing:** Multiple users can access shared files, printers, applications, and internet connections, reducing costs and improving efficiency
2. **Communication:** Networks enable email, messaging, video conferencing, and collaboration tools that facilitate communication between users regardless of their physical location
3. **Data Exchange:** Networks allow efficient transfer of information between different systems, enabling real-time data sharing and synchronized operations across multiple devices

### 2. Explain the difference between LAN and WAN.

**Answer:**

| Aspect | LAN (Local Area Network) | WAN (Wide Area Network) |
|--------|-------------------------|------------------------|
| **Coverage Area** | Limited geographical area (building, campus) | Large geographical area (cities, countries, continents) |
| **Speed** | High speed (10 Mbps to 10+ Gbps) | Varies (dial-up to high-speed fiber) |
| **Ownership** | Single organization | Multiple telecommunications providers |
| **Cost** | Lower implementation and maintenance costs | Higher costs for long-distance infrastructure |
| **Technology** | Ethernet, WiFi | Satellites, fiber optic, telephone lines |
| **Latency** | Low latency | Higher latency due to distance |
| **Examples** | Office network, home network | Internet, corporate networks spanning multiple cities |

### 3. Describe the functions of a router in a network.

**Answer:** A router is a networking device that connects different networks and determines the best path for data transmission between them.

**Key Functions:**
1. **Path Determination:** Analyzes routing tables and uses routing protocols to find the optimal path for data packets to reach their destination across multiple networks
2. **Packet Forwarding:** Receives data packets and forwards them to the next appropriate hop based on destination IP addresses and routing decisions
3. **Network Interconnection:** Connects different network segments, enabling communication between devices on separate networks with different IP address ranges
4. **Traffic Control:** Manages data flow between networks, implements access control policies, and can prioritize certain types of traffic for Quality of Service (QoS)
5. **Network Address Translation (NAT):** Allows devices with private IP addresses to access the internet by translating between private and public IP addresses
6. **Security Implementation:** Provides basic firewall functionality, access control lists, and can implement security policies to protect networks

### 4. What are the advantages and disadvantages of wireless networks?

**Answer:**

**Advantages:**
1. **Mobility and Flexibility:** Users can move freely within coverage area while maintaining network connectivity
2. **Easy Installation:** No need for extensive cable infrastructure, reducing installation time and complexity
3. **Cost-Effective:** Lower installation costs, especially for temporary or hard-to-reach locations
4. **Scalability:** Easy to add new devices without running additional cables
5. **Accessibility:** Provides network access in areas where cable installation is impractical

**Disadvantages:**
1. **Security Vulnerabilities:** Wireless signals can be intercepted, requiring strong encryption and security protocols
2. **Interference:** Radio frequency interference from other devices can affect performance and reliability
3. **Limited Bandwidth:** Generally lower bandwidth compared to wired connections, shared among all connected devices
4. **Range Limitations:** Signal strength decreases with distance and can be blocked by physical obstacles
5. **Battery Dependency:** Mobile devices require battery power, limiting continuous operation
6. **Weather Sensitivity:** Outdoor wireless links can be affected by weather conditions

### 5. Explain the OSI model and its purpose.

**Answer:** The Open Systems Interconnection (OSI) model is a conceptual framework that standardizes the functions of network communication into seven distinct layers. Each layer has specific responsibilities and communicates with adjacent layers.

**Purpose:**
- **Standardization:** Provides a common reference for network protocol development and implementation
- **Interoperability:** Enables different vendors' equipment to work together
- **Troubleshooting:** Helps isolate network problems to specific layers
- **Education:** Serves as a teaching tool for understanding network communication

**The Seven Layers:**
1. **Physical Layer (Layer 1):** Defines physical transmission medium, electrical specifications, and hardware connections
2. **Data Link Layer (Layer 2):** Handles error detection, frame formatting, and MAC addressing for local network communication
3. **Network Layer (Layer 3):** Manages logical addressing (IP addresses) and routing between different networks
4. **Transport Layer (Layer 4):** Provides reliable end-to-end communication, error recovery, and flow control
5. **Session Layer (Layer 5):** Manages communication sessions between applications
6. **Presentation Layer (Layer 6):** Handles data formatting, encryption, and compression
7. **Application Layer (Layer 7):** Provides network services directly to end-users and applications

### 6. Compare TCP and UDP protocols.

**Answer:**

| Feature | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
|---------|-----------------------------------|----------------------------|
| **Connection Type** | Connection-oriented | Connectionless |
| **Reliability** | Reliable delivery with acknowledgments | No guarantee of delivery |
| **Error Checking** | Comprehensive error detection and correction | Basic error detection only |
| **Ordering** | Maintains packet order | No ordering guarantee |
| **Flow Control** | Built-in flow control mechanisms | No flow control |
| **Speed** | Slower due to overhead | Faster with minimal overhead |
| **Header Size** | 20 bytes minimum | 8 bytes fixed |
| **Applications** | Web browsing, email, file transfer | Streaming media, gaming, DNS |
| **Use Case** | When reliability is critical | When speed is more important than reliability |

### 7. What is subnetting and why is it used?

**Answer:** Subnetting is the process of dividing a large network into smaller, more manageable subnetworks (subnets) by borrowing bits from the host portion of an IP address to create additional network portions.

**Why Subnetting is Used:**
1. **Improved Performance:** Reduces broadcast traffic by creating smaller broadcast domains, improving overall network performance
2. **Enhanced Security:** Enables network segmentation, allowing different security policies for different network segments
3. **Efficient Address Utilization:** Prevents waste of IP addresses by creating appropriately sized subnets for different purposes
4. **Better Network Management:** Makes networks easier to administer, monitor, and troubleshoot
5. **Reduced Congestion:** Distributes network traffic across multiple segments, reducing congestion on any single segment
6. **Organizational Structure:** Allows network design to match organizational structure (departments, floors, functions)

**Example:** A Class C network 192.168.1.0/24 can be subnetted into four /26 subnets:
- 192.168.1.0/26 (hosts 1-62)
- 192.168.1.64/26 (hosts 65-126)
- 192.168.1.128/26 (hosts 129-190)
- 192.168.1.192/26 (hosts 193-254)

### 8. Describe three types of network cables and their characteristics.

**Answer:**

**1. Twisted-Pair Cable:**
- **Structure:** Pairs of insulated copper wires twisted together to reduce electromagnetic interference
- **Types:** Unshielded Twisted Pair (UTP) and Shielded Twisted Pair (STP)
- **Categories:** Cat5e (1 Gbps), Cat6 (1-10 Gbps), Cat6a (10 Gbps)
- **Distance:** Up to 100 meters for Ethernet applications
- **Advantages:** Cost-effective, easy to install, widely available
- **Disadvantages:** Susceptible to EMI, limited distance without repeaters
- **Applications:** Ethernet LANs, telephone systems, building automation

**2. Coaxial Cable:**
- **Structure:** Central copper conductor surrounded by insulation, metallic shield, and outer jacket
- **Types:** Thick coax (10Base5) and thin coax (10Base2)
- **Impedance:** 50 ohms for data networks, 75 ohms for cable TV
- **Distance:** Several hundred meters without amplification
- **Advantages:** Good EMI resistance, supports high frequencies, reliable for long distances
- **Disadvantages:** Bulky, difficult to install, single point of failure in bus topology
- **Applications:** Cable TV networks, broadband internet, legacy Ethernet

**3. Fiber Optic Cable:**
- **Structure:** Glass or plastic core carrying light signals, surrounded by cladding and protective layers
- **Types:** Single-mode (long distance) and multimode (shorter distance)
- **Speed:** Up to 100+ Gbps over long distances
- **Distance:** Kilometers without signal degradation
- **Advantages:** Highest bandwidth, immune to EMI, secure transmission, future-proof
- **Disadvantages:** Expensive, requires specialized skills, fragile installation
- **Applications:** Internet backbone, data centers, campus networks, long-distance telecommunications

## Part C: Practical Exercises

### 1. Calculate subnet information for the network 192.168.10.0/24 divided into 4 subnets.

**Solution:**

**Given Information:**
- Original network: 192.168.10.0/24
- Required subnets: 4
- Subnet bits needed: 2 bits (2² = 4 subnets)
- New subnet mask: /26 (24 + 2 = 26)

**Subnet Calculations:**

**Subnet 1: 192.168.10.0/26**
- Network address: 192.168.10.0
- Subnet mask: 255.255.255.192
- First usable host: 192.168.10.1
- Last usable host: 192.168.10.62
- Broadcast address: 192.168.10.63
- Number of hosts: 62

**Subnet 2: 192.168.10.64/26**
- Network address: 192.168.10.64
- Subnet mask: 255.255.255.192
- First usable host: 192.168.10.65
- Last usable host: 192.168.10.126
- Broadcast address: 192.168.10.127
- Number of hosts: 62

**Subnet 3: 192.168.10.128/26**
- Network address: 192.168.10.128
- Subnet mask: 255.255.255.192
- First usable host: 192.168.10.129
- Last usable host: 192.168.10.190
- Broadcast address: 192.168.10.191
- Number of hosts: 62

**Subnet 4: 192.168.10.192/26**
- Network address: 192.168.10.192
- Subnet mask: 255.255.255.192
- First usable host: 192.168.10.193
- Last usable host: 192.168.10.254
- Broadcast address: 192.168.10.255
- Number of hosts: 62

### 2. Design a network topology for a small office with 25 computers, 2 printers, and 1 server.

**Solution:**

**Recommended Topology: Star Topology with Hierarchical Design**

**Network Components:**
1. **Core Layer:**
   - 1 x 24-port managed switch (primary)
   - 1 x 8-port switch (expansion for future growth)
   - 1 x Router with firewall capabilities
   - 1 x Uninterruptible Power Supply (UPS)

2. **Distribution Layer:**
   - Connect switches using high-speed uplinks
   - Implement VLANs for network segmentation

3. **Access Layer:**
   - All end devices connect to access switches
   - Structured cabling to each workstation

**Network Segmentation (VLANs):**

**VLAN 10 - Management (192.168.10.0/24):**
- Network infrastructure devices
- 10 IP addresses allocated

**VLAN 20 - Servers (192.168.20.0/24):**
- File server: 192.168.20.10
- Backup and domain services
- 20 IP addresses allocated

**VLAN 30 - Workstations (192.168.30.0/24):**
- Employee computers: 192.168.30.11-192.168.30.35
- DHCP pool: 192.168.30.50-192.168.30.100
- 100 IP addresses allocated for growth

**VLAN 40 - Printers (192.168.40.0/24):**
- Printer 1: 192.168.40.10 (static)
- Printer 2: 192.168.40.11 (static)
- Print servers and related services
- 20 IP addresses allocated

**Physical Layout:**
```
Internet
    |
[Router/Firewall]
    |
[24-port Main Switch]
    |
    +--- Server (direct connection)
    +--- Printer 1 (direct connection)
    +--- Printer 2 (direct connection)
    +--- [8-port Switch] --- Workstations 21-25
    +--- Workstations 1-20 (direct connections)
```

**Cable Requirements:**
- Cat6 UTP cables for all connections
- Patch panels for organized cable management
- Cable management system for neat installation
- Redundant uplinks between switches

**Security Considerations:**
- Firewall rules between VLANs
- Access control for server VLAN
- Guest network isolation if needed
- Regular security updates and monitoring

**Advantages of This Design:**
- Scalable for future growth
- Centralized management
- Network segmentation for security
- Single points of failure minimized
- Easy troubleshooting and maintenance

### 3. Configure static IP addresses for a network with the following requirements:
   - Network: 172.16.5.0/24
   - Server: First usable IP
   - Printer: Second usable IP
   - Router: Last usable IP

**Solution:**

**Network Analysis:**
- Network: 172.16.5.0/24
- Subnet mask: 255.255.255.0
- Network address: 172.16.5.0
- Broadcast address: 172.16.5.255
- First usable IP: 172.16.5.1
- Last usable IP: 172.16.5.254
- Total usable IPs: 254

**Static IP Configuration:**

**Server Configuration:**
- IP Address: 172.16.5.1
- Subnet Mask: 255.255.255.0
- Default Gateway: 172.16.5.254
- DNS Servers: 8.8.8.8, 8.8.4.4

**Printer Configuration:**
- IP Address: 172.16.5.2
- Subnet Mask: 255.255.255.0
- Default Gateway: 172.16.5.254
- DNS Servers: 8.8.8.8, 8.8.4.4

**Router Configuration:**
- LAN Interface IP: 172.16.5.254
- Subnet Mask: 255.255.255.0
- DHCP Pool: 172.16.5.10 - 172.16.5.200
- Reserved Addresses: 172.16.5.1-172.16.5.9 (static assignments)

**Windows Static IP Configuration Steps:**
1. Open Network and Sharing Center
2. Click "Change adapter settings"
3. Right-click network adapter and select "Properties"
4. Select "Internet Protocol Version 4 (TCP/IPv4)"
5. Click "Properties"
6. Select "Use the following IP address"
7. Enter IP address, subnet mask, and default gateway
8. Enter DNS server addresses
9. Click "OK" to save settings

**Linux Static IP Configuration (/etc/netplan/ for Ubuntu):**
```yaml
network:
  version: 2
  ethernets:
    eth0:
      addresses:
        - 172.16.5.1/24
      gateway4: 172.16.5.254
      nameservers:
        addresses: [8.8.8.8, 8.8.4.4]
```

**Verification Commands:**
```bash
# Windows
ipconfig /all
ping 172.16.5.254

# Linux
ip addr show
ping 172.16.5.254
```

### 4. Plan cable installation for a two-story office building with 15 computers per floor.

**Solution:**

**Building Assessment:**
- 2 floors with 15 computers each
- Total of 30 network drops required
- Additional infrastructure devices
- Future expansion considerations

**Cable Infrastructure Design:**

**Main Distribution Frame (MDF) - First Floor:**
- Location: Central, secure room with proper ventilation
- 48-port patch panel
- Network switches and routers
- UPS power backup
- Cable management systems

**Intermediate Distribution Frame (IDF) - Second Floor:**
- Location: Similar to MDF requirements
- 24-port patch panel
- Layer 2 switch
- Fiber uplink to MDF

**Horizontal Cabling System:**

**First Floor (15 workstations + infrastructure):**
- 18 Cat6 UTP cable runs (15 workstations + 3 spare)
- Maximum distance: 90 meters from patch panel to outlet
- Cable routing through ceiling or raised floor
- Wall outlets at each workstation location

**Second Floor (15 workstations):**
- 18 Cat6 UTP cable runs (15 workstations + 3 spare)
- Terminate at IDF patch panel
- Wall outlets at each workstation location

**Vertical Backbone Cabling:**
- 2 x multimode fiber cables (primary and backup)
- Route through dedicated risers or conduits
- Connect MDF to IDF
- Support 1-10 Gbps speeds

**Cable Specifications:**

**Horizontal Cables:**
- Type: Cat6 UTP (23 AWG solid conductor)
- Length: Cut to appropriate length + 10% extra
- Certification: TIA/EIA-568-B standard
- Fire rating: Plenum-rated for ceiling installation

**Fiber Backbone:**
- Type: 62.5/125 multimode fiber
- Connector: LC or SC connectors
- Length: Measure vertical distance + routing path
- Protection: Armored cable if needed

**Installation Process:**

**Phase 1: Planning and Preparation**
1. Conduct detailed site survey
2. Create detailed cable routing diagrams
3. Obtain building permits if required
4. Coordinate with other trades (electrical, HVAC)
5. Order cables and materials

**Phase 2: Rough-in Installation**
1. Install cable trays and conduits
2. Pull horizontal cables to outlet locations
3. Install backbone fiber between floors
4. Label all cables with unique identifiers
5. Test cables for continuity

**Phase 3: Termination and Testing**
1. Install patch panels in MDF and IDF
2. Terminate horizontal cables
3. Install fiber termination equipment
4. Terminate fiber connections
5. Install wall outlets at workstations

**Phase 4: Testing and Documentation**
1. Test all cable runs with cable tester
2. Certify installation meets TIA standards
3. Create as-built documentation
4. Label all connections clearly
5. Provide test results and warranties

**Materials List:**

**Cables:**
- 3000 feet Cat6 UTP cable (plenum-rated)
- 200 feet multimode fiber cable
- Cable ties and organizing materials

**Hardware:**
- 48-port patch panel (MDF)
- 24-port patch panel (IDF)
- Wall outlets (40 pieces with faceplates)
- Fiber patch panel and adapters
- Cable management bars and rings

**Tools Required:**
- Cable pulling equipment
- Cable tester/certifier
- Punch-down tools
- Fiber fusion splicer or connectors
- Labeling equipment

**Testing Requirements:**
- Continuity testing for all cable runs
- Length measurement within specifications
- Near-end crosstalk (NEXT) testing
- Attenuation testing
- Return loss measurement
- Fiber power loss testing

**Documentation Deliverables:**
- Cable installation drawings
- Test results for each cable run
- Labeling scheme documentation
- Warranty information
- Maintenance recommendations

---

*These solutions provide comprehensive guidance for understanding and implementing computer networking concepts, from basic theory to practical application scenarios.*