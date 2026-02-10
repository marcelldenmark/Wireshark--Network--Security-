Project 3: Baseline Pattern Identification (Wireshark)
Objective
The goal of this project is to establish normal network traffic patterns (baselines) and compare how traffic changes over time.
Understanding what “normal” looks like is critical in cybersecurity because you cannot detect abnormal or malicious activity without a baseline.
In this project, I captured and analyzed network traffic at three different times of day using Wireshark on macOS.
What Is a Network Baseline?
A network baseline is a snapshot of normal network behavior, including:
Common protocols in use
Typical traffic volume
Frequent source and destination IPs
Normal traffic spikes and quiet periods
Security teams use baselines to:
Detect anomalies
Identify suspicious spikes or drops
Spot unexpected protocols or connections
Baselines Collected
Three 10-minute captures were collected under normal usage conditions:
Baseline	Time of Day	File
A	Morning	P3-baseline-A-morning.pcapng
B	Afternoon	P3-baseline-B-afternoon.pcapng
C	Night	P3-baseline-C-night.pcapng
All captures were taken on the same machine and network to ensure consistency.
Tools Used
Wireshark
macOS
Wi-Fi interface (en0)
Analysis Performed
For each baseline, the following analyses were completed:
1. Protocol Hierarchy
Shows the breakdown of network protocols (e.g., TCP, UDP, TLS, QUIC).
This helps identify which protocols dominate normal traffic.
Screenshots:
P3-04-protocol-hierarchy-A.png
P3-04-protocol-hierarchy-B.png
P3-04-protocol-hierarchy-C.png
2. Conversations (IPv4)
Displays the most active see which systems communicate the most and how much data is exchanged.
Screenshots:
P3-05-conversations-ipv4-A.png
P3-05-conversations-ipv4-B.png
P3-05-conversations-ipv4-C.png
3. I/O Graphs
Visualizes traffic volume over time.
This helps identify:
Normal traffic spikes
Periods of inactivity
Differences between times of day
Screenshots:
P3-09-io-graph-A.png
P3-09-io-graph-B.png
P3-09-io-graph-C.png
Key Observations
Traffic volume and spikes varied by time of day
Common protocols (TLS/QUIC) remained consistent across baselines
Afternoon traffic showed higher activity compared to night
No unexpected protocols or abnormal traffic patterns were observed
These results indicate normal, healthy network behavior for this environment.
Why This Matters in Cybersecurity
In real-world security operations:
Baselines are used to detect malware, data exfiltration, and intrusions
Sudden deviations from baseline behavior trigger investigations
SOC analysts rely on tools like Wireshark to validate alerts
This project demonstrates:
Understanding of packet capture
Ability to analyze traffic trends
Foundational skills required for SOC and network security roles
