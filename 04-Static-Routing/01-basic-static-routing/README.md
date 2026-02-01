# Basic Static Routing with Three Routers

## Overview
This lab demonstrates **static routing between multiple LAN networks** using three routers.  
It simulates a small routed network where end devices communicate across different subnets via static routes.

## Network Topology
- 3 Cisco 2911 Routers
- 3 Layer 2 switches
- 3 LAN segments
- Inter-router point-to-point links

## LAN Subnets
- LAN 1: 10.1.1.0/24
- LAN 2: 10.0.1.0/24
- LAN 3: 10.1.2.0/24

## Inter-Router Networks
- Router3 ↔ Router1: 10.1.0.0/24
- Router1 ↔ Router2: 10.0.0.0/24

## Routing Configuration
- Static routes configured on all routers
- Each router has reachability to all remote LANs
- Default gateways configured on end devices

## Verification
- Successful ping tests between all PCs
- Multi-hop routing verified across routers

## Skills Demonstrated
- Static routing configuration
- IP addressing and subnetting
- Router-to-router connectivity
- Network troubleshooting fundamentals

## Tools Used
- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches

## Author
Heint Thant Kyaw  
IT Networking & Cybersecurity Student
