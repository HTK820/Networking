# Multi-Area OSPF Configuration

## Overview
This lab demonstrates the configuration of **Multi-Area OSPF (Open Shortest Path First)** to enable scalable and efficient routing across different OSPF areas.

The network is divided into **Area 0 (Backbone Area)** and **Area 1**, showing how OSPF uses a hierarchical design to improve performance and reduce routing table size.

---

## Network Topology
The topology consists of:
- 3 Cisco 2911 Routers
- 2 Layer 2 switches
- Multiple LAN subnets
- Loopback interfaces for router identification
- Point-to-point links between routers

### OSPF Areas
- **Area 0 (Backbone)**
  - LAN: `10.1.1.0/24`
  - Loopback: `1.1.1.1/32`
- **Area 1**
  - LAN: `10.2.2.0/24`
  - Loopback: `3.3.3.3/32`
- **Inter-Area Link**
  - `192.168.1.0/30`
- **Additional Loopback**
  - `2.2.2.2/32`

---

## Configuration Objectives
- Configure OSPF on all routers
- Assign interfaces to correct OSPF areas
- Use **Area 0 as the backbone**
- Advertise LAN and loopback networks
- Verify inter-area routing and neighbor relationships

---

## Key Configuration Concepts
- OSPF process configuration using `router ospf`
- Area assignment with `network` statements
- Use of **loopback interfaces** for stable router IDs
- Multi-area OSPF design principles
- Inter-area route propagation

---

## Verification
The following checks are performed:
- `show ip ospf neighbor` to verify adjacency
- `show ip route ospf` to confirm learned routes
- Ping tests between hosts in different areas
- Ping tests to loopback interfaces

Successful communication confirms correct OSPF multi-area operation.

---

## Files Included
- `multi_area_ospf.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Multi-area OSPF configuration
- OSPF backbone and non-backbone areas
- Inter-area routing
- Router ID and loopback usage
- Enterprise network design principles

---

## Notes
Multi-area OSPF improves scalability and is widely used in **enterprise and ISP networks**.  
This lab reflects real-world OSPF deployment best practices.
