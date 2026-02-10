Project 3 – Baseline Pattern Identification
Baseline Pattern Identification Using Wireshark
Objective
To observe and analyze normal network traffic patterns over time using Wireshark, and establish baselines that can later be used to identify abnormal or suspicious network behavior.
Environment
Operating System: macOS
Tool: Wireshark
Network Interface: Wi-Fi (en0)
Method
Captured live network traffic using Wireshark
Created three separate 10-minute packet captures at different times of day:
Morning
Afternoon
Night
Analyzed each capture using:
Protocol Hierarchy
IPv4 Conversations
I/O Graphs
Compared traffic volume, protocol usage, and communication patterns across baselines
Baselines Captured
Baseline	Time of Day	File
A	Morning	P3-baseline-A-morning.pcapng
B	Afternoon	P3-baseline-B-afternoon.pcapng
C	Night	P3-baseline-C-night.pcapng
All captures were collected on the same system and network to maintain consistency.
Findings
Common protocols such as TCP, TLS, and QUIC were consistently observed across all baselines
Traffic volume varied depending on time of day:
Afternoon showed higher overall activity
Night showed reduced traffic and fewer spikes
IPv4 conversations revealed recurring destination IPs, indicating normal background services and web traffic
No unexpected protocols or abnormal traffic patterns were identified
These findings represent normal, healthy network behavior for this environment.
Conclusion
This project demonstrates how network baselines can be established and compared to understand typical traffic behavior.
Baseline analysis is a foundational cybersecurity skill, as deviations from normal patterns are often the first indicators of malicious activity.

