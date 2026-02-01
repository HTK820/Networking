# Layer 3 Switch Route Port Configuration

## Overview
This lab demonstrates **Layer 3 switching using routed ports** on a multilayer switch.

Instead of using a trunk link or Router-on-a-Stick, the Layer 3 switch is configured with:
- SVIs for inter-VLAN routing
- A routed physical interface (`no switchport`) to connect directly to an upstream router

---

## Network Topology
- Cisco 3560 Layer 3 Switch
- Cisco 2911 Router (R1)
- Simulated ISP router with loopback addresses
- Two VLANs:
  - VLAN 10
  - VLAN 20

---

## VLAN & IP Addressing

### VLAN 10
- Network: `10.1.10.0/24`
- Default Gateway: `10.1.10.1`

### VLAN 20
- Network: `10.1.20.0/24`
- Default Gateway: `10.1.20.1`

### Routed Port (L3 Switch → Router)
- Network: `10.1.30.0/24`
- Layer 3 Switch: `10.1.30.1`
- Router (R1): `10.1.30.2`

---

## Key Configurations
- Enabled IP routing on Layer 3 switch
- Configured SVIs for VLAN 10 and VLAN 20
- Converted switch interface to routed port using `no switchport`
- Configured static route/default route toward the router
- Router connected to simulated ISP with loopback interfaces

---

## Verification
- Verified inter-VLAN communication
- Verified connectivity from VLANs to upstream router
- Tested reachability to ISP loopback addresses
- Used `ping`, `show ip route`, and `show ip interface brief`

---

## Key Concepts Demonstrated
- Layer 3 switching
- Routed ports vs trunk ports
- Inter-VLAN routing using SVIs
- Enterprise campus design fundamentals

---

## Files Included
- `l3_route_port.pkt` – Cisco Packet Tracer lab file
- `topology.png` – Network topology diagram

---

## Skills Demonstrated
- Layer 3 switch configuration
- Enterprise VLAN routing design
- Campus-to-WAN connectivity
