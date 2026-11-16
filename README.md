# Network Traffic Analysis Lab

## Overview

This project demonstrates practical network traffic analysis using Wireshark and tcpdump in a controlled VirtualBox laboratory environment.

The lab involved capturing and inspecting network packets to understand how devices communicate, how common network protocols operate, and how packet analysis supports network troubleshooting and cybersecurity investigations.

## Lab Environment

The laboratory consisted of two virtual machines:

- **Kali Linux** — used for packet capture and network analysis.
- **Ubuntu Server** — used as the communication endpoint.

### Network Configuration

| Machine | Host-Only IP Address |
|---|---|
| Kali Linux | 192.168.56.102 |
| Ubuntu Server | 192.168.56.101 |

**Wireshark version:** 4.6.6

## Objectives

- Capture and analyse network traffic.
- Understand ICMP (Internet Control Message Protocol) communication.
- Inspect DNS (Domain Name System) queries and responses.
- Identify the TCP (Transmission Control Protocol) three-way handshake.
- Examine HTTP (Hypertext Transfer Protocol) requests and responses.
- Use tcpdump for command-line packet capture.
- Understand how packet analysis supports network monitoring and troubleshooting.

## Tools Used

- Kali Linux
- Ubuntu Server
- Oracle VirtualBox
- Wireshark
- tcpdump
- ping
- nslookup

## Practical Activities

### 1. ICMP Packet Analysis

Generated ICMP traffic using `ping` to examine communication between Kali Linux and Ubuntu Server.

Observed:
- ICMP Echo Request packets (Type 8, Code 0).
- ICMP Echo Reply packets (Type 0, Code 0).

### 2. DNS Traffic Analysis

Used `nslookup` to generate DNS queries and inspect how domain names are resolved into IP addresses.

Examined DNS query and response packets.

### 3. TCP Three-Way Handshake

Inspected the TCP connection establishment process:

1. **SYN** — client requests a connection.
2. **SYN-ACK** — server acknowledges the request.
3. **ACK** — client confirms the connection.

### 4. HTTP Request and Response Analysis

Examined HTTP communication to understand how a client sends requests and receives responses from a web server.

### 5. Command-Line Packet Capture

Used `tcpdump` to capture and inspect network traffic from the terminal.

This demonstrated an alternative to graphical packet analysis with Wireshark.

## Wireshark Display Filters

| Filter | Purpose |
|---|---|
| `icmp` | Display ICMP packets |
| `dns` | Display DNS traffic |
| `tcp` | Display TCP packets |
| `tcp.port == 80` | Display TCP traffic using port 80 |
| `http` | Display HTTP traffic where the protocol is recognised |

## Key Learning Outcomes

- Understanding packet capture and inspection.
- Recognising common network protocols.
- Analysing DNS resolution.
- Understanding TCP connection establishment.
- Inspecting HTTP communication.
- Using Wireshark display filters.
- Performing command-line packet capture with tcpdump.

## Evidence

Screenshots documenting the practical activities are provided in this repository.

The original packet capture file (`.pcapng`) can also be included to allow further inspection of the captured traffic.

## Conclusion

This project provided practical experience in network traffic analysis and protocol inspection. It strengthened my understanding of how network communication works and how tools such as Wireshark and tcpdump can be used for troubleshooting, monitoring, and cybersecurity investigations.

All activities were conducted within my controlled virtual laboratory environment.
