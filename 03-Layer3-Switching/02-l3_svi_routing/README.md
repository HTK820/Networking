# Inter-VLAN Routing using Layer 3 Switch (SVI)

## Overview
This lab demonstrates **Inter-VLAN Routing using a Layer 3 Switch** with **SVI (Switched Virtual Interfaces)**.  
Routing between VLANs is performed directly on the switch without using Router-on-a-Stick.

## Network Topology
- Layer 3 Switch (Cisco 3560)
- Router (Cisco 2911) simulating external/ISP connectivity
- Two VLANs:
  - ENG VLAN
  - SALES VLAN

## VLAN & IP Addressing

### ENG VLAN
- Network: 10.10.10.0/24
- Default Gateway (SVI): 10.10.10.1
- Hosts:
  - 10.10.10.10
  - 10.10.10.11
  - 10.10.10.12

### SALES VLAN
- Network: 10.10.20.0/24
- Default Gateway (SVI): 10.10.20.1
- Hosts:
  - 10.10.20.10
  - 10.10.20.11

## Layer 3 Switch Configuration
- VLANs created on the switch
- SVI interfaces configured:
  - Interface VLAN 10 → 10.10.10.1
  - Interface VLAN 20 → 10.10.20.1
- IP routing enabled on the Layer 3 switch
- Access ports assigned to correct VLANs

## External Connectivity
- Router connected to Layer 3 switch
- Router interface IP: 203.0.113.1
- Loopback interface configured (8.8.8.8) to simulate external network

## Verification
- Successful inter-VLAN communication between ENG and SALES hosts
- Hosts can reach external loopback address
- Default gateway functionality verified via SVI

## Tools Used
- Cisco Packet Tracer
- Cisco 3560 Layer 3 Switch
- Cisco 2911 Router

## Author
Heint Thant Kyaw  
IT Networking & Cybersecurity Student


