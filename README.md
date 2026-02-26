# KERNELiOS Networking Final Project

### Overview

This project is a comprehensive Cisco simulation of a multi-area enterprise network designed for a small-to-medium business (SMB). It features a robust OSPF architecture, centralized server management, and multi-layered security protocols to ensure a scalable and secure corporate environment.

### Network Architecture

The infrastructure is segmented into distinct logical areas to optimize routing performance and organizational structure:

* **Multi-Area OSPF:**
* **Area 0 (Core/WAN):** Interconnects all routers using high-speed WAN links.
* **LANs 1-3:** Departmental segments, each utilizing its own switch with **PVST (Per-VLAN Spanning Tree)** for loop prevention across 3 distinct VLANs per LAN.
* **LAN 4:** Dedicated Wireless (Wi-Fi) segment for mobile connectivity.
* **LAN 5:** Centralized Server Farm hosting critical business services.


* **Edge Connectivity:**
* **ISP Simulation (LAN 10):** A dedicated area mimicking external internet connectivity.
* **Redundancy:** Configured with a Primary Default Route and a **Floating Default Route** for failover reliability.
* **NAT/PAT:** Implemented on Router 3 to mask internal IP addresses for secure internet egress.



### Implemented Services (LAN 5)

* **DHCP:** Dynamic addressing for the majority of the network.
* **DNS:** Internal name resolution, including a hosted web server and specific PC endpoints.
* **NTP & Syslog:** Centralized time synchronization and logging for all networking equipment in LAN 2, ensuring audit-ready management.

### Security & Access Control

* **Access Control Lists (ACL):** Traffic filtering example implemented on PC 5 (LAN 2).
* **Port Security:** MAC-based security example configured in LAN 2 (PC 4).
* **Encrypted Management:** All switches in LAN 2 are configured with **SSH v2** (Telnet disabled) for secure remote administration.
* **Authentication:** Password protection examples implemented across all Area 1 routers.

### Technical Stack

* **Protocols:** OSPF, PVST, NAT/PAT, SSH, DHCP, DNS, NTP, Syslog.
* **Tools:** Cisco Packet Tracer / Cisco IOS.
* **Concepts:** VLSM Subnetting, Inter-VLAN Routing, WAN Encapsulation.


### Pro-Tip for your GitHub:

Now that you have the text, make sure to upload your **.pkt** file to the same repository. If you have a screenshot of the network topology, I recommend adding it to the top of the README using this syntax:
`![Network Topology](your_image_name.png)`

**Would you like me to help you write a "Troubleshooting" section that explains how you verified the OSPF convergence or the NAT translations?**
