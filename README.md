Network Traffic Capture and Analysis Using Wireshark
====================================================

Overview
--------
This project involves capturing live network traffic on Kali Linux using Wireshark, identifying different network protocols, and analyzing the captured data.

Tools Used
----------
- Kali Linux
- Wireshark (version 4.4.6)

Steps to Reproduce
------------------
1. Install Wireshark (if not installed):
   sudo apt update
   sudo apt install wireshark

2. Launch Wireshark with root privileges to avoid permission issues:
   sudo wireshark

3. Select the active network interface connected to the internet (e.g., wlan0 for Wi-Fi).

4. Start capturing packets by clicking the interface in Wireshark.

5. Generate network traffic by:
   - Pinging a server in the terminal:
     ping -c 5 google.com
   - Or browsing a website in a browser.

6. Stop the capture after about 1 minute or sufficient packets are captured.

7. Filter captured packets by protocol using the filter bar:
   - icmp for ping packets
   - dns for domain lookups
   - tcp for connection-oriented traffic
   - http for web traffic

8. Save the capture as a .pcap file via File > Save As.

Protocols Identified
--------------------
- ICMP (Internet Control Message Protocol)
- DNS (Domain Name System)
- TCP (Transmission Control Protocol)

Summary
-------
This capture and analysis exercise helped in understanding basic network communication protocols and how to use Wireshark for packet analysis.

Files Included
--------------
- capture.pcap — The packet capture file generated during the task.
- report.docx or report.pdf — The detailed report summarizing the findings.
