# Multi-Router Static Routing with Multiple Subnets

## Overview
This lab demonstrates **static routing across multiple routers** connecting several LAN subnets.  
The topology simulates a small enterprise network with multiple departments and routing paths.

## Network Topology
- 4 Cisco 2911 Routers (R1, R2, R3, R4)
- Multiple Layer 2 switches
- End hosts across six LAN subnets
- Point-to-point links between routers

## LAN Subnets

### Left Side Networks
- Subnet A: 192.168.1.0/24
- Subnet B: 192.168.2.0/24
- Subnet C: 192.168.3.0/24

### Right Side Networks
- Subnet D: 192.168.4.0/24
- Subnet E: 192.168.5.0/24
- Subnet F: 192.168.6.0/24

## Inter-Router Networks
- 192.168.7.0
- 192.168.8.0
- 192.168.9.0
- 192.168.10.0

## Routing Configuration
- Static routes configured on all routers
- Each router has routes to all remote LAN subnets
- Redundant routing paths implemented between routers

## Verification
- End-to-end connectivity verified between all LAN subnets
- Successful ping tests across multiple routing hops
- Static route correctness validated

## Skills Demonstrated
- IP subnetting
- Static routing
- Multi-router topology design
- Troubleshooting connectivity issues
- Enterprise-style network segmentation

## Tools Used
- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches
