# Module 2 — Network Foundations

## What This Module Covers
Core networking concepts that underpin all cybersecurity
work. Understanding networks is essential for detecting
and investigating security incidents.

## What I Learned

### OSI Model — 7 Layers
| Layer | Name | What It Does |
|---|---|---|
| 7 | Application | User-facing apps (HTTP, FTP, DNS) |
| 6 | Presentation | Encryption, compression, formatting |
| 5 | Session | Manages connections between apps |
| 4 | Transport | TCP/UDP, ports, reliability |
| 3 | Network | IP addressing, routing |
| 2 | Data Link | MAC addresses, switches |
| 1 | Physical | Cables, signals, hardware |

### TCP/IP Model — 4 La
yers
| Layer | Covers |
|---|---|
| Application | HTTP, DNS, FTP, SMTP |
| Transport | TCP, UDP, ports |
| Internet | IP addressing, routing |
| Network Access | Physical transmission |

### TCP Three-Way Handshake
Client → SYN → Server
Client ← SYN-ACK ← Server
Client → ACK → Server
Connection established

### Key Ports
| Port | Service |
|---|---|
| 22 | SSH |
| 23 | Telnet |
| 80 | HTTP |
| 443 | HTTPS |
| 445 | SMB |
| 3389 | RDP |

### IP Addressing
- IPv4 format: 192.168.1.1
- Subnet mask: 255.255.255.0
- CIDR notation: 192.168.1.0/24
- Private ranges: 10.x.x.x, 172.16.x.x, 192.168.x.x

## Key Takeaway
Network knowledge is used in every security investigation.
Every attack travels through a network — understanding how
is what allows you to detect and trace it.

## Date Completed
August 2026
