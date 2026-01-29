# Enterprise Network Project
A complete simulation of a headquarters and branch office network with VLANs, OSPF routing, port security, SSH access, DHCP, and DNS services.


## Table of Contents
- [Network Topology](#network-topology)
- [Key Features](#key-features)
- [Technologies Used](#technologies-used)
- [Configuration Highlights](#configuration-highlights)
- [Screenshots](#screenshots)
- [How to Use](#how-to-use)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Network Topology
![Network Topology](screenshots/Network_Topology.png)

## Key Features
- VLAN segmentation per department
- Inter-VLAN routing using OSPF
- Port security on all access ports
- SSH access restricted via ACL
- DHCP and DNS services
- Access control for site-to-site traffic (future ACL implementation)

## Technologies Used
- Cisco Packet Tracer
- VLANs, ACLs, Port Security
- SSH remote access
- OSPF routing protocol
- DHCP and DNS services

Configuration Highlights

VLAN Segmentation: The network is divided by department for better organization and security.

VLAN 10: Admin

VLAN 20: HR

VLAN 30: Sales

VLAN 40: Finance

VLAN 50-80 (Branch side) mirror the departments at the branch

VLAN 90: Server Room

Inter-VLAN Routing: Configured router-on-a-stick using sub-interfaces on routers for each VLAN to enable communication within the same site while maintaining isolation between VLANs.

Dynamic Routing: OSPF is used between Site A (Headquarters) and Site B (Branch) to ensure proper route exchange and network connectivity.

Port Security: Implemented on all switch access ports:

Maximum 2 MAC addresses per port

Sticky MAC addresses to bind devices permanently

Violation set to restrict unauthorized devices

SSH Access Control: Remote access to routers is secured via SSH and restricted using an ACL to allow only authorized administrator PCs.

DHCP and DNS Services:

DHCP server assigns IPs to devices per VLAN

DNS server configured to resolve hostnames within the network

Network Security: VLAN isolation is applied to prevent unauthorized access between VLANs and sites. ACLs and port security enhance overall network security
VLAN isolation to limit unauthorized inter-department communication
Extended ACLs to control inter-VLAN traffic
SSH enabled on routers for secure remote access
ACL applied to VTY lines to restrict SSH access to the Admin workstation only
Port security enabled on access switch ports
