# Single Area OSPF Configuration (Area 0)

## Overview
This lab demonstrates the configuration of **Open Shortest Path First (OSPF)** using a **single backbone area (Area 0)**.

The topology includes multiple routers with point-to-point links and loopback interfaces, all advertised dynamically using OSPF.

---

## Network Topology
- 3 Cisco 2911 routers (R1, R2, R3)
- Single OSPF Area: **Area 0**
- Point-to-point links between routers
- Loopback interfaces used as router IDs and advertised networks

---

## IP Addressing

### Router Links
- R1 ↔ R2: `10.1.12.0/24`
- R1 ↔ R3: `10.1.13.0/24`

### Loopback Interfaces
- R1: `192.168.10.1/24`
- R2: `192.168.20.1/24`
- R3: `192.168.30.1/24`

---

## OSPF Configuration
- OSPF process enabled on all routers
- All networks advertised into **Area 0**
- Loopback interfaces included in OSPF
- Automatic route learning between routers

---

## Verification
- Verified OSPF neighbor adjacency using `show ip ospf neighbor`
- Verified learned routes using `show ip route ospf`
- Successful end-to-end connectivity using ping tests

---

## Key Concepts Demonstrated
- OSPF single-area design
- Dynamic routing
- Router ID selection using loopback interfaces
- Link-state routing fundamentals

---

## Files Included
- `single_area_ospf.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Dynamic routing protocols
- OSPF configuration and verification
- Enterprise routing design principles
