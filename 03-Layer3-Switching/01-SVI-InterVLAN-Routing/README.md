# Inter-VLAN Routing using SVI on Layer 3 Switch

## Overview
This lab demonstrates **Inter-VLAN Routing using Switch Virtual Interfaces (SVI)** on a Cisco Layer 3 switch.

Instead of using Router-on-a-Stick, the Layer 3 switch performs routing internally, providing better performance and scalability.

---

## Network Topology
The topology consists of:
- 1 Cisco 3560 Layer 3 switch
- 1 Cisco 2911 router (external VLAN connectivity)
- 3 VLANs
- End hosts connected to different VLANs

---

## VLAN and IP Design

### VLAN 10
- Subnet: `10.1.10.0/24`
- Gateway: `10.1.10.1`

### VLAN 20
- Subnet: `10.1.20.0/24`
- Gateway: `10.1.20.1`

### VLAN 30
- Subnet: `10.1.30.0/24`
- Used for router uplink and external connectivity

---

## Configuration Objectives
- Create VLANs on Layer 3 switch
- Configure SVI interfaces
- Enable IP routing on the switch
- Assign access ports to correct VLANs
- Verify inter-VLAN communication

---

## Key Configuration Concepts
- `interface vlan X`
- `ip routing`
- Layer 3 switching
- Default gateway configuration
- Enterprise campus switching design

---

## Verification
- Ping tests between VLAN 10 and VLAN 20 hosts
- Verify routing table using `show ip route`
- Confirm SVI status using `show ip interface brief`

Successful communication confirms correct SVI-based routing.

---

## Files Included
- `svi_intervlan.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Layer 3 switching
- Inter-VLAN routing using SVI
- Enterprise VLAN design
- Network segmentation
- Performance-optimized routing

---

## Notes
SVI-based routing is preferred in enterprise networks due to higher throughput and lower latency compared to Router-on-a-Stick.
