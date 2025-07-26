# 🔐 DMZ with NAT and ACL Configuration Project

## 📌 Summary
This project demonstrates a secure network design using a **DMZ (Demilitarized Zone)**, **Access Control Lists (ACLs)**, and **Network Address Translation (NAT)** to regulate and protect traffic between internal, external, and public-facing zones.

Built in **Cisco Packet Tracer**, the setup simulates a real-world enterprise network environment with **segmentation, NAT, and access control**, commonly used in federal and enterprise networks.

---

## 🎯 Objectives

- Isolate public-facing services from internal users using a DMZ
- Apply ACLs to restrict access between network segments
- Use NAT (PAT) to enable secure outbound internet access
- Simulate federal-grade traffic control using NIST-aligned concepts

---

## 🖥️ Network Topology

**Router 2911 Configuration:**

| Interface | IP Address | Zone |
|-----------|------------|------|
| G0/0 | 192.168.1.1 | Internal LAN |
| G0/1 | 192.168.10.1 | DMZ |
| G0/2 | 192.168.20.1 | Internet/Outside |

**Switches:** One Cisco 2960 switch per segment

**Devices:**

| Device | IP | Role |
|--------|----|------|
| PC0 | 192.168.1.2 | Internal LAN user |
| Web Server | 192.168.10.10 | DMZ server |
| Outside PC | 192.168.20.2 | Simulated Internet host |

---

## 🧭 Framework Alignment

### 🔹 NIST Cybersecurity Framework (CSF)

| Function | Project Implementation |
|----------|------------------------|
| **Identify** | Defined network segments and critical assets (DMZ, LAN, External) |
| **Protect** | Enforced ACLs and NAT for access control |
| **Detect** | Packet loss troubleshooting and connectivity tests |
| **Respond** | Access denied defaults and control logic built in |
| **Recover** | Backup configs and simulation reset included |

---

### 🔹 NICE Framework Roles

| Role Title | Code | Description |
|------------|------|-------------|
| Network Operations Specialist | OM-NET-001 | Implement and manage secure network configurations |
| Technical Support Specialist | OM-TEE-001 | Troubleshoot and maintain network systems |

---


## 🔧 Key Features

- **DMZ Design**: Public web server is isolated from internal users
- **ACL Implementation**:
  - PC0 can access the web server (port 80)
  - DNS (port 53) from LAN to DMZ is explicitly blocked
  - ACLs applied **inbound on G0/0**
- **NAT (PAT)**:
  - Internal and DMZ IPs translated to G0/2 (outside interface)
  - Enables secure outbound access and hides internal IPs

---

## 🧪 Skills Demonstrated

- VLAN/DMZ-based segmentation
- ACL configuration for precise access control
- NAT setup using Cisco IOS (PAT)
- Network security testing and packet flow validation
- Federal framework awareness (NICE, CSF, 800-53)

---

## 🗂️ Repository Files

| File | Description |
|------|-------------|
| `DMZ.pkt` | Main Cisco Packet Tracer project |
| `network_diagram.png` | Visual topology |
| `NAT-Configuration.txt` | NAT IOS configuration commands |
| `ACL-and-DMZ-Rules.txt` | ACL setup for access control |
| `README.md` | Project explanation and documentation |

---

## 🧠 How to Use

1. Open `DMZ.pkt` in Cisco Packet Tracer
2. Load interface configurations
3. Review `NAT-Configuration.txt` and `ACL-and-DMZ-Rules.txt` to understand the rule sets
4. Test connectivity from:
   - PC0 → Web Server (HTTP allowed)
   - PC0 → DNS (should be blocked)
   - Outside PC → Internal (should be blocked)

---

## 📎 About Me

👤 **Shakthivel Rajesh**  
🎓 B.Tech Cybersecurity (3rd Year)  
🎯 Aspiring Network Security Engineer | SFS Candidate (Fall 2027)  

📧 svelr005@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/svelr005/)  

Built with support from **ChatGPT (OpenAI)** for technical guidance and framework alignment.

