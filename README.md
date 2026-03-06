# Cyber-Physical Systems Security Labs

## Advanced Security Experimentation in Network Defence, Intrusion Detection, and Infrastructure Hardening

This repository documents a series of practical cybersecurity experiments conducted as part of my MSc Cybersecurity studies. The project focuses on the security challenges present within Cyber-Physical Systems (CPS), where digital networks interact with physical devices, industrial infrastructure, and remotely managed systems.

Cyber-physical environments introduce complex security risks due to the integration of embedded devices, remote connectivity, and distributed operational systems. Attackers frequently target these environments through credential attacks, network exploitation, and protocol vulnerabilities in order to gain unauthorised access or disrupt system availability.

This project investigates these threats through controlled laboratory experiments that simulate real-world attack behaviour and evaluate defensive security mechanisms. The work combines offensive security testing with defensive infrastructure deployment to analyse how cyber-physical systems can be protected against common network-based attacks.

The laboratory exercises presented in this repository cover several key security domains including attack simulation, network traffic analysis, firewall configuration, encrypted communication deployment, and intrusion detection engineering.

---

# Research Objectives

The primary aim of this project was to explore how cyber-physical systems can be secured against network-based attacks through a combination of detection, monitoring, and defensive infrastructure.

The research focused on several objectives:

- Simulating unauthorised access attempts against network services
- Analysing exploit traffic through packet-level inspection
- Evaluating firewall behaviour and network routing controls
- Deploying encrypted communication channels through VPN infrastructure
- Implementing intrusion detection systems capable of identifying malicious network activity

Through these experiments the project demonstrates how layered defensive mechanisms can be used to strengthen security across cyber-physical network environments.

---

# Cyber-Physical Threat Landscape

Cyber-physical systems are increasingly targeted by attackers due to their reliance on network connectivity and remote management. Devices operating within these environments often include industrial controllers, embedded systems, and IoT devices that may lack strong authentication or robust security controls.

Several large-scale cyber incidents have demonstrated the potential impact of compromised cyber-physical devices. Botnets composed of insecure IoT devices have previously been used to launch distributed denial-of-service attacks capable of disrupting major internet infrastructure.

Within this context, organisations must deploy multiple defensive mechanisms to detect intrusion attempts, monitor abnormal network activity, and protect critical systems from exploitation.

The following experiments were conducted to analyse these threats and evaluate practical defensive security techniques.

---

# Security Experiments

## SSH Brute Force Attack Simulation

Secure Shell (SSH) is widely used for remote administration of servers and network infrastructure. Due to its remote accessibility, SSH services are frequently targeted by automated brute-force attacks that attempt to guess authentication credentials.

This experiment simulated repeated unauthorised SSH login attempts against a Linux system in order to evaluate how intrusion prevention mechanisms detect and block malicious behaviour.

### Environment Configuration

- Virtualisation platform: Oracle VM VirtualBox  
- Operating system: Debian Linux  
- Remote administration service: OpenSSH  
- Intrusion prevention tool: SSHGuard  
- Firewall system: iptables  

### Attack Simulation

Multiple failed SSH login attempts were generated against the target system to replicate the behaviour of automated credential-guessing attacks commonly used by attackers.

Authentication logs were monitored to observe how repeated login failures were recorded within the system.

### Defensive Response

SSHGuard analysed the authentication logs and automatically identified repeated failed login attempts originating from the attacking host.

Once the attack threshold was reached, SSHGuard dynamically inserted firewall rules using iptables in order to block the offending IP address.

### Security Analysis

The experiment demonstrates how automated intrusion prevention systems can mitigate brute-force attacks by analysing authentication logs and dynamically blocking malicious hosts.

In real-world environments, this form of automated response is essential because manual monitoring of authentication logs would be insufficient to respond to high-volume credential attacks.

---

## Network Exploit Traffic Analysis

Network-level exploit analysis is an essential skill for security analysts and incident responders. Attackers often exploit protocol vulnerabilities in order to gain unauthorised system access or execute remote code.

This experiment analysed malicious network traffic associated with a well-known vulnerability in the Server Message Block (SMB) protocol.

### Analysis Tool

- Network packet analyser: Wireshark

### Analysis Process

Captured network traffic was inspected using protocol filters in order to isolate SMB communication between hosts.

The analysis focused on identifying abnormal packet behaviour that could indicate exploitation attempts.

Key characteristics examined included:

- unusual SMB command patterns
- abnormal packet sequences
- suspicious payload transmission
- fragmented network packets

### Observed Indicators

The captured traffic revealed abnormal SMB communication patterns consistent with exploit behaviour.

Indicators included irregular transaction requests and large outbound data transmissions that deviated from normal SMB traffic patterns.

### Security Implications

Packet-level traffic analysis allows security analysts to detect exploitation attempts by examining protocol behaviour and identifying anomalies in network communication.

This capability is critical for incident response teams investigating potential network intrusions.

---

## Firewall Architecture and Network Routing

Firewalls represent one of the primary defensive mechanisms used to protect cyber-physical network environments. They enforce security policies that regulate which network traffic is permitted to enter or leave a system.

This experiment focused on configuring firewall rules and network routing behaviour in order to control traffic flow within a virtualised network environment.

### Firewall Configuration

The firewall environment was configured using iptables within a Linux system.

Key firewall features implemented included:

- packet filtering
- network address translation (NAT)
- traffic forwarding rules
- access control policies

### Routing Behaviour

Network routing was configured to allow communication between different network segments while ensuring that unauthorised traffic could be restricted.

### Security Analysis

Firewall systems play a critical role in protecting cyber-physical networks by preventing unauthorised communication and limiting potential attack pathways.

Correct firewall configuration ensures that only legitimate traffic is permitted to interact with critical systems.

---

## Secure VPN Deployment

Cyber-physical systems often require remote management capabilities, which introduces additional security risks if communication channels are not properly protected.

To address this challenge, a Virtual Private Network (VPN) was deployed to provide encrypted communication between remote systems.

### VPN Implementation

The VPN infrastructure was implemented using OpenVPN.

Key configuration components included:

- TLS certificate generation
- encrypted communication tunnels
- client authentication
- secure key exchange

### Security Benefits

VPN technology ensures that network communication between remote systems is encrypted and protected from interception.

This is particularly important when managing distributed cyber-physical infrastructure across untrusted networks.

---

## Intrusion Detection System Deployment

Intrusion detection systems are used to monitor network traffic and identify malicious activity.

In this experiment, a network-based intrusion detection system was configured to analyse network traffic and generate alerts when suspicious activity was detected.

### IDS Platform

- Snort Network Intrusion Detection System

### Detection Capabilities

The IDS was configured to perform several security functions:

- packet inspection
- protocol analysis
- traffic logging
- signature-based threat detection

### Alert Generation

Snort analysed network traffic in real time and generated alerts when traffic patterns matched known attack signatures.

### Security Significance

Intrusion detection systems provide organisations with visibility into network activity and allow security teams to detect potential attacks before they escalate into full system compromise.

---

# Security Findings

The experiments conducted in this project demonstrate several important principles of cyber-physical system security.

Firstly, exposed network services such as SSH can be rapidly targeted by automated attacks if appropriate defensive controls are not implemented.

Secondly, packet-level network monitoring is essential for detecting exploit activity and understanding malicious network behaviour.

Thirdly, layered security architecture significantly improves system resilience. The combination of firewall rules, encrypted communication channels, and intrusion detection systems provides multiple defensive barriers that reduce the likelihood of successful compromise.

---

# Defensive Security Architecture

The project demonstrates how multiple defensive mechanisms can work together to protect cyber-physical network environments.

Key defensive technologies implemented include:

- firewall traffic control using iptables
- automated brute-force attack blocking with SSHGuard
- encrypted communication using OpenVPN
- network traffic monitoring using Wireshark
- intrusion detection using Snort

This layered defensive model reflects the principle of defence-in-depth commonly used in enterprise cybersecurity environments.

---

# Key Learning Outcomes

Through the completion of this project several important cybersecurity competencies were developed:

- practical attack simulation techniques
- packet-level network traffic analysis
- firewall configuration and network routing
- secure remote communication deployment
- intrusion detection system configuration

These skills are essential for cybersecurity professionals responsible for protecting network infrastructure and cyber-physical environments.

---

# Tools and Technologies

- Wireshark  
- Snort IDS  
- OpenVPN  
- SSHGuard  
- iptables  
- Oracle VM VirtualBox  
- Debian Linux  

---

# Author

Mohammad Mahmood  
MSc Cybersecurity
