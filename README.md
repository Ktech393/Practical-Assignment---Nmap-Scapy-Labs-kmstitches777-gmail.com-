# Practical-Assignment---Nmap-Scapy-Labs-kmstitches777-gmail.com-
Over the past week, I had the opportunity to reproduce lab exercises using Nmap and Scapy, gaining hands-on experience in network reconnaissance and packet-level analysis.
Objectives
Reproduce all network scanning techniques demonstrated in class
Practice safe host discovery, port scanning, service detection, and OS fingerprinting
Learn packet crafting, sending, sniffing, and analysis using Scapy
Document methodology, commands used, and results
Environment Setup
Operating System: (Kali, Ubuntu, Windows Subsystem for Linux, etc.)
-------------------------------------------------------------------
Tools:
Nmap
Scapy (Python3)
Network: Classroom / Lab VM environment only
Nmap
-Host Discovery
-Port Scanning
-Service Detection
-OS Fingerprinting
-Basic NSE Scripts
Scapy
-Packet Crafting
-Packet Sending
-Packet Sniffing
-Basic Protocol Analysis

---------------------------------------------------------------------
Results Summary During this lab, I successfully reproduced all Nmap and Scapy exercises demonstrated in class within a controlled, authorized network environment
Nmap Results Summary

1. Host Discovery
Successfully identified active hosts on the lab subnet using -sn.
Observed differences between ARP-based discovery (on local networks) and ICMP-based discovery (on remote networks).

2. Port Scanning
Identified open, closed, and filtered ports using SYN scans (-sS) and TCP Connect scans (-sT).
Compared behavior when scanning:
TCP vs UDP ports
Single targets vs entire subnets
Noted the impact of firewall rules on port visibility.

3. Service Detection
Used -sV to detect running services such as SSH, HTTP, and database services.
Observed accurate version detection when services returned banners.
Learned how different version intensities affect scan speed and accuracy.

4. OS Fingerprinting
Applied OS detection with -O and -A.
Nmap was able to identify general OS families (Linux/Windows) based on TCP/IP fingerprinting.
Understood conditions for accurate OS detection:
At least one open and one closed port
Unfiltered responses from the target

5. Basic Nmap Scripting (NSE)
Executed default safe scripts for additional information.
Observed script outputs such as:
HTTP metadata
SSH host keys
Basic security checks

Scapy Results Summary
1. Packet Crafting
Successfully crafted packets for IP, TCP, ICMP, ARP, and DNS layers.
Used show() and ls() to inspect fields and understand protocol structure.

2. Packet Sending
Sent test packets within the lab environment using send() (Layer 3) and sendp() (Layer 2).
Observed how Scapy automatically fills certain header values (TTL, checksums, sequence numbers).

3. Packet Sniffing
Captured live traffic using sniff().
Applied filters (TCP, ICMP, ARP) to observe specific protocol activity.
Used summary() and show() to examine captured packets.

4. Basic Protocol Analysis
Extracted protocol fields (src/dst IP, ports, flags).
Analyzed packet flows and relationships between protocol layers.

----------------------------------------------------------------------
Overall Learning Outcomes
Strengthened understanding of network reconnaissance fundamentals.
Gained hands-on experience with Nmap's scanning techniques and output interpretation.
Learned how to build, inspect, send, and analyze packets programmatically using Scapy.
Improved ability to document cybersecurity workflows professionally using GitHub Markdown.
