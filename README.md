🏥 Secure Healthcare Network Infrastructure
📌 Project Overview

This project focuses on the design and implementation of a secure, scalable, and high-availability healthcare network system. The solution was developed for Dr. Devi ShettyLabs Limited, a leading healthcare diagnostics provider headquartered in Mumbai, India.

The network spans multiple departments across three floors, accommodating 2,120+ users (with scalability to double by 2025). The design ensures Confidentiality, Integrity, and Availability (CIA) of critical healthcare data while supporting robust performance, redundancy, and enterprise security.

🎯 Objectives

Build a secure, scalable, and redundant network for healthcare operations.

Segment departments into dedicated VLANs for better performance and security.

Provide secure communication using ACLs, Firewalls, and IPsec VPNs.

Enable VoIP telephony, WLAN connectivity, and centralized IT services.

Implement high availability (HSRP, failover servers, redundancy).

Integrate on-premise and cloud (AWS) resources for business continuity.

🏗️ Network Infrastructure
🔹 Core Components

ISP Connectivity: Airtel ISP with static public IPs.

Firewall: Cisco ASA 5500-X series for advanced security.

Routing: Cisco WAN Router (configured for VoIP + OSPF).

Switching:

2 × Catalyst 3850 (Core L3 switches)

8 × Catalyst 2960 (48-Port Access switches)

2 × Catalyst 2960 (24-Port Access switches)

Servers (VMware ESXi on HP ProLiant DL38 Gen10):

Active Directory (LDAP + DNS + DHCP)

Health Information System (HIS)

Email & File Server

Failover & Redundancy Configured

Storage: NetApp devices for centralized storage.

Wireless: Cisco WLC + 10 Lightweight Access Points.

VoIP: Cisco Voice Gateways + IP Phones across departments.

Cloud Integration: AWS for global service access.

🔑 Technologies Implemented

Hierarchical Design with redundancy

VLANs:

LAN → VLAN 10

WLAN → VLAN 50

VoIP → VLAN 99

Routing: OSPF + Static Default Routes

HSRP: High Availability & Failover for Core Routers

EtherChannel (LACP) for link aggregation

STP Enhancements: PortFast + BPDU Guard

DHCP (via AD Servers) for dynamic addressing

NAT/PAT for outbound Internet access

Access Control Lists (ACLs): Standard + Extended rules

SSH Access Control for secure remote administration

VoIP Telephony with dial plan (3xxx numbering)

Site-to-Site VPN (IPsec) for secure branch-HQ communication

🌐 Addressing Scheme

LAN → 192.168.0.0/20

WLAN → 10.10.0.0/16

Voice → 172.16.0.0/20

DMZ → 10.20.20.0/26

Public IPs → 197.200.100.0

🛡️ Security Features

Cisco ASA Firewall → Security zones + policies

VLAN segmentation → Isolate LAN, WLAN & VoIP

SSH-only remote management

Sticky MAC + Port Security on servers

IPsec VPN → Encrypted HQ ↔ Branch communication

HSRP → Redundancy for core routing

Failover Servers → Continuous availability of HIS, DNS, Email

📊 Deliverables

Network Topology Diagram (Cisco Packet Tracer file .pkt)

Configuration Scripts (Switches, Routers, Firewalls)

Testing & Verification (Connectivity, Security, Failover)

🚀 How to Use

Install Cisco Packet Tracer.

Open the provided .pkt file.

Explore topology, routing, VLANs, and firewall rules.

Test configurations (e.g., ping, VoIP calls, SSH access).

---

👤 Author

Developed by Saurav Pokhrel

🎓 Postgraduate in Computer System Technology & Networking (Centennial College)

🎓 Bachelor’s in Ethical Hacking & Cybersecurity (Coventry University)


