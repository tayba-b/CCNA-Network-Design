# Enterprise Network Project

A complete simulation of a headquarters and branch office network, featuring department-based VLANs, inter-VLAN routing, OSPF dynamic routing, port security, SSH remote access, DHCP, and DNS services. The project demonstrates network design, configuration, and basic security measures in a professional enterprise environment.

---

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

---

## Network Topology

*The network consists of a Headquarters (Site A) and a Branch Office (Site B), connected via OSPF routing. Each site contains multiple VLANs segregated by department.*

![Network Topology](screenshots/Network_Topology.png)

---

## Key Features

- Department-based VLAN segmentation (Admin, HR, Sales, Finance, Server Room)  
- Inter-VLAN routing using router-on-a-stick  
- OSPF dynamic routing between Headquarters and Branch  
- Port security on all switch access ports  
- SSH remote access restricted with ACL  
- DHCP and DNS services for all VLANs  
- VLAN isolation and ACL-based site access control  

---

## Technologies Used

- Cisco Packet Tracer  
- VLANs and Subnetting  
- Router-on-a-stick Inter-VLAN Routing  
- OSPF Routing Protocol  
- Port Security  
- SSH Remote Access with ACL  
- DHCP and DNS Services  

---

## Configuration Highlights

VLAN Segmentation

-- Department-based VLANs for HQ and Branch (Admin, HR, Sales, Finance, Server Room)

Inter-VLAN Routing

-- Router-on-a-stick using sub-interfaces for each VLAN

Dynamic Routing

-- OSPF configured between HQ (Site A) and Branch (Site B)

Port Security

-- Enabled on all access ports with sticky MAC and violation restrict

SSH Access Control

-- SSH enabled on routers
-- Restricted access via ACL for administrator PCs only

DHCP and DNS

-- DHCP server assigns IPs per VLAN
-- DNS server resolves hostnames within the network

Network Security

-- VLAN isolation between departments and sites
-- ACLs and port security enhance overall security

