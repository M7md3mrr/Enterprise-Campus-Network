<div align="center">

# 🏢 Enterprise Campus Network

### High Availability Enterprise Network using Cisco Packet Tracer

![Cisco](https://img.shields.io/badge/Cisco-Packet_Tracer-1BA0D7?style=for-the-badge&logo=cisco)
![CCNA](https://img.shields.io/badge/CCNA-Level-success?style=for-the-badge)
![Enterprise](https://img.shields.io/badge/Enterprise-Network-blue?style=for-the-badge)
![HSRP](https://img.shields.io/badge/HSRP-Enabled-red?style=for-the-badge)
![EtherChannel](https://img.shields.io/badge/EtherChannel-Configured-blueviolet?style=for-the-badge)
![VLAN](https://img.shields.io/badge/VLAN-Implemented-orange?style=for-the-badge)

### Designing a scalable, redundant, and highly available enterprise campus network using Cisco Layer 2 and Layer 3 switching technologies.

---

*"Reliable networks are not built by chance; they are built by design."*

</div>

---

# 📖 Project Overview

This project simulates a real-world **Enterprise Campus Network** using Cisco Packet Tracer.

The objective was to build a highly available network that integrates multiple Cisco networking technologies into one complete enterprise solution.

The network provides:

- High Availability
- Gateway Redundancy
- Link Redundancy
- Layer 2 Switching
- Layer 3 Routing
- Efficient VLAN Segmentation
- Enterprise Network Design

This project demonstrates how enterprise switches collaborate to provide continuous connectivity while minimizing downtime.

---

# 🎯 Project Objectives

- Design a scalable enterprise switching infrastructure.
- Separate departments using VLANs.
- Centralize VLAN management using VTP.
- Configure IEEE 802.1Q Trunk Links.
- Aggregate physical links using EtherChannel.
- Enable Inter-VLAN Routing.
- Eliminate the gateway single point of failure using HSRP.
- Build a redundant enterprise network.

---

# 🖥 Network Topology

![Topology](Images/topology.png)

---

# 🏗 Network Architecture

| Layer | Devices | Responsibilities |
|--------|----------|-----------------|
| Distribution Layer | Two Cisco Multilayer Switches | Inter-VLAN Routing, HSRP |
| Access Layer | Two Cisco Switches | VLAN Access, VTP, Trunking |

The multilayer switches provide Layer 3 routing and gateway redundancy using HSRP.

The access switches operate at Layer 2 and provide redundant paths using EtherChannel.

---

# 🌐 VLAN Design

| VLAN | Department | Network |
|------|------------|----------------|
| VLAN 2 | HR | 192.168.1.0/24 |
| VLAN 3 | Sales | 192.168.2.0/24 |
| VLAN 4 | Accounting | 192.168.3.0/24 |

---

# ⚙ Technologies Implemented

| Technology | Description |
|------------|-------------|
| VLAN | Logical network segmentation |
| VTP | Centralized VLAN management |
| IEEE 802.1Q | VLAN trunking |
| EtherChannel | Link aggregation and redundancy |
| Layer 3 Switching | Inter-VLAN Routing |
| HSRP | Default gateway redundancy |

---

# 🔹 VLAN Verification

The VLAN database was successfully configured and verified on the multilayer switches.

![SW1 VLAN](Images/sw1-vlan-brief.png)

![SW4 VLAN](Images/sw4-vlan-brief.png)

---

# 🔹 VTP Verification

VTP was configured to simplify VLAN administration across the network.

- VTP Server
- VTP Clients

![VTP Server](Images/sw4-vtp-status.png)

![VTP Client](Images/sw1-vtp-status.png)

---

# 🔹 Trunk Verification

IEEE 802.1Q trunk links successfully transport traffic for multiple VLANs between switches.

![Trunk](Images/trunk-links.png)

---

# 🔹 EtherChannel Verification

EtherChannel combines multiple physical interfaces into a single logical connection.

### Benefits

- Increased Bandwidth
- Link Redundancy
- Better Availability
- Simplified Management

![EtherChannel](Images/etherchannel-summary.png)

---

# 🔹 Inter-VLAN Routing

Layer 3 switching enables communication between hosts located in different VLANs.

The routing functionality was successfully verified through end-to-end connectivity tests.

![Routing](Images/inter-vlan-ping.png)

---

# 🔹 HSRP Verification

Hot Standby Router Protocol (HSRP) was configured to provide gateway redundancy.

### HSRP Roles

| Device | Role |
|---------|------|
| Left Multilayer Switch | Standby |
| Right Multilayer Switch | Active |

Clients use a single Virtual IP Address as their default gateway.

If the Active switch fails, the Standby switch automatically assumes the Active role.

![HSRP](Images/hsrp-status.png)

---

# 🔹 Redundancy Validation

The network was validated by testing redundant paths and gateway failover.

The implemented design ensures network availability while reducing the impact of device or link failures.

![Redundancy](Images/redundancy-test.png)

---

# ✅ Project Validation

| Test | Status |
|------|--------|
| VLAN Configuration | ✅ Passed |
| VTP Synchronization | ✅ Passed |
| Trunk Verification | ✅ Passed |
| EtherChannel | ✅ Passed |
| Inter-VLAN Routing | ✅ Passed |
| HSRP | ✅ Passed |
| Redundancy | ✅ Passed |

---

# 🎓 Skills Demonstrated

- Enterprise Network Design
- Cisco Switching
- Layer 2 Technologies
- Layer 3 Switching
- VLAN Configuration
- VTP Configuration
- EtherChannel Configuration
- HSRP Configuration
- Inter-VLAN Routing
- Network Troubleshooting
- High Availability Design

---

# 📂 Repository Structure

```text
Enterprise-Campus-Network
│
├── Images
│   ├── topology.png
│   ├── sw1-vlan-brief.png
│   ├── sw4-vlan-brief.png
│   ├── sw1-vtp-status.png
│   ├── sw4-vtp-status.png
│   ├── trunk-links.png
│   ├── etherchannel-summary.png
│   ├── hsrp-status.png
│   ├── inter-vlan-ping.png
│   └── redundancy-test.png
│
├── PacketTracer
│   └── Enterprise_Campus_Network.pkt
│
├── README.md
└── LICENSE
```

---

# 🚀 Future Improvements

Potential enhancements for future versions include:

- Dynamic Routing (OSPF)
- ACL Implementation
- Port Security
- DHCP Server Integration
- Rapid PVST+
- SSH Remote Management
- SNMP Monitoring
- Syslog Server
- NTP Configuration

---

# 👨‍💻 Author

## Mohamed Amr

**CCNA Certified**

Faculty of Computers and Artificial Intelligence

Cairo University

---

<div align="center">

### ⭐ Thank you for visiting this repository.

If you found this project helpful, consider giving it a ⭐.

*"Enterprise networks are not measured by speed alone, but by their ability to remain operational when failures occur."*

</div>
