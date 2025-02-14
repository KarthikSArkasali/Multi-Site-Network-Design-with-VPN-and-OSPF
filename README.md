# 🌐 Multi-Site Network Design with VPN, and OSPF

## 🚀 Project Overview
    This project simulates a multi-site enterprise network with advanced routing, redundancy, and security mechanisms. The network spans Site A and Site B, using VLANs for segmentation, OSPF 
    for dynamic routing, HSRP for redundancy, and a site-to-site VPN for secure communication.


# 📌 Key Features

🔹 **VLAN Trunking** – Efficient segmentation of network traffic

🔹 **HSRP (Hot Standby Router Protocol)** – Redundancy for uninterrupted connectivity

🔹 **OSPF (Open Shortest Path First)** – Dynamic routing for optimal path selection

🔹 **Site-to-Site VPN (GRE over IPsec)** – Secure encrypted communication

🔹 **NAT (Network Address Translation)** – Secure internet access for internal networks


# 🖥️ Network Topology


![Project](https://github.com/user-attachments/assets/871baf79-f445-4d9d-8a94-b4ac30357cf6)

# 🛠️ Configuration Steps

1️⃣ **VLAN and Trunking Configuration**

- Created VLANs 10, 20, and 30 for network segmentation
- Configured trunk ports between distribution and core switches
- Assigned VLANs to respective access-layer switches

2️⃣ **OSPF Routing Setup**

- Enabled OSPF process for dynamic routing between routers
- Configured network statements for proper route advertisement
- Optimized OSPF with cost values for best path selection


3️⃣ **HSRP Configuration (Redundant Gateway)**

- Assigned Virtual IP for gateway redundancy
- Configured priority and preemption for active router failover


4️⃣ **GRE Tunnel (VPN) Implementation**

- Created Tunnel interfaces on both Site A and Site B routers
- Assigned GRE IPs: 172.16.1.1/30 & 172.16.1.2/30
- Routed internal subnets over the GRE tunnel


5️⃣ **NAT Setup for Internet Access**

- Configured NAT for translating private IPs to public IPs
- Allowed clients to access the internet securely

# 🎯 Key Learnings

- Configuring enterprise-grade network infrastructure
- Implementing redundancy & failover using HSRP
- Securing site-to-site communication with VPN
- Optimizing routing with OSPF and NAT
