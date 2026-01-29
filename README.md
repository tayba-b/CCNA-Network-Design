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

## Configuration Highlights

VLAN Segmentation

-- VLAN 10: Admin
-- VLAN 20: HR
-- VLAN 30: Sales
-- VLAN 40: Finance
-- VLAN 50: Admin (Branch)
-- VLAN 60: HR (Branch)
-- VLAN 70: Sales (Branch)
-- VLAN 80: Finance (Branch)
-- VLAN 90: Server Room

Extended ACLs to control inter-VLAN traffic
SSH enabled on routers for secure remote access
ACL applied to VTY lines to restrict SSH access to the Admin workstation only
Port security enabled on access switch ports
