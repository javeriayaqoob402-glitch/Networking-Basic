# Networking Basics

Beginner notes for Cyber Security / SOC Analyst learning.

## 1. Network
A network is a group of connected devices that communicate and share data or resources.

Examples: computers, phones, servers, printers, routers, and switches.

## 2. Wired Network
A wired network uses a physical Ethernet/network cable.

**Example:** Computer → Ethernet Cable → Switch → Router

**Benefits:** stable, reliable, and usually less affected by wireless interference.

## 3. Wireless Network
A wireless network connects devices using Wi-Fi/radio signals instead of a physical cable.

**Example:** Laptop → Wi-Fi → Router

**Benefits:** convenient and supports mobile devices.

### Wired vs Wireless

| Wired | Wireless |
|---|---|
| Uses cable | Uses Wi-Fi/radio |
| Usually more stable | More convenient |
| Good for fixed devices | Good for mobile devices |

## 4. Public Network
A public network is a less-trusted network, such as Wi-Fi at an airport, cafe, or hotel.

**Security:** Avoid unnecessary sensitive activity on untrusted networks and keep security settings enabled.

## 5. Private Network
A private network is a controlled/trusted network used at places such as homes, offices, and organizations.

**Example:** Home Wi-Fi connecting a laptop, phone, and smart TV.

### Public vs Private

| Public | Private |
|---|---|
| Less trusted | More controlled/trusted |
| Often shared | Usually limited to authorized users |
| Higher security risk | Easier to secure |

## 6. DHCP
**DHCP = Dynamic Host Configuration Protocol**

DHCP automatically provides network settings to a device, such as:
- IP address
- Subnet mask
- Default gateway
- DNS server

**Easy:** DHCP = automatic network configuration.

## 7. Manual / Static IP
A manual/static IP is configured by entering the network settings yourself.

Typical settings:
- IP address
- Subnet mask
- Default gateway
- DNS server

**Example:** `192.168.1.50`

Static IPs are useful when a device needs a predictable address, such as a server.

### DHCP vs Manual

| DHCP | Manual / Static |
|---|---|
| Automatic | Manually configured |
| Easy for normal devices | Useful when a fixed address is needed |
| Address may change | Address normally stays fixed |

## 8. Hub
A **hub** is a basic networking device that sends incoming data to all connected ports.

**Easy:** Hub = sends traffic to all ports.

Hubs are mostly outdated and have largely been replaced by switches.

## 9. Switch
A **switch** connects devices in a local network and forwards Ethernet frames toward the appropriate port using MAC addresses.

**Easy:** Switch = forwards traffic using MAC addresses.

### Hub vs Switch

| Hub | Switch |
|---|---|
| Sends traffic to all ports | Forwards to the appropriate port |
| Less efficient | More efficient |
| Basic/outdated | Commonly used today |
| No MAC-based forwarding table | Uses a MAC address table |

## 10. Useful Kali Linux Commands

Check IP addresses and interfaces:
```bash
ip address
```

Check the routing table:
```bash
ip route
```

Test connectivity:
```bash
ping 8.8.8.8
```

Show network interfaces:
```bash
ip link
```

## Quick Revision

- **Network** → connected devices that communicate
- **Wired** → uses a network cable
- **Wireless** → uses Wi-Fi/radio
- **Public** → less-trusted network
- **Private** → controlled/trusted network
- **DHCP** → automatically assigns network settings
- **Manual/Static IP** → settings entered manually
- **Hub** → sends traffic to all ports
- **Switch** → forwards traffic based on MAC addresses

## Conclusion
These are basic networking concepts that are important for Cyber Security and SOC Analyst learning. They provide a foundation for later topics such as DNS, routing, packet analysis, and network security.
