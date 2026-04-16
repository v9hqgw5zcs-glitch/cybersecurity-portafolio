🔍 Lab 1 – Network Discovery & SYN Scan

📌 Objective

To perform network reconnaissance by identifying active hosts and analyzing port states using Nmap.


🛠 Tools & Environment
	•	Kali Linux (VirtualBox)
	•	Nmap


🌐 Network Information
	•	Local IP Address: 10.0.2.15
	•	Network Range: 10.0.2.0/24
	•	Environment: VirtualBox NAT network


Methodology

1. Identify Local IP

Code: ip a

2. Discover Active Hosts

Code: nmap -sn 10.0.2.0/24

3. Perform SYN Scan

nmap -sS 10.0.2.2

📊 Results
	•	4 active hosts discovered
	•	Target host responded with:
	•	Filtered ports (likely firewall presence)
	•	Closed ports
	•	No open services detected

🧠 Analysis

The scan results indicate that the target system is either protected by firewall rules or operating within a restricted NAT environment.

Filtered ports suggest that packets are being blocked or dropped, preventing full visibility into available services.

📚 Key Takeaways
	•	Learned how to identify network ranges
	•	Understood host discovery techniques
	•	Gained experience with SYN (stealth) scanning
	•	Interpreted filtered vs closed port responses

⚠️ Disclaimer

This lab was conducted in a controlled environment for educational purposes only.
