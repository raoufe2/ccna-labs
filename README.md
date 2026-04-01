# 🌐 CCNA 200-301 Lab Repository

[![CCNA](https://img.shields.io/badge/Cisco-CCNA%20200--301-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/associate/ccna.html)
[![Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-049fd9?style=for-the-badge&logo=cisco&logoColor=white)](https://www.netacad.com/courses/packet-tracer)
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)

> **Hands-on lab practice for Cisco CCNA 200-301 certification exam**

This repository contains practical network labs and configurations created during my CCNA preparation journey. All labs are designed to be run in **Cisco Packet Tracer** and cover key networking concepts tested in the CCNA exam.

---

## 📚 About This Repository

This repository serves as:
- ✅ **Study companion** for CCNA 200-301 exam preparation
- 🔬 **Hands-on practice** for networking concepts
- 📖 **Reference material** for network configurations
- 🎯 **Portfolio** demonstrating practical networking skills

**Target Audience:**
- CCNA certification candidates
- Networking students
- IT professionals seeking practical examples
- Anyone learning Cisco networking fundamentals

---

## 🗂️ Repository Structure

```
ccna-labs/
├── 01-network-fundamentals/
│   ├── cabling/
│   ├── tcp-udp/
│   └── osi-model/
├── 02-network-access/
│   ├── vlans/
│   ├── trunking/
│   ├── vtp/
│   ├── dtp/
│   ├── etherchannel/
│   └── wireless/
├── 03-ip-connectivity/
│   ├── static-routing/
│   ├── ospf/
│   ├── eigrp/
│   └── first-hop-redundancy/
├── 04-ip-services/
│   ├── nat-pat/
│   ├── dhcp/
│   ├── dns/
│   └── ntp/
├── 05-security-fundamentals/
│   ├── acls/
│   ├── port-security/
│   ├── dhcp-snooping/
│   └── aaa/
├── 06-automation/
│   ├── python-scripts/
│   ├── json-xml/
│   └── rest-api/
└── full-topology-labs/
    ├── campus-network/
    ├── branch-office/
    └── exam-scenarios/
```

---

## 🎯 Topics Covered

### ✅ Completed Labs

#### Network Access (Layer 2)
- [x] **VLANs** - VLAN creation, assignment, and verification
- [x] **Trunking** - 802.1Q trunk configuration and native VLAN
- [x] **VTP** - VLAN Trunking Protocol (Server, Client, Transparent modes)
- [x] **DTP** - Dynamic Trunking Protocol negotiation
- [x] **EtherChannel** - LACP, PAgP, and static port aggregation
- [x] **STP/RSTP** - Spanning Tree Protocol configuration and optimization
- [x] **Inter-VLAN Routing** - Router-on-a-Stick and Layer 3 switches

#### IP Connectivity (Layer 3)
- [x] **Static Routing** - IPv4/IPv6 static routes and default routes
- [x] **OSPF** - Single-area and multi-area OSPF configuration
- [x] **OSPF Advanced** - Network types, LSAs, authentication
- [x] **HSRP** - Hot Standby Router Protocol for gateway redundancy

#### Security
- [x] **Port Security** - MAC address limiting and violation modes
- [x] **DHCP Snooping** - Rogue DHCP server prevention
- [x] **STP Security** - BPDU Guard, Root Guard, Loop Guard

### 🔄 In Progress

- [ ] **ACLs** - Standard and Extended Access Control Lists
- [ ] **NAT/PAT** - Network Address Translation and Port Address Translation
- [ ] **DHCP** - Dynamic Host Configuration Protocol server configuration
- [ ] **IPv6** - IPv6 addressing, SLAAC, DHCPv6, OSPFv3
- [ ] **Automation** - Python scripting, REST APIs, JSON/XML

---

## 🚀 Getting Started

### Prerequisites

1. **Cisco Packet Tracer** (version 8.2 or later)
   - Download from: [Cisco NetAcad](https://www.netacad.com/courses/packet-tracer)
   - Free with Cisco NetAcad account

2. **Basic Networking Knowledge**
   - OSI/TCP-IP model
   - IP addressing and subnetting
   - Basic CLI commands

### How to Use These Labs

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ccna-labs.git
   cd ccna-labs
   ```

2. **Open labs in Packet Tracer:**
   - Navigate to the desired topic folder
   - Open the `.pkt` file in Cisco Packet Tracer
   - Read the accompanying `README.md` or `LAB-GUIDE.md` for instructions

3. **Follow the lab guide:**
   - Each lab includes:
     - 📋 **Objectives** - What you'll learn
     - 🗺️ **Topology diagram** - Network layout
     - 📝 **Step-by-step instructions** - Configuration tasks
     - ✅ **Verification commands** - How to test your work
     - 🎯 **Challenge tasks** - Additional practice (optional)

---

## 📖 Lab Format

Each lab directory contains:

```
topic-name/
├── topology.pkt              # Packet Tracer file (starting point)
├── topology-solution.pkt     # Complete configuration (solution)
├── README.md                 # Lab guide with instructions
├── configs/                  # Configuration files
│   ├── router1.txt
│   ├── switch1.txt
│   └── ...
└── diagrams/                 # Visual aids (optional)
    └── topology.png
```

---

## 🎓 Study Recommendations

### For Each Lab:

1. **Read the theory first** - Understand concepts before configuring
2. **Attempt without solution** - Try to configure from scratch
3. **Verify your work** - Use show commands to confirm
4. **Compare with solution** - Check differences and learn
5. **Repeat** - Redo labs until confident

### Suggested Order:

1. Start with **Network Access** (VLANs, Trunking, STP)
2. Move to **IP Connectivity** (Routing protocols)
3. Add **IP Services** (DHCP, NAT, ACLs)
4. Finish with **Security** and **Automation**
5. Practice **Full Topology Labs** before the exam

---

## 🔧 Useful Commands Reference

### Common Verification Commands

```cisco
! Show interface status
show ip interface brief
show interfaces status

! VLAN verification
show vlan brief
show interfaces trunk

! Routing verification
show ip route
show ip protocols
show ip ospf neighbor

! STP verification
show spanning-tree
show spanning-tree summary

! EtherChannel verification
show etherchannel summary
show etherchannel port-channel
```

### Configuration Backup

```cisco
! Save running config
copy running-config startup-config

! Export config (from Packet Tracer)
Right-click device > Export > Save As .txt
```

---

## 📚 Additional Resources

### Official Cisco Resources
- [CCNA 200-301 Exam Topics](https://learningnetwork.cisco.com/s/ccna-exam-topics)
- [Cisco Learning Network](https://learningnetwork.cisco.com/)
- [Cisco Documentation](https://www.cisco.com/c/en/us/support/index.html)

### Recommended Study Materials
- **Books:**
  - *CCNA 200-301 Official Cert Guide* by Wendell Odom
  - *31 Days Before Your CCNA Exam* by Allan Johnson

- **Video Courses:**
  - Jeremy's IT Lab (YouTube) - Free CCNA course
  - Neil Anderson - CCNA Complete Course (Udemy)
  - David Bombal - CCNA Lab Practice (YouTube)

- **Practice Platforms:**
  - [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
  - [GNS3](https://www.gns3.com/) - Advanced network emulation
  - [Cisco Modeling Labs](https://learningnetworkstore.cisco.com/cisco-modeling-labs-personal) (CML)

---

## 🤝 Contributing

Contributions are welcome! If you have:
- 🐛 **Found a bug** in a lab configuration
- 💡 **Suggestions** for new labs or improvements
- 📝 **Better explanations** or documentation

Please:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-lab`)
3. Commit your changes (`git commit -m 'Add new ACL lab'`)
4. Push to the branch (`git push origin feature/new-lab`)
5. Open a Pull Request

---

## 📝 Notes

- All configurations are tested in **Cisco Packet Tracer 8.2+**
- Some advanced features may not be available in Packet Tracer (use GNS3 for production-like environments)
- Configurations follow Cisco best practices but are simplified for learning purposes
- Real production networks require additional security and optimization

---

## ⚖️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

You are free to:
- ✅ Use these labs for personal study
- ✅ Modify and adapt for your needs
- ✅ Share with other CCNA students
- ❌ Claim as your own work
- ❌ Use for commercial purposes without attribution

---

## 📧 Contact

**Abderaouf Touati**
- 🌐 GitHub: [@yourusername](https://github.com/yourusername)
- 💼 LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- 📧 Email: your.email@example.com

---

## 🎯 CCNA Exam Preparation Checklist

- [ ] Complete all Network Fundamentals labs
- [ ] Master VLANs, Trunking, and STP
- [ ] Configure OSPF multi-area networks
- [ ] Implement HSRP/VRRP for redundancy
- [ ] Configure and troubleshoot ACLs
- [ ] Implement NAT/PAT for internet connectivity
- [ ] Set up DHCP server and relay
- [ ] Configure IPv6 addressing and routing
- [ ] Practice full topology scenarios
- [ ] Take practice exams (score 85%+ consistently)
- [ ] Schedule CCNA exam

---

## 🌟 Acknowledgments

- **Cisco NetAcad** - For Packet Tracer and learning resources
- **Jeremy's IT Lab** - Excellent free CCNA video course
- **r/ccna Community** - Support and study tips
- **All contributors** - Thank you for improving these labs!

---

## 📊 Repository Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/ccna-labs?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/ccna-labs?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/yourusername/ccna-labs?style=social)

---

<div align="center">

**⭐ If you find this repository helpful, please consider giving it a star! ⭐**

*Good luck with your CCNA certification journey!* 🚀

</div>
