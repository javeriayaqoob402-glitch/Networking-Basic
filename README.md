# Networking-Basic
Networking is simply connecting two or more devices (like your phone, computer, or TV) together so they can talk to each other and share things.
**Example:**
Think of networking like a postal system:
Devices (computers, phones) are like houses.
Data (photos, messages, videos) are like letters.
Routers & Cables are like post offices and roads that deliver the letters to the right house.
**Difference between IP Address and MAC Address?**
An IP address identifies a device's location on a network logically and changes based on where you connect, while a MAC address is a permanent, physical identifier burned directly into your device's network hardware.
**Feature:**
IP Address (Logical)	MAC Address (Physical)
Purpose	Routes data across different networks (e.g., across the internet)	Identifies your device on the immediate local network (LAN)
Changeability	Dynamic — changes whenever you join a new Wi-Fi or router	Static — permanently assigned by the hardware manufacturer
Layer (OSI)	Network Layer (Layer 3)	Data Link Layer (Layer 2)
Format	IPv4 (192.168.1.1) or IPv6 (2001:db8::1)	12-digit Hexadecimal (00:1A:2B:3C:4D:5E)
Analogy	Your mailing address (changes when you move homes)	Your fingerprint or ID number (never changes)
**How They Work Together**
When sending data across a network:
The IP address guides data from the sender's network all the way across the internet to the destination network.
The MAC address ensures that once the data reaches the correct destination router, it gets delivered to your specific device rather than another device on the same local Wi-fi.
**what is loop back?**
**Loopback** (or a loopback address) is a virtual network interface that a computer uses to send network traffic back to itself.
It allows your device to talk to itself over network protocols without sending any data out to the physical network or internet.
**Key Concepts**
IP Address: The standard loopback IP address is 127.0.0.1 (IPv4) or ::1 (IPv6).
Hostname: It is commonly referred to by the domain name localhost.
Traffic Routing: When a program sends data to 127.0.0.1, the network hardware bypasses the physical network card (NIC) and routes the traffic directly back into the local operating system.
**TTL and traceroute**
TTL (Time to Live) and Traceroute are network tools used to track the path data takes across the internet and prevent network loops.
**Key Concepts**
**TTL (Time to Live):** A numerical limit (hop count) set inside a data packet. Every time the packet passes through a router (a "hop"), the TTL value decreases by 1. If TTL reaches 0, the router drops the packet and sends a Time Exceeded message back to you. This prevents lost packets from traveling endlessly around the network.

**Traceroute:** A diagnostic tool that maps the exact route data travels from your computer to a destination IP/website. It works by deliberately sending packets with increasing TTL values (TTL=1, TTL=2, TTL=3...) to identify every router along the way.
**COMMANDS**
traceroute 8.8.8.8
**ttl**
TTL (Time to Live) is a counter or time limit embedded inside a data packet that tells it how long to exist before being discarded.
**Difference between curl and wget?**
CURL and wget are both command-line tools used to download content from servers, but they serve different purposes depending on what you are trying to do.
**Command Examples**
wget: wget [https://example.com/file.zip](https://example.com/file.zip)
curl: curl -O [https://example.com/file.zip](https://example.com/file.zip)



