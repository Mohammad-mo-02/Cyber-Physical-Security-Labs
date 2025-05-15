 Cyber Physical Systems (CPS) Security Labs ⚙️  
[![Academic Project](https://img.shields.io/badge/MSc%20Project-CPS%20Security-orange)](https://github.com/Mohammad-mo-02)

This repository documents the security hardening of a simulated **Cyber-Physical System (CPS)** environment. Key areas include SSH brute-force mitigation, firewall configuration, VPN deployment, Snort intrusion detection, and protocol exploit analysis using Wireshark.

---

📁 Included File

| File | Description |
|------|-------------|
| `Attack-Simulation-CPS.pdf` | Full report with screenshots of SSH mitigation, Snort IDS, firewall routing, OpenVPN setup, and EternalBlue detection. |

---

🔐 Security Techniques Demonstrated

- Brute force SSH attack simulation and blocking via `sshguard`
- Public/private key authentication and config hardening
- `iptables` firewall with NAT masquerading & IP forwarding
- OpenVPN tunnel setup with Easy-RSA certs and TLS handshake
- Wireshark EternalBlue (CVE-2017-0144) detection using protocol filters
- Snort IDS traffic logging & alert rules (HTTP, ICMP, SSH)
- VLAN segmentation & access policy discussion

---

 🧠 Key Tools Used

- 🔐 **OpenSSH / sshguard**
- 🌐 **iptables**
- 🔒 **OpenVPN**
- 🔍 **Wireshark**
- 🚨 **Snort IDS**
- 🧪 **Oracle VirtualBox** (Ubuntu & Debian simulation)

---

 🏁 Learning Outcomes

- Understood layered defence in CPS and IoT networks
- Built a firewall/router simulation with IP segmentation
- Detected protocol-level attacks (SMB exploits) using Wireshark
- Designed and tested SSH cryptographic login enforcement
- Configured IDS signatures for early threat detection
- Applied real-world DDoS and brute-force mitigation strategies

---

 🎓 Academic Context

> This lab project was completed for **COS7051-B: Cyber Physical Systems Security** during my MSc Cybersecurity at the University of Bradford.

📧 Contact: arsalanmahmood893@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/mohammad-mahmood-ba1a321ba)
