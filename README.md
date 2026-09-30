Cisco Network Design & Implementation

A complete multi-site enterprise network designed, implemented, configured, tested, and troubleshot using Cisco Packet Tracer.

Project Overview

This project demonstrates the design and implementation of an enterprise network connecting multiple network segments, including:

HQ1

HQ2

Server / SP Office

Users Network

Public Network

Core WAN

The project focuses on practical network engineering, including IP addressing, VLAN segmentation, dynamic routing, network services, security, WAN connectivity, testing, and troubleshooting.

Key Implementations

VLSM-based IP addressing and subnetting

VLAN segmentation

Inter-VLAN Routing

802.1Q trunking

LACP EtherChannel

OSPF dynamic routing using Area 0

DHCP for dynamic IP addressing

Static NAT for public access to an internal server

SSH and secure remote access

Local user authentication

Console and VTY security

Enable Secret and password encryption

WAN point-to-point connectivity

End-to-end connectivity testing

OSPF neighbor verification

NAT translation verification

DHCP verification

Network troubleshooting and issue resolution

Network Architecture

The topology is organized into multiple functional areas:

HQ1

HQ1 contains multiple VLANs and Layer 3 routing components, with dedicated user networks and routed connections toward the WAN/core infrastructure.

HQ2

HQ2 uses VLAN segmentation and routed connectivity to provide communication between its internal networks and the rest of the enterprise infrastructure.

Server / SP Office

The Server / SP Office contains internal servers and a WAN connection. Static NAT is implemented to provide external access to an internal server through a public address.

Users Network

The Users Network uses DHCP to provide dynamic IP addressing, default gateway information, and DNS configuration to clients.

Public Network

The public side of the infrastructure is connected through the core WAN and is used to demonstrate external access through Static NAT.

Core WAN

Core_Router6 provides the central WAN connectivity between the major network segments.

Routing

OSPF is implemented across the network using:

OSPF Process ID: 1

Area: 0

Router IDs configured for the participating routers

OSPF neighbor relationships and routing behavior were verified using Cisco IOS verification commands.

Network Services

DHCP

DHCP is configured for the Users Network to provide dynamic addressing and network configuration to clients.

NAT

Static NAT is configured to map the internal server address:

192.168.1.2

to the public address:

203.0.0.10

NAT translations are verified using Cisco IOS commands.

Security Configuration

The project includes practical device-access security configurations such as:

SSH

Local authentication

Console password protection

VTY line security

Enable Secret

Password encryption

Verification & Testing

The network was tested using multiple verification methods, including:

Local gateway connectivity

Cross-site connectivity

End-to-end ping tests

OSPF neighbor verification

NAT translation verification

DHCP verification

WAN connectivity checks

The testing phase was used to confirm that the implemented network components operate together as expected.

Troubleshooting

Several configuration issues were identified and resolved during implementation, including:

VLAN communication problems caused by missing Layer 3 routing configuration

WAN access problems related to private addressing and Static NAT

DHCP clients receiving addresses without the required default gateway configuration

Each issue was investigated, corrected, and verified through subsequent testing.

Technologies

Cisco Packet Tracer

Cisco IOS

VLAN

Inter-VLAN Routing

OSPF

NAT

DHCP

VLSM

EtherChannel

LACP

SSH

TCP/IP

Project Structure

Cisco-Network-Design-Implementation/
│
├── README.md
├── Packet-Tracer/
│   └── project.pkt
│
├── Report/
│   └── Final-Project-Report.pdf
│
├── Topology/
│   └── Complete-Topology.png
│
├── Screenshots/
│   ├── HQ1/
│   ├── HQ2/
│   ├── Server-SP-Office/
│   ├── Users-DHCP/
│   ├── Public-Network/
│   ├── Core-WAN/
│   ├── OSPF/
│   ├── NAT/
│   └── Testing/
│
└── Documentation/
    └── Configuration-Notes.md

Project Documentation

The repository includes the Cisco Packet Tracer project file, supporting screenshots, network documentation, and the final project report.

Author

Youssef Salah

Instructor

Eng. Saher Waleed

This project was developed as a practical implementation of enterprise networking concepts, with emphasis on network design, configuration, verification, and troubleshooting.
