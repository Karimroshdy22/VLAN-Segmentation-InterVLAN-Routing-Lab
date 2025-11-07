# VLAN Segmentation & Inter-VLAN Routing Lab

## 🔍 Overview
This lab demonstrates how to configure VLAN segmentation, inter-VLAN routing using the **Router-on-a-Stick** method, and VLAN isolation using **Access Control Lists (ACLs)**.

The topology was created in **Cisco Packet Tracer**, and it includes:
- 1 Router (Cisco 1941)
- 1 Switch (Cisco 2960)
- 10 PCs divided into 5 VLANs

---

## 🧠 Objectives
- Configure VLANs on a Layer 2 Switch.
- Implement Inter-VLAN routing using sub-interfaces on a Router.
- Assign static IPs to PCs within each VLAN.
- Apply ACLs to isolate specific VLANs (VLAN 30 & VLAN 40).

---

## 🧩 Topology
<img width="1316" height="690" alt="Topology" src="https://github.com/user-attachments/assets/a63ecbd3-8fb5-41d5-8c86-1bb84d4f5144" />


---

## ⚙️ Devices Configuration

### 🔸 VLAN Configuration on Switch
See full configuration in [`switch-config.txt`]().

### 🔸 Router Sub-interfaces & ACLs
See full configuration in [`router-config.txt`]().

---

## 🧾 IP Addressing Plan
| VLAN | Department | Network | Gateway | PCs Range |
|------|-------------|----------|----------|------------|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 | 192.168.10.2–192.168.10.3 |
| 20 | DEV | 192.168.20.0/24 | 192.168.20.1 | 192.168.20.2–192.168.20.3 |
| 30 | Research | 192.168.30.0/24 | 192.168.30.1 | 192.168.30.2–192.168.30.3 |
| 40 | PR | 192.168.40.0/24 | 192.168.40.1 | 192.168.40.2–192.168.40.3 |
| 50 | Finance | 192.168.50.0/24 | 192.168.50.1 | 192.168.50.2–192.168.50.3 |

---

## 🚫 VLAN Isolation
- VLANs 30 and 40 are **isolated** from all other VLANs using **ACLs**.
- Other VLANs can communicate normally.

---

## 👨‍💻 Project by
**Name:** Karim Roshdy Mousa  
**Bootcamp:** WE Innovate SOC  
**Track:** Cybersecurity – SOC Analyst  
**Tool Used:** Cisco Packet Tracer 
