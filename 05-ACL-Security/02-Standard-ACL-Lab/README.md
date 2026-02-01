# Standard ACL Configuration – Lab 2

## Overview
This lab demonstrates the use of **Standard Access Control Lists (ACLs)** to control traffic between multiple LAN subnets and server networks.

The focus is on **source-based traffic filtering** using standard ACL rules applied at appropriate router interfaces.

---

## Network Topology
The topology includes:
- 2 Cisco 2911 routers (R1, R2)
- 3 LAN segments
- 1 server network
- Serial WAN link between routers

---

## IP Addressing

### LAN Subnets
- Host A & B: `10.1.1.0/24`
- Host C: `10.3.3.0/24`
- Server Network: `10.2.2.0/24`

### WAN Link
- `10.1.12.0/30`

---

## ACL Scenarios Implemented

1. Server S1 **can access** subnet of Host A and B  
2. Server S1 **cannot access** Host C subnet  
3. Server S2 **can access** Host C subnet  
4. Server S2 **cannot access** Host A and B subnet  

---

## Configuration Objectives
- Configure standard ACLs
- Apply ACLs on correct router interfaces
- Control access based on source IP addresses
- Verify access using ping tests

---

## Key Concepts
- Standard ACL (`access-list 1 permit|deny`)
- Source-based filtering
- Interface ACL application
- Security segmentation

---

## Verification
- Ping tests from servers to hosts
- Confirm allowed and denied traffic behavior
- Verify ACL counters using `show access-lists`

---

## Files Included
- `standard_acl_lab2.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Network security fundamentals
- Standard ACL configuration
- Traffic filtering
- Enterprise access control design
