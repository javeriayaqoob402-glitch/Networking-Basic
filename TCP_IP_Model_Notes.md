# TCP/IP Model

## What is TCP/IP Model?

TCP/IP (Transmission Control Protocol/Internet Protocol) is a networking model used for communication between devices over a network and the Internet.

It has **4 layers**:
1. Application Layer
2. Transport Layer
3. Internet Layer
4. Network Access Layer

---

## 1. Application Layer

User applications ke network communication ko handle karti hai.

**Common protocols:**
- HTTP / HTTPS
- DNS
- FTP
- SMTP
- SSH

**Example:** Browser se website request bhejna.

**Data Unit:** Data

---

## 2. Transport Layer

End-to-end communication provide karti hai.

- TCP reliable communication provide karta hai.
- UDP fast but connectionless communication provide karta hai.
- Source aur destination port numbers use hote hain.
- TCP data ko segments mein divide karta hai.

**Examples:**
- TCP
- UDP

**Data Unit:** Segment / Datagram

---

## 3. Internet Layer

Devices ko logical addressing provide karti hai.

- Source IP address aur Destination IP address use hote hain.
- Routers packets ko destination ki taraf forward karte hain.
- Routing isi layer ka important function hai.

**Examples:**
- IPv4
- IPv6
- ICMP

**Data Unit:** Packet

---

## 4. Network Access Layer

Local network par data transmission handle karti hai.

- MAC addresses use hote hain.
- Data ko frames aur physical signals mein transmit kiya jata hai.

**Examples:**
- Ethernet
- Wi-Fi
- ARP

**Data Unit:** Frame / Bits

---

## TCP/IP Encapsulation

```
Application
    ↓
   Data
    ↓
Transport
    ↓
 Segment
    ↓
Internet
    ↓
 Packet
    ↓
Network Access
    ↓
 Frame → Bits
```

---

## Simple Example

Jab user browser mein website open karta hai:

1. **Application Layer** — HTTP/HTTPS request create karti hai.
2. **Transport Layer** — TCP ports aur reliability information add karta hai.
3. **Internet Layer** — source aur destination IP addresses add karti hai.
4. **Network Access Layer** — local delivery ke liye MAC addresses/frame information handle karti hai.
5. Data network medium ke through transmit hota hai.

---

## TCP/IP vs OSI

| TCP/IP | OSI Equivalent |
|---|---|
| Application | Application + Presentation + Session |
| Transport | Transport |
| Internet | Network |
| Network Access | Data Link + Physical |

---

## Quick Revision

**Application → Transport → Internet → Network Access**

**Data → Segment → Packet → Frame → Bits**

---

## Key Points

- Port Number → Transport Layer
- IP Address → Internet Layer
- MAC Address → Network Access Layer
- Routing → Internet Layer
- TCP/UDP → Transport Layer
- HTTP/HTTPS/DNS/SSH → Application Layer
