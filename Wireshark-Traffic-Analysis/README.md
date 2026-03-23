# 🕸️ Project: Network Traffic Analysis & Port Scan Detection

## Objective
[cite_start]The goal of this project was to prove I understand what a hack looks like "on the wire"[cite: 16, 17]. By simulating a port scan using Nmap and analyzing the traffic with Wireshark, I identified the specific network patterns associated with reconnaissance activities.

## Skills Demonstrated
- Capturing live network traffic on local interfaces.
- Applying Wireshark display filters to isolate specific TCP flags (SYN/ACK).
- Understanding the TCP 3-way handshake and how it is manipulated during a stealth scan.
- Identifying an attacker's IP address and the specific ports targeted during reconnaissance.

## Tools Used
- [cite_start]**Wireshark** (Network Protocol Analyzer) [cite: 18]
- [cite_start]**Nmap** (Network Mapper / Attacking Tool) [cite: 18]

## Steps Taken
1. Initiated a live packet capture on the local loopback adapter using Wireshark.
2. [cite_start]Executed a stealth SYN scan (`nmap -sS`) against the local machine's IP address using Nmap[cite: 19].
3. [cite_start]Stopped the packet capture and applied the display filter `tcp.flags.syn == 1 and tcp.flags.ack == 0` to isolate the scanner's initial connection requests[cite: 20].
4. [cite_start]Analyzed the captured PCAP data to pinpoint the origin of the scan and document the targeted ports[cite: 22].

## Evidence
*(Drag and drop your Wireshark screenshot here)*
