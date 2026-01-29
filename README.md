Enterprise Headquarters & Branch Network Infrastructure

📘 Overview

-This project demonstrates the design and implementation of a secure enterprise

Headquarters–Branch network based on CCNA-level networking concepts.

The network uses department-based VLAN segmentation, centralized services,

dynamic routing, and multiple security controls to ensure efficient and secure

communication between the Headquarters and Branch offices.

🗺️ Network Topology

The network consists of two sites connected via a WAN link:

Side A – Headquarters (HQ)

Side B – Branch Office

The HQ hosts centralized network services (DHCP and DNS), while both sites are

segmented into multiple VLANs based on organizational departments.

⭐ Key Features

Multi-site enterprise network design (HQ & Branch)
Department-based VLAN segmentation
Inter-VLAN routing (Router-on-a-Stick)
Centralized DHCP and DNS services
Dynamic routing using OSPF
Secure remote management using SSH
Access control using ACLs
Switch port security implementation
End-to-end connectivity testing and verification

🛠️ Technologies Used

Cisco Packet Tracer
Cisco Routers and Switches
VLAN & Trunking (IEEE 802.1Q)
Inter-VLAN Routing
OSPF (Open Shortest Path First)
DHCP Server
DNS Server
Access Control Lists (ACL)
SSH (Secure Shell)
Switch Port Security

⚙️ Configuration Highlights

🔹VLAN Segmentation

VLANs are assigned per department to isolate broadcast domains
Separate VLANs are used for user traffic and server services

🔹Routing

OSPF is implemented to enable dynamic routing between HQ and Branch
Inter-VLAN routing is configured on the HQ router

🔹Network Services

DHCP and DNS services are centralized at the Headquarters
DHCP pools are created for each VLAN

🔹Security

VLAN isolation to limit unauthorized inter-department communication
Extended ACLs to control inter-VLAN traffic
SSH enabled on routers for secure remote access
ACL applied to VTY lines to restrict SSH access to the Admin workstation only
Port security enabled on access switch ports
