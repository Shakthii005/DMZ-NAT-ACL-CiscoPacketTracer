# 🔐 Network Security Project: DMZ with ACL and NAT (Cisco Packet Tracer) with the help of ChatGpt

## Summary

This project demonstrates a secure network design using a **DMZ (Demilitarized Zone)**, **Access Control Lists (ACL)**, and **Network Address Translation (NAT)** to control and protect traffic between internal, external, and public-facing systems.

Built in **Cisco Packet Tracer**, this setup simulates real-world enterprise segmentation and traffic filtering, commonly used in secure networks.

---

## Objectives

- Isolate public-facing servers from the internal network using a **DMZ**
- Control traffic using **Access Control Lists**
- Mask internal IP addresses using **NAT (PAT)** for outbound access

---

## Network Topology

- **Router 2911**
  - G0/0: 192.168.1.1 (Internal LAN)
  - G0/1: 192.168.10.1 (DMZ)
  - G0/2: 192.168.20.1 (Internet/Outside)

- **Switch 2960** (one per segment)
- **Devices**
  - PC0: 192.168.1.2 (LAN user)
  - Web Server: 192.168.10.10 (DMZ)
  - Outside PC: 192.168.20.2 (Internet)

---

## Key Features

1. **DMZ Design:**  
Isolates the public web server from the internal network to reduce risk.

2. **ACLs:**  
- PC0 can access the web server via HTTP (port 80)
- DNS (port 53) access from LAN to DMZ is blocked
- ACLs applied inbound on internal interface (G0/0)

3. **NAT (PAT):**  
- Internal and DMZ IPs are translated to the router’s G0/2 IP
- Allows outbound traffic while keeping internal IPs hidden

---

## Skills Demonstrated

- Network segmentation and traffic control
- Realistic access control using ACLs
- NAT configuration using Cisco IOS commands
- Debugging packet loss and improving connectivity

---

## How to Open

1. Open `DMZ.pkt` in Cisco Packet Tracer
2. Verify interface configurations
3. Use provided command files to understand NAT and ACL setup

---

## Created By

**Shakthivel Rajesh**  
B.Tech Cybersecurity (3rd Year)  
Aspiring Network Security Engineer  

Built with support from **ChatGPT (OpenAI)** for guidance and technical explanation.

---

## Repository Files

| File | Description |
|------|-------------|
| `DMZ.pkt` | Main Cisco Packet Tracer project |
| `network_diagram.png` | Topology overview |
| `NAT-Configuration.txt` | NAT command setup |
| `ACL-and-DMZ-Rules.txt` | ACL configuration commands |
| `README.md` | Project explanation |

---

## Contact

📧 svelr005@gmail.com  
🔗 https://www.linkedin.com/in/svelr005/

