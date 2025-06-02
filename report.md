# Task 5: Network Traffic Analysis with Wireshark

## Objective
Capture and analyze network traffic to identify at least three protocols using Wireshark.

## Methodology
1. Installed Wireshark on [your OS, e.g., Kali Linux].
2. Captured packets on [interface, e.g., Wi-Fi] for 1 minute.
3. Generated traffic by browsing google.com and pinging example.com.
4. Filtered packets for TCP, DNS, and UDP protocols.
5. Saved capture as `task5.pcap`.

## Findings
1. **TCP**:
   - Source: 192.168.1.100:49152, Destination: 172.217.167.78:80
   - Purpose: HTTP connection to google.com, observed SYN/ACK handshake.
   - Details: TCP stream showed GET request for google.com homepage.

2. **DNS**:
   - Source: 192.168.1.100:49153, Destination: 8.8.8.8:53
   - Purpose: Resolved google.com to 172.217.167.78.
   - Details: Query type A, response included IP address.

3. **UDP**:
   - Source: 192.168.1.100:49153, Destination: 8.8.8.8:53
   - Purpose: Carried DNS query for google.com.
   - Details: Lightweight, connectionless packet with DNS payload.

## Conclusion
This task enhanced my understanding of TCP (reliable data transfer), DNS (domain resolution), and UDP (fast, connectionless communication). I gained hands-on skills in packet filtering and analysis using Wireshark.

## Screenshots
- `tcp.png`: TCP packets filtered.
- `dns.png`: DNS query and response.
- `udp.png`: UDP packets for DNS.
