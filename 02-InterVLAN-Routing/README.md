# Inter-VLAN Routing using Router-on-a-Stick (ROAS)

## Overview
This lab demonstrates **Inter-VLAN Routing** using the **Router-on-a-Stick (ROAS)** method.  
A single router interface is configured with multiple sub-interfaces to route traffic between VLANs.

## Network Topology
- VLAN 10 (Users)
- VLAN 20 (Sales)
- One Layer 2 switch (Cisco 2960)
- One router (Cisco 2911)
- Trunk link between switch and router

## IP Addressing
### VLAN 10
- Network: 10.1.10.0/24
- Gateway: 10.1.10.1
- Hosts: 10.1.10.2, 10.1.10.3

### VLAN 20
- Network: 10.1.20.0/24
- Gateway: 10.1.20.1
- Hosts: 10.1.20.2, 10.1.20.3

## Configuration Summary
- Created VLANs on the switch
- Configured access ports for end devices
- Configured trunk port between switch and router
- Configured router sub-interfaces:
  - Gi0/0.10 for VLAN 10
  - Gi0/0.20 for VLAN 20
- Enabled 802.1Q encapsulation on sub-interfaces
- Set default gateways on all PCs

## Verification
- Successful ping between hosts in different VLANs
- Inter-VLAN communication verified through router

## Tools Used
- Cisco Packet Tracer
- Cisco 2960 Switch
- Cisco 2911 Router

## Author
Heint Thant Kyaw  
IT Networking & Cybersecurity Student

