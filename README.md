# KERNELiOS Networking Final Project
Overview
This project involved designing and implementing a fully functional network infrastructure from scratch to simulate a Small-to-Medium Business (SMB) environment. The goal was to ensure high availability, security, and efficient routing across multiple departments within a strictly timed window.

Technical Implementation
Routing & Switching:

OSPF: Implemented as the primary dynamic routing protocol for fast convergence and scalability.

Inter-VLAN Routing: Utilized to allow communication between different business departments (e.g., HR, IT, Finance) while maintaining logical separation.

Static & Default Routes: Configured for efficient edge traffic management and ISP simulation.

Security & Management:

Access Control Lists (ACLs): Deployed Standard and Extended ACLs to filter traffic and enforce security policies between VLANs.

Port Security: Configured on access switches to mitigate MAC address flooding and unauthorized device connections.

Secure Management: Disabled Telnet in favor of SSH v2 for encrypted remote administration of all network devices.

Services:

DHCP: Configured for automated IP address assignment across the infrastructure.

VLAN Design: Segmented the network to improve performance and security.

Tools Used
Cisco Packet Tracer / GNS3

Cisco IOS

Subnetting (VLSM)

How to Use
Download the provided .pkt file.

Open the file using Cisco Packet Tracer.

Test connectivity by pinging between different VLANs or checking the OSPF routing table using show ip route.
