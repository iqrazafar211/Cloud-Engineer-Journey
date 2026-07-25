# Day 1 — Computer Networking

Date: Day 1

## Topics covered
- Computer networking fundamentals
- LAN, MAN, WAN
- IP addresses (public vs private)
- Routers and switches
- Basic internetworking concepts
- Why networking matters for cloud computing

## Summary
Networking is the foundation that enables devices and systems to communicate. In cloud computing, understanding how networks connect, address, and route traffic is essential for designing, securing, and troubleshooting cloud architectures.

## Key concepts

- LAN (Local Area Network): network covering a small/local area (home, office).  
- MAN (Metropolitan Area Network): covers a city or metropolitan area.  
- WAN (Wide Area Network): covers large geographic areas, often connecting LANs across regions.

- IP address: numeric identifier for a device on a network. Examples: IPv4 (e.g., 192.0.2.1), IPv6 (e.g., 2001:db8::1).
- Private IP addresses: used inside local networks (not routable on the public internet). Common IPv4 ranges:
  - 10.0.0.0/8
  - 172.16.0.0/12
  - 192.168.0.0/16
- Public IP addresses: assigned to networks or devices to be reachable over the internet.

- Switch: connects devices within the same network (Layer 2 — forwards by MAC address).
- Router: connects different networks and forwards traffic between them (Layer 3 — forwards by IP).

## Practical commands / checks
- Windows: `ipconfig` — view IP configuration
- Linux/macOS: `ifconfig` or `ip addr` — view IP configuration
- Check external/public IP: `curl ifconfig.me` or visit a "what is my IP" service

## Basic topology (example)
- Home/office: devices → switch → router → ISP → Internet
- In cloud: VM/subnet → virtual router (VPC gateway) → Internet gateway / NAT

## Why networking matters in cloud computing
- Cloud architectures depend on virtual networks (VPCs/subnets), routing, and security controls (security groups, NACLs).
- Proper IP addressing, segmentation, and routing are essential for availability, performance, and security.

## Next steps / study recommendations
- Learn subnetting and CIDR notation (how to divide networks).
- Practice using cloud provider networking (create VPCs, subnets, route tables).
- Study basic firewall/security group concepts and NAT.

## Resources
- "TCP/IP Illustrated" (book) — fundamentals
- Cloud provider docs: AWS VPC, Azure Virtual Network, GCP VPC
- Quick subnetting guides and CIDR calculators (online)

## Day 1 Status
Completed
