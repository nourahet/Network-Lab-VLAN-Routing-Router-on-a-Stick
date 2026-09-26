# 🌐 Inter-VLAN Routing via Router-on-a-Stick (Cisco Packet Tracer) 🚀

![Network Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge&logo=checkmarx)
![Cisco Packet Tracer](https://img.shields.io/badge/Simulator-Cisco%20Packet%20Tracer-005691?style=for-the-badge&logo=cisco)
![IEEE 802.1Q](https://img.shields.io/badge/Protocol-IEEE%20802.1Q-orange?style=for-the-badge)

---

## 🎯 Project Purpose & Objectives

This laboratory project demonstrates the implementation of **VLAN segmentation** across a multi-floor enterprise infrastructure and configures **Inter-VLAN routing** using the **Router-on-a-Stick (ROAS)** architectural model.

By leveraging Cisco sub-interfaces on a single physical link (`Gig0/0`), devices on isolated virtual networks (**VLAN 10 - Marketing** and **VLAN 11 - RH**) distributed across two different physical floors can seamlessly communicate while maintaining strict logical boundaries.

---

## 🏢 Network Topologies & Architectures

### 📸 1. Cisco Packet Tracer Topology
Below is the physical topology implemented inside Cisco Packet Tracer, displaying the two-floor switch distribution and single router connection:

<p align="center">
  <img
    width="511"
    height="316"
    alt="Network Architecture"
    src="https://github.com/user-attachments/assets/b300d95b-2c82-4220-86c6-f97a23570072"
  />
</p>


---

### 🎨 2. High-Level Modern Logical Diagram
The diagram below highlights the logical trunk connections, sub-interface configurations, and VLAN boundaries:

<p align="center">
  <img
    width="800"
    alt="Network Architecture Diagram"
    src="https://github.com/user-attachments/assets/0d34a013-02a3-456a-a14f-6bb591beef29"
  />
</p>


---

## 📊 Addressing & VLAN Scheme

| 🏢 Floor | 💻 Host Device | 🏷️ VLAN | 🌐 IP Address / Subnet | 🚪 Default Gateway | 🔌 Switch Port |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Floor 1** | `PC0` | **VLAN 10** (Marketing) | `192.168.1.3/24` | `192.168.1.1` | `SWITCH01 Fa0/2` |
| **Floor 1** | `Laptop0` | **VLAN 11** (RH) | `192.168.2.3/24` | `192.168.2.1` | `SWITCH01 Fa0/3` |
| **Floor 2** | `PC1` | **VLAN 10** (Marketing) | `192.168.1.4/24` | `192.168.1.1` | `SWITCH02 Fa0/2` |
| **Floor 2** | `Laptop1` | **VLAN 11** (RH) | `192.168.2.4/24` | `192.168.2.1` | `SWITCH02 Fa0/3` |

---
