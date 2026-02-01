# Layer 3 EtherChannel Configuration

## Overview
This lab demonstrates **Layer 3 EtherChannel (Port-Channel)** configuration between two Layer 3 switches to provide increased bandwidth, redundancy, and efficient inter-VLAN routing.

Multiple physical links are bundled into a single **logical routed interface** using EtherChannel.

---

## Network Topology
The topology consists of:
- 2 Cisco 3560 Layer 3 switches
- 2 VLANs hosted on separate switches
- Layer 3 Port-Channel interface between switches
- End hosts connected to different VLANs

### VLAN and Subnet Design
- **VLAN 2**
  - Subnet: `10.1.2.0/24`
  - Gateway: `10.1.2.1`
- **VLAN 3**
  - Subnet: `10.1.3.0/24`
  - Gateway: `10.1.3.1`
- **Port-Channel Network**
  - Subnet: `10.1.12.0/24`

---

## Configuration Objectives
- Bundle multiple physical links using EtherChannel
- Configure **Layer 3 Port-Channel**
- Enable routing between VLANs across switches
- Ensure redundancy and load balancing
- Verify connectivity between VLAN hosts

---

## Key Configuration Concepts
- EtherChannel using `channel-group`
- Routed Port-Channel (`no switchport`)
- VLAN interface configuration (SVI)
- Inter-switch Layer 3 routing
- Redundancy and bandwidth aggregation

---

## Verification
The following checks are performed:
- `show etherchannel summary`
- `show ip route`
- Ping tests between VLAN 2 and VLAN 3 hosts
- Link failure testing to confirm redundancy

Successful ping results confirm correct Layer 3 EtherChannel operation.

---

## Files Included
- `l3_etherchannel.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Layer 3 EtherChannel configuration
- Inter-VLAN routing
- Switch-to-switch routed links
- Enterprise network design
- High availability and link redundancy

---

## Notes
Layer 3 EtherChannel is commonly used in **enterprise core and distribution layers** to improve performance and resiliency.
