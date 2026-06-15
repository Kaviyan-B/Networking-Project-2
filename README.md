# Secure Multi-Branch Enterprise Network using OSPF, VLANs, ACLs, and Port Security

## 1. Project Overview

This project demonstrates the design and implementation of a secure multi-branch enterprise network using Cisco Packet Tracer. The topology connects a Headquarters (HQ) with two branch offices—Coimbatore and Madurai—through WAN serial links.

The network incorporates enterprise-grade technologies including dynamic routing, VLAN segmentation, inter-VLAN routing, branch isolation, and Layer 2 security.

---

## 2. Objectives

- Connect multiple branch offices to the headquarters.
- Implement dynamic routing using OSPF.
- Configure VLANs for departmental segmentation.
- Enable Inter-VLAN communication using Router-on-a-Stick.
- Restrict branch-to-branch communication using Extended ACLs.
- Secure switch ports using Port Security.
- Simulate a real-world enterprise network environment.

---

## 3. Network Topology

- **Headquarters (HQ)**
  - Multiple VLANs
  - Core Router
  - Two Layer 2 Switches
  - Servers

- **Coimbatore Branch**
  - Branch Router
  - Access Switch
  - End Devices

- **Madurai Branch**
  - Branch Router
  - Access Switch
  - End Devices

---

## 4. Technologies Used

- Cisco Packet Tracer
- OSPF (Open Shortest Path First)
- VLANs
- Inter-VLAN Routing
- Extended Access Control Lists (ACLs)
- Port Security
- Static IP Addressing
- WAN Serial Connections

---

## 5. IP Addressing Scheme

| Location | Network |
|----------|---------|
| HQ VLAN 10 | 192.168.10.0/24 |
| HQ VLAN 20 | 192.168.20.0/24 |
| Coimbatore Branch | 192.168.30.0/24 |
| Madurai Branch | 192.168.40.0/24 |
| HQ ↔ Coimbatore WAN | 10.0.0.0/30 |
| HQ ↔ Madurai WAN | 10.0.0.4/30 |

---

## 6. Routing Configuration

Dynamic routing is implemented using OSPF Area 0 across all routers.

### Features

- Automatic route learning
- Fast convergence
- Scalable enterprise routing
- Efficient WAN communication

---

## 7. VLAN Configuration

| VLAN ID | Department |
|--------|------------|
| 10 | Sales |
| 20 | HR |

### Benefits

- Broadcast domain separation
- Improved security
- Better network management

---

## 8. Security Features

### Extended ACLs

Branch-to-branch communication is blocked while allowing both branches to access HQ resources.

- Madurai ❌ Coimbatore
- Coimbatore ❌ Madurai
- Branches ✅ Headquarters

### Port Security

- Maximum MAC addresses: 1
- Violation Mode: Shutdown
- Sticky MAC enabled

---

## 9. Testing Results

| Test | Result |
|------|--------|
| HQ to Coimbatore | ✅ Success |
| HQ to Madurai | ✅ Success |
| Coimbatore to HQ | ✅ Success |
| Madurai to HQ | ✅ Success |
| Coimbatore to Madurai | ❌ Blocked |
| Madurai to Coimbatore | ❌ Blocked |

---



## 10. Skills Demonstrated

- Enterprise Network Design
- OSPF Configuration
- VLAN Implementation
- Router-on-a-Stick
- WAN Configuration
- Access Control Lists
- Port Security
- Network Troubleshooting

---

## 11 Learning Outcomes

This project provides hands-on experience in:

- Designing scalable enterprise networks
- Implementing routing protocols
- Securing network infrastructure
- Managing VLANs and WAN links
- Troubleshooting enterprise environments

---

## 📸 Screenshots
<img width="1734" height="711" alt="project 2" src="https://github.com/user-attachments/assets/57568ab7-705d-4fed-aa00-97056bb99c98" />
