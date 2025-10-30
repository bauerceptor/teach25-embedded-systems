---
title: "Exercise Solutions - Computer Networks"
date: "2025-10-25"
thumbnail: "/assets/img/thumbnail/bricks.jpg"
bookmark: true
---

# Exercise Solutions: Computer Networks

*These solutions provide comprehensive guidance for understanding and implementing computer networking concepts, from basic theory to practical application scenarios.*

## Select the most appropriate option

### 1. Which of the following is the hardware/physical address of a computer?
a. IP Address  
b. MAC Address  
c. Static IP  
d. Subnet Mask

**Answer: b. MAC Address**

**Explanation:** MAC (Media Access Control) Address is the hardware or physical address that uniquely identifies a network adapter on a LAN. It is a 48-bit address permanently assigned to the network interface card.

### 2. Speed of data is expressed in:
a. Hz/s  
b. words/s  
c. bits/s  
d. bits/min

**Answer: c. bits/s**

**Explanation:** Data speed is measured in bits per second (bits/s or bps). This represents the number of bits that can be transmitted in one second.

### 3. Which of the following is not an active network component?
a. Cable  
b. Router  
c. Hub  
d. Switch

**Answer: a. Cable**

**Explanation:** Cables are passive network components as they simply carry signals without amplifying, modifying, or processing them. Active components like routers, hubs, and switches actively process and manage network signals.

### 4. Ping is used to
a. Assign IP  
b. Login  
c. Test a network  
d. search files

**Answer: c. Test a network**

**Explanation:** Ping is a network diagnostic tool used to test connectivity between devices and measure round-trip time using ICMP packets.

### 5. There are ____ classes of IP addresses.
a. 4  
b. 3  
c. 5  
d. None of these

**Answer: c. 5**

**Explanation:** TCP/IP defines five classes of IP addresses: Class A, B, C, D, and E. Classes A, B, and C are used for host addresses, Class D for multicast, and Class E for experimental purposes.

## Write short answer of the following.

### 1. Define Computer Networks.

A computer network is a group of computers linked to each other that enables them to communicate with each other and share their resources, data, and applications. It allows devices to exchange information and access shared resources like files, printers, and internet connections.

### 2. Differentiate between wired and wireless networks.

**Wired Networks:**
- Use physical cables for data transmission
- Higher security and reliability
- Limited mobility due to cable connections
- Better performance and speed
- Lower installation costs for permanent setups

**Wireless Networks:**
- Use radio waves for data transmission
- Greater mobility and flexibility
- Potential security vulnerabilities
- Easy installation without cable infrastructure
- May have interference and performance issues

### 3. What is the difference between access point and stations?

**Access Points:**
- Devices that create wireless networks
- Host and control wireless connections
- Bridge between wireless and wired networks
- Operate in "Master" or "Infrastructure" mode
- Manage multiple client connections

**Stations (Wireless Clients):**
- Devices that connect to wireless networks
- Include computers, tablets, phones
- Operate in "Station" or "Client" mode
- Request and receive services from access points
- Cannot directly connect to other stations

### 4. Define Router.

A router is a network device that connects different networks and determines the best path for data transmission between them. It operates at the Network Layer and routes data packets based on their IP addresses. Routers maintain routing tables and make decisions about forwarding packets to their destinations across multiple networks.

### 5. Define Switch.

A switch is a network device that connects devices in a LAN and forwards data only to the intended recipient. It operates at the Data Link Layer and uses MAC addresses to deliver messages to the correct destination port. Unlike hubs, switches create separate collision domains for each port and can perform full-duplex communication.

## Answer the following question in detail.

### 1. Differentiate between LAN and PAN.

**Local Area Network (LAN):**
- **Coverage Area:** Small geographical area like buildings or offices
- **Range:** Up to a few kilometers
- **Devices:** Computers, servers, printers, switches
- **Technology:** Ethernet cables, switches, routers
- **Speed:** High data transfer rates (10 Mbps to 10 Gbps)
- **Cost:** Higher infrastructure costs
- **Management:** Requires technical expertise
- **Purpose:** Business and organizational networking

**Personal Area Network (PAN):**
- **Coverage Area:** Individual person's workspace
- **Range:** Up to 10 meters (30 feet)
- **Devices:** Smartphones, tablets, laptops, wearables
- **Technology:** Bluetooth, infrared, USB
- **Speed:** Lower data transfer rates
- **Cost:** Low cost for personal use
- **Management:** Easy setup and configuration
- **Purpose:** Personal device connectivity

### 2. Differentiate between IP address and MAC address.

**IP Address:**
- **Type:** Logical address assigned by network administrator or DHCP
- **Length:** 32 bits (IPv4) or 128 bits (IPv6)
- **Format:** Dotted decimal notation (IPv4) or hexadecimal (IPv6)
- **Scope:** Used for routing between different networks
- **Changeability:** Can be changed or reassigned
- **Layer:** Network Layer (Layer 3)
- **Example:** 192.168.1.100

**MAC Address:**
- **Type:** Physical address permanently assigned by manufacturer
- **Length:** 48 bits (6 bytes)
- **Format:** Hexadecimal notation with colons or hyphens
- **Scope:** Used for local network communication
- **Changeability:** Cannot be changed (hardware-based)
- **Layer:** Data Link Layer (Layer 2)
- **Example:** 00:1B:44:11:3A:B7

### 3. Differentiate between IPv6 and IPv4.

**IPv4:**
- **Address Length:** 32 bits
- **Address Space:** 4.3 billion addresses
- **Format:** Dotted decimal notation (xxx.xxx.xxx.xxx)
- **Header Size:** 20-60 bytes (variable)
- **Security:** Security features added through IPSec
- **Configuration:** Manual or DHCP configuration required
- **NAT:** Network Address Translation required for internet access
- **Example:** 192.168.1.1

**IPv6:**
- **Address Length:** 128 bits
- **Address Space:** 340 undecillion addresses
- **Format:** Hexadecimal notation with colons
- **Header Size:** 40 bytes (fixed)
- **Security:** Built-in security features
- **Configuration:** Auto-configuration capabilities
- **NAT:** No need for NAT due to large address space
- **Example:** 2001:0db8:85a3:0000:0000:8a2e:0370:7334

### 4. Describe network topologies.

**Point-to-Point Topology:**
- Direct connection between two devices
- Maximum bandwidth utilization
- High reliability but limited scalability
- Used for backup connections and dedicated links

**Bus Topology:**
- All devices connected to single central cable
- Cost-effective and simple installation
- Single point of failure at the main cable
- Performance degrades with more devices

**Star Topology:**
- All devices connected to central hub or switch
- Easy installation and fault isolation
- Central device is single point of failure
- Most common topology in modern networks

**Ring Topology:**
- Devices connected in circular loop
- Equal access for all devices
- Failure of any device affects entire network
- Used in Token Ring and FDDI networks

**Mesh Topology:**
- Multiple connections between devices
- Highest fault tolerance and performance
- Expensive and complex to implement
- Used in critical business networks

### 5. Describe DHCP mode.

**Dynamic Host Configuration Protocol (DHCP)** automatically assigns IP addresses and network configuration to devices on a network.

**DHCP Process:**
1. **DHCP Discover:** Client broadcasts request for IP address
2. **DHCP Offer:** Server responds with available IP address offer
3. **DHCP Request:** Client requests the offered IP address
4. **DHCP Acknowledge:** Server confirms address assignment

**Key Features:**
- **Automatic Configuration:** Eliminates manual IP assignment
- **Lease Management:** Addresses assigned for specific time periods
- **Address Pool:** Manages available IP addresses efficiently
- **Configuration Options:** Provides subnet mask, gateway, DNS servers

**Advantages:**
- Reduces administrative overhead
- Prevents IP address conflicts
- Efficient use of address space
- Easy network management

**Components:**
- **DHCP Server:** Manages IP address assignment
- **DHCP Client:** Requests IP configuration
- **DHCP Relay:** Forwards DHCP messages across subnets
- **Address Pool:** Range of available IP addresses

## Practical Tasks

### 1. Assign static IP addresses to the computers in the computer lab.

**Steps to assign static IP addresses:**

**For Windows:**
1. Open Control Panel → Network and Internet → Network Connections
2. Right-click on the network adapter and select Properties
3. Select Internet Protocol Version 4 (TCP/IPv4) and click Properties
4. Select "Use the following IP address"
5. Enter the IP address, subnet mask, and default gateway
6. Enter DNS server addresses if required
7. Click OK to save settings

**For Linux:**
1. Edit network configuration file: `/etc/network/interfaces`
2. Add configuration:
   ```
   auto eth0
   iface eth0 inet static
   address 192.168.1.100
   netmask 255.255.255.0
   gateway 192.168.1.1
   dns-nameservers 8.8.8.8 8.8.4.4
   ```
3. Restart network service: `sudo systemctl restart networking`

**Example IP Configuration for Lab:**
- Network: 192.168.1.0/24
- Computer 1: 192.168.1.10
- Computer 2: 192.168.1.11
- Computer 3: 192.168.1.12
- Gateway: 192.168.1.1
- DNS: 8.8.8.8, 8.8.4.4

### 2. Perform Ping test to check the Internet connectivity of your computer.

**Steps to perform ping test:**

**Basic Connectivity Test:**
```bash
ping 8.8.8.8
```
This tests connectivity to Google's public DNS server.

**Domain Name Test:**
```bash
ping google.com
```
This tests both connectivity and DNS resolution.

**Local Network Test:**
```bash
ping 192.168.1.1
```
This tests connectivity to the default gateway.

**Interpreting Results:**
- **Success:** Shows "Reply from" messages with response time
- **Failure:** Shows "Request timeout" or "Destination unreachable"
- **DNS Issues:** IP ping works but domain ping fails

**Example Output:**
```
C:\>ping google.com
Pinging google.com [172.217.164.110] with 32 bytes of data:
Reply from 172.217.164.110: bytes=32 time=45ms TTL=54
Reply from 172.217.164.110: bytes=32 time=44ms TTL=54
Reply from 172.217.164.110: bytes=32 time=46ms TTL=54

Ping statistics for 172.217.164.110:
    Packets: Sent = 3, Received = 3, Lost = 0 (0% loss),
Approximate round-trip times in milli-seconds:
    Minimum = 44ms, Maximum = 46ms, Average = 45ms
```

**Troubleshooting Steps:**
1. Check physical connections
2. Verify IP configuration
3. Test local network connectivity
4. Check firewall settings
5. Contact network administrator if issues persist
