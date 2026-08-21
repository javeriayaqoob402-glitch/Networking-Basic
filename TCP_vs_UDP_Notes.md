# TCP vs UDP

## TCP (Transmission Control Protocol)

TCP is a **connection-oriented** and **reliable** protocol.

### Main Points
- TCP sends data in the correct order using **sequence numbers**.
- If a packet is lost, TCP can **retransmit** it.
- TCP uses **acknowledgments (ACKs)** to confirm received data.
- TCP establishes a connection using a **3-way handshake**:
  1. SYN
  2. SYN-ACK
  3. ACK
- TCP is generally slower than UDP because it provides reliability and uses more control mechanisms.

## UDP (User Datagram Protocol)

UDP is a **connectionless** protocol.

### Main Points
- UDP does **not** perform a 3-way handshake.
- UDP sends data quickly with less overhead.
- UDP does **not guarantee delivery**.
- If a packet is lost, UDP does not automatically retransmit it.
- UDP is generally faster than TCP.

## TCP vs UDP

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Reliable | No delivery guarantee |
| Handshake | 3-way handshake | No handshake |
| Packet Loss | Retransmission | No automatic retransmission |
| Ordering | Maintains order | No guarantee of order |
| Speed | Generally slower | Generally faster |
| Example Uses | Web, email, file transfer | Streaming, DNS, online gaming, VoIP |

## Simple Example

**TCP:**  
If a packet is lost, TCP detects the missing data and retransmits it.

**UDP:**  
If a packet is lost, UDP normally continues sending the next data without automatically retransmitting the lost packet.

## Easy Way to Remember

**TCP = Reliable + Ordered + Connection**

**UDP = Fast + Connectionless + No Delivery Guarantee**

---
Prepared for GitHub learning notes.
