# 🌐 Networking Basics & Fundamentals

These notes cover the **core networking concepts required for CompTIA Security+ (SY0-701)**.  
Understanding networking fundamentals is essential because **security protects networks and the systems that communicate across them**.

---

# 📡 What is a Network?

A **network** is a collection of devices connected together to share:

- Data
- Resources
- Applications
- Internet access

Devices communicate using **protocols** (rules for communication).

Examples of networked devices:

- Computers
- Servers
- Smartphones
- Routers
- Switches
- Printers
- IoT devices

---

# 🧠 Key Networking Terms

| Term | Definition |
|-----|------------|
| Node | Any device connected to a network |
| Host | A device with an IP address |
| Packet | Small unit of data transmitted across a network |
| Protocol | Rules governing communication |
| Bandwidth | Maximum data transfer rate |
| Latency | Delay in data transmission |
| Throughput | Actual rate of successful data transfer |

---

# 📦 Data Transmission Concepts

### Packetization

Large data is divided into **packets** before transmission.

Each packet contains:

- Source address
- Destination address
- Payload (actual data)
- Control information

---

### Packet Flow Example

```
Client → Router → ISP → Internet → Server
```

Packets may take **different routes** to reach the destination.

---

# 🧱 The OSI Model

The **OSI (Open Systems Interconnection) Model** describes how network communication works.

It has **7 layers**.

| Layer | Name | Function |
|------|------|---------|
| 7 | Application | User-facing applications |
| 6 | Presentation | Data formatting & encryption |
| 5 | Session | Session management |
| 4 | Transport | End-to-end communication |
| 3 | Network | Routing packets |
| 2 | Data Link | MAC addressing |
| 1 | Physical | Physical transmission |

---

### Memory Trick

```
All People Seem To Need Data Processing
```

or

```
Please Do Not Throw Sausage Pizza Away
```

---

# 📡 TCP/IP Model

The **TCP/IP model** is the practical model used on the internet.

| Layer | Equivalent OSI Layers |
|------|----------------------|
| Application | OSI 5–7 |
| Transport | OSI 4 |
| Internet | OSI 3 |
| Network Access | OSI 1–2 |

---

# 🌍 IP Addressing

An **IP address** uniquely identifies a device on a network.

Two main versions:

| Version | Format |
|------|------|
| IPv4 | 192.168.1.1 |
| IPv6 | 2001:0db8::1 |

---

# 🔢 IPv4 Addressing

IPv4 uses **32-bit addresses**.

Example:

```
192.168.1.10
```

Range:

```
0.0.0.0 → 255.255.255.255
```

---

# 🏠 Private IP Ranges

Private IPs are used **inside internal networks**.

| Range | CIDR |
|------|------|
| 10.0.0.0 – 10.255.255.255 | /8 |
| 172.16.0.0 – 172.31.255.255 | /12 |
| 192.168.0.0 – 192.168.255.255 | /16 |

These addresses are **not routable on the public internet**.

---

# 🌍 Public IP Addresses

Public IPs are:

- Globally unique
- Assigned by ISPs
- Routable on the internet

---

# 🔀 Network Address Translation (NAT)

NAT allows **private networks to access the internet using one public IP**.

Example:

```
192.168.1.10 → 203.0.113.5
```

Types:

| NAT Type | Description |
|--------|-------------|
| Static NAT | One-to-one mapping |
| Dynamic NAT | Pool of public addresses |
| PAT (Port Address Translation) | Multiple devices share one IP |

PAT is most common.

---

# 🧮 Subnetting Basics

Subnetting divides a network into **smaller networks**.

Purpose:

- Improve performance
- Increase security
- Reduce broadcast traffic

Example:

```
192.168.1.0 /24
```

Subnet mask:

```
255.255.255.0
```

---

# 📶 MAC Addresses

A **MAC address** identifies a physical network interface.

Example:

```
00:1A:2B:3C:4D:5E
```

Characteristics:

- 48-bit identifier
- Assigned by manufacturer
- Used at **Layer 2**

---

# 🔁 ARP (Address Resolution Protocol)

ARP maps:

```
IP Address → MAC Address
```

Example:

```
Who has 192.168.1.10?
```

Device replies with its MAC address.

---

# 📡 Common Networking Protocols

| Protocol | Purpose |
|------|---------|
| HTTP | Web traffic |
| HTTPS | Secure web traffic |
| FTP | File transfer |
| SSH | Secure remote login |
| DNS | Domain resolution |
| DHCP | Automatic IP assignment |
| SMTP | Send email |
| POP3 | Retrieve email |
| IMAP | Email management |

---

# 🧠 Important Port Numbers

| Protocol | Port |
|--------|------|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| FTP | 21 |
| DNS | 53 |
| SMTP | 25 |
| RDP | 3389 |
| SNMP | 161 |

---

# 🧱 Networking Hardware

## Router

Connects **multiple networks together**.

Functions:

- Routing packets
- NAT
- Internet connectivity

---

## Switch

Connects devices **within a local network**.

Uses **MAC addresses** to forward traffic.

---

## Hub (Legacy)

Broadcasts traffic to **all devices**.

Not secure.

---

## Access Point

Provides **wireless connectivity**.

---

## Firewall

Filters network traffic based on **security rules**.

---

# 🌐 Network Types

| Network | Description |
|------|-------------|
| LAN | Local Area Network |
| WAN | Wide Area Network |
| MAN | Metropolitan Area Network |
| PAN | Personal Area Network |
| VLAN | Virtual LAN |

---

# 📶 Wireless Networking

Wireless networks use **radio signals**.

Common standards:

| Standard | Speed |
|------|------|
| 802.11n | Up to 600 Mbps |
| 802.11ac | Up to 1.3 Gbps |
| 802.11ax | WiFi 6 |

---

# 🔐 Wireless Security

| Protocol | Security |
|------|---------|
| WEP | Broken |
| WPA | Weak |
| WPA2 | Strong |
| WPA3 | Strongest |

---

# 📊 Network Topologies

Network layout structures.

| Topology | Description |
|--------|-------------|
| Star | Central switch |
| Bus | Shared backbone |
| Ring | Circular network |
| Mesh | Fully interconnected |

Star topology is most common today.

---

# 📡 DNS (Domain Name System)

DNS converts:

```
google.com → 142.250.190.78
```

This allows humans to use **domain names instead of IP addresses**.

---

# 🧾 DHCP (Dynamic Host Configuration Protocol)

Automatically assigns:

- IP address
- Subnet mask
- Gateway
- DNS server

DHCP process:

```
DORA
```

1. Discover  
2. Offer  
3. Request  
4. Acknowledge

---

# 🧪 Network Troubleshooting Tools

| Tool | Function |
|----|-----------|
| ping | Test connectivity |
| tracert | Show packet path |
| ipconfig | Display IP configuration |
| nslookup | DNS queries |
| netstat | Network connections |

---

# 🚨 Security Concepts in Networking

Key principles:

| Principle | Meaning |
|---------|--------|
| Least privilege | Minimal access |
| Defense in depth | Multiple security layers |
| Segmentation | Isolate networks |

---

# 🧠 Networking Summary

Key networking fundamentals:

✔ OSI & TCP/IP models  
✔ IPv4 vs IPv6  
✔ Subnetting basics  
✔ NAT and private IP ranges  
✔ Common protocols and ports  
✔ Network hardware  
✔ Wireless networking  

These fundamentals form the **foundation for all cybersecurity concepts**.

---

# 🎯 Study Tip

Security+ questions often describe **network scenarios**.

If you understand:

- how packets travel
- how IP addressing works
- how protocols communicate

…most security questions become **logical to solve**.