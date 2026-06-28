# Enterprise Network Topology — Cisco Packet Tracer

![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-1BA0D7?style=flat&logo=cisco&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Course](https://img.shields.io/badge/Course-Computer%20Networks%20Lab-orange)

> A fully configured dual-office enterprise network simulation built in Cisco Packet Tracer,
> featuring VLANs, inter-VLAN routing, departmental segmentation, and a branch office 
> connected via WAN link.

---

## Project Overview

This project simulates a real-world enterprise network for an organization with a **Main Office**
and a **Branch Office**, connected through WAN routers (2911 series). The network is segmented 
into multiple VLANs for each department, managed via Layer 3 switches and routers to ensure 
secure, organized, and efficient communication.

**Course:** Computer Networks Lab  
**Institution:** AIR University
**Team Members:**
- Muhammad Afnan Jadoon (241873)
- Muhammad Ahsan Ali Shah (241852)
- Muhammad Abdul Hanan (241789)


---

## Network Architecture

### Main Office
| Department       | Hosts          | Device Range     |
|-----------------|----------------|------------------|
| Sales PC         | 6 PCs          | PC0 – PC5        |
| Engineering PC   | 6 PCs          | PC6 – PC11       |
| Management PC    | 2 PCs          | PC16 – PC17      |
| Finance PC       | 4 PCs          | PC12 – PC15      |
| Servers          | 3 Servers      | Web, File, Email |

### Branch Office
| Department            | Hosts          | Device Range     |
|----------------------|----------------|------------------|
| Marketing PC          | 4 PCs          | PC18 – PC21      |
| Support PCs           | 4 PCs          | PC22 – PC25      |
| Branch Management     | 1 PC           | PC26             |
| Laptops               | 2 Laptops      | Laptop0 – Laptop1|

---

## Network Devices Used

| Device              | Model          | Count | Role                          |
|--------------------|----------------|-------|-------------------------------|
| Routers             | Cisco 2911     | 2     | WAN link, inter-office routing|
| Layer 3 Switches    | Cisco 3560-24PS| 2     | Inter-VLAN routing            |
| Layer 2 Switches    | Cisco 2950-24  | 2     | Access layer switching        |
| Servers             | Server-PT      | 3     | Web, File, Email services     |
| PCs                 | PC-PT          | 27    | End-user workstations         |
| Laptops             | Laptop-PT      | 2     | Mobile workstations           |

---

## Technologies & Protocols Configured

- **VLANs** — Departmental network segmentation
- **Inter-VLAN Routing** — Via Layer 3 switches (3560-24PS)
- **Static / Dynamic Routing** — Between Main and Branch office routers
- **DHCP** — Dynamic IP assignment per VLAN
- **DNS** — Name resolution via Web Server
- **HTTP / FTP** — Web Server and File Server services
- **Email (SMTP/POP3)** — Email Server configuration
- **Trunk & Access Ports** — 802.1Q trunking on switch uplinks
- **WAN Link** — Serial connection between R1 and R2 (2911 routers)

---

## Project Files

```
enterprise-network-topology/
│
├── network_topology.pkt         # Cisco Packet Tracer simulation file
├── command_reference.doc        # All CLI commands used (routers & switches)
├── README.md                    # Project documentation
└── screenshots/
    └── topology_overview.png    # Network diagram screenshot
```

---

## How to Open

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (v8.0+ recommended)
2. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/enterprise-network-topology.git
   ```
3. Open `network_topology.pkt` in Cisco Packet Tracer
4. Refer to `command_reference.doc` for all configured CLI commands

---

## Features

- [x] Dual-office topology (Main + Branch)
- [x] VLAN segmentation per department
- [x] Inter-VLAN routing via L3 switches
- [x] WAN connectivity between offices via 2911 routers
- [x] Web, File, and Email server configuration
- [x] DHCP configured per VLAN
- [x] Full end-to-end connectivity verified with ping tests

---

## License

This project is submitted as part of the Computer Networks Lab course.
Free to use for educational and reference purposes.

---

> **CN Lab Project** — AIR University | Semester 4th | 2026
