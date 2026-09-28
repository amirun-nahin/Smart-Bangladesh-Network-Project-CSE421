# Smart Bangladesh Digital City Network

> A Cisco Packet Tracer network design that connects six government departments into one secure network.

## Overview

The Smart Bangladesh Digital City (SBDC) initiative aims to bring essential public services onto one secure network. This project designs and implements that network in Cisco Packet Tracer for six departments:

- Smart City Control Center (SCCC)
- Traffic Management Authority (TMA)
- Public Health Department (PHD)
- Education Service Center (ESC)
- Emergency Response Unit (ERU)
- Digital Citizen Service (DCS)

Each department has its own router, a LAN switch, two PCs, and a network printer. The departments are linked so that there is more than one routing path between them.

The network includes:

- **Addressing:** VLSM subnetting of a /16 base network for department LANs and router-to-router links
- **Routing:** RIPv2 between SCCC, TMA and PHD, plus next-hop, directly connected, default, and floating static routes on the other routers
- **DHCP:** router-based DHCP (SCCC), dedicated DHCP servers (DCS and ERU), and DHCP relay for ESC
- **Services:** a central DNS server, two websites, and email servers for two domains with cross-domain mail
- **Backup routing:** automatic failover through a floating static route if the primary link goes down

## Documentation

The VLSM calculation, IP address table, configuration commands, and test screenshots are in the project report: [`CSE421-Project-Group-2703.pdf`](CSE421-Project-Group-2703.pdf). The original assignment is in [`8__Smart_Bangladesh_Digital_City_Network.pdf`](8__Smart_Bangladesh_Digital_City_Network.pdf).

## Repository Contents

- `CSE421-Project-Group-2703.pkt`: the Cisco Packet Tracer project
- `CSE421-Project-Group-2703.pdf`: project report
- `8__Smart_Bangladesh_Digital_City_Network.pdf`: project brief
