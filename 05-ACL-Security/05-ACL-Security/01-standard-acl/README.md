# Standard ACL Configuration – Lab 2

## Overview
This lab demonstrates the implementation of **Standard Access Control Lists (ACLs)** to control network traffic based on **source IP addresses**.  
The objective is to apply security policies that allow or deny access between hosts and servers across multiple subnets.

This lab focuses on **basic network security concepts** using Cisco IOS Standard ACLs.

---

## Network Topology
The network consists of:
- 2 Cisco 2911 Routers (R1, R2)
- 3 Layer 2 switches
- Multiple client PCs
- Two servers located in a remote subnet
- Point-to-point serial connection between routers

Subnet layout:
- **Host Subnet A:** `10.1.1.0/24`
- **Host Subnet B:** `10.3.3.0/24`
- **Server Subnet:** `10.2.2.0/24`
- **WAN Links:** `/30` point-to-point networks

---

## Lab Scenarios
The following access control requirements are implemented:

1. **Server S1** is allowed to access subnets of **Host A and Host B**
2. **Server S1** is denied access to **Host C’s subnet**
3. **Server S2** is allowed to access **Host C’s subnet**
4. **Server S2** is denied access to **Host A and Host B subnets**

These scenarios simulate real-world access policies where different servers have different access permissions.

---

## Configuration Highlights
- Standard ACLs are configured using **source IP filtering**
- ACLs are applied **inbound/outbound** on router interfaces
- Correct placement of ACLs is emphasized to minimize unnecessary traffic
- Connectivity is verified using `ping` tests after ACL implementation

---

## Verification
- Successful and failed ping tests confirm correct ACL behavior
- Traffic is permitted or denied according to the defined scenarios
- Routing remains functional while access is selectively restricted

---

## Files Included
- `standard_acl_lab2.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Standard ACL configuration
- Network traffic filtering
- Basic network security principles
- Cisco IOS command-line usage
- Access policy implementation and testing

---

## Notes
This lab uses **Standard ACLs**, which filter traffic only by source IP address.  
For more granular control (destination, protocol, port), **Extended ACLs** should be used.
