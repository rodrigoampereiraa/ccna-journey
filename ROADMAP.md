# 🧭 Roadmap — CCNA 200-301 by the end of January

**Period:** Oct 7, 2026 → Jan 31, 2027 (17 weeks, ~2h/day ≈ 240h)
**Exam:** target **Thu, Jan 21, 2027** → if it goes wrong, Cisco allows a retake after 5 days → retake possible on **Jan 27–29**, still before the deadline.
**⛔ Hard deadline:** CCNA v1.1 retires on **Feb 2, 2027**. From Feb 3 it's v2.0 (new AI domain, ~28% troubleshooting, study materials still immature). No room to postpone.
**Method:** theory → lab → documentation → flashcards.

> ⚠️ 240h is enough but **tight** when starting from scratch. Extra hours on weekends (3h Sat/Sun) are the safety margin. Cybersecurity (Bandit, PortSwigger, OPNsense, Raspberry Pi) moves to **after the exam**.

---

## 📚 Resources

| Resource | Use | Cost |
|---|---|---|
| **CCNA 200-301 Official Cert Guide, Vol. 1 & 2** (Wendell Odom, Cisco Press, v1.1 edition) | **Main written material.** Follows the blueprint chapter by chapter | ~€50–60 each (ebook cheaper) |
| **study-ccna.com** | Free written alternative, organized by topic | Free |
| **Jeremy's IT Lab** (YouTube) | **Only when the written material isn't clear** | Free |
| **Anki** | Daily flashcards | Free |
| **Boson ExSim-Max for CCNA** | Practice exams in January (closest to the real thing) | ~$100 |
| CCNA 200-301 exam (Pearson VUE) | Online or at a test center | ~$300 |

| Domain | Weight | When |
|---|---|---|
| 1. Network Fundamentals | 20% | October |
| 2. Network Access (VLANs, STP, Wireless) | 20% | November |
| 3. IP Connectivity (routing, OSPF, FHRP) | 25% | December |
| 4. IP Services (NAT, DHCP, NTP, SNMP, QoS...) | 10% | December |
| 5. Security Fundamentals | 15% | Dec/Jan |
| 6. Automation & Programmability | 10% | January |

---

## 📅 Typical week

| Day | Focus |
|---|---|
| Mon | 📖 Theory (reading; video only if stuck) |
| Tue | 🧪 Packet Tracer (topic lab) |
| Wed | 📖 Theory |
| Thu | 🧪 Packet Tracer |
| Fri | 🔁 Review: Anki + topic quiz + subnetting |
| Sat | 🧪 Bigger lab / physical switch (3h if possible) |
| Sun | 📝 Documentation + weekly review |

**Every day, 15 min:** Anki + 2 subnetting exercises (subnettingpractice.com).

---

## ⚡ How to use this plan

Every topic gets covered, but not with the same time. Before each topic, check the color it got in [CCNA-BLUEPRINT.md](CCNA-BLUEPRINT.md):

| Color | What to do | Time |
|---|---|---|
| 🟢 Know it | Quick read → lab without notes → flashcards | 1–2 days |
| 🟡 Rusty | Read → lab → note | 2–3 days |
| 🔴 Don't know | Full study: read + 2 labs + detailed note | 3–5 days |

**Golden rule:** 🟢 only counts if you can **configure it without notes**. The exam asks for commands and `show` outputs.

**Self-assessment result (Oct 7):** 0 🟢 · 13 🟡 · 40 🔴 → the plan runs **at normal pace, no shortcuts**. All 53 exam topics are covered below.

---

## 🟦 Phase 0 — Setup + self-assessment (Oct 7–11)

- [x] Self-assess every topic in [CCNA-BLUEPRINT.md](CCNA-BLUEPRINT.md)
- [ ] Install Packet Tracer (free Cisco Networking Academy account)
- [ ] Install Anki
- [x] Set up Git
- [ ] Create the GitHub repo and first push
- [ ] **Book the exam NOW (by end of October) at Pearson VUE for ~Jan 21** — January slots will fill up with everyone rushing v1.1 before Feb 2. Rescheduling is free up to 48h before.

---

## 🟩 OCTOBER — Network Fundamentals (20%)

### Week 1 · Oct 7–11 — Kickoff
- [x] 📖 1.1 Network components (router, switch, firewall, AP, WLC, endpoints, servers, PoE)
- [x] 📖 0.1 OSI & TCP/IP models
- [ ] 📖 1.2 Topology architectures: 2-tier, 3-tier, spine-leaf, WAN, SOHO, on-prem vs cloud
- [ ] 🧪 PT: 2 PCs + switch, `ping`
- [x] 📝 `network/01-network-components.md` · `network/00-osi-tcpip.md`

### Week 2 · Oct 12–18 — Layers 1 & 2
- [ ] 📖 Cables (UTP, SMF/MMF fiber), interfaces, errors (duplex, speed, collisions)
- [ ] 📖 Ethernet, MAC, MAC address table, ARP
- [ ] 🧪 PT: Simulation mode — ARP and MAC table (`show mac address-table`)
- [ ] 📝 `network/02-ethernet-mac-arp.md`

### Week 3 · Oct 19–25 — IPv4 + Subnetting
- [ ] 📖 IPv4, private ranges (RFC 1918), mask, gateway
- [ ] 📖 Subnetting + VLSM
- [ ] 📖 Basic IOS CLI (modes, `running-config`, `startup-config`, `show ip interface brief`)
- [ ] 🧪 PT: `PC ── Switch ── Router ── PC`, two networks
- [ ] 🎯 Subnetting: a /27 in your head in < 30 s
- [ ] 📝 `network/03-ipv4-subnetting.md`

### Week 4 · Oct 26 – Nov 1 — IPv6 + Transport
- [ ] 📖 IPv6: format, abbreviation, global unicast, link-local, unique local, multicast, anycast, EUI-64, SLAAC
- [ ] 📖 TCP vs UDP, common ports, ICMP
- [ ] 📖 Virtualization: VMs, containers, VRFs
- [ ] 📖 Wireless principles: non-overlapping 2.4 GHz channels, SSID, RF
- [ ] 🧪 PT: IPv6 on routers and PCs
- [ ] 📝 `network/04-ipv6-tcp-udp.md`

### 🎯 October checkpoint
- [ ] Explain in writing: **"What happens when 192.168.1.10 communicates with 192.168.2.10?"**
- [ ] 20 subnetting exercises in a row without errors

---

## 🟨 NOVEMBER — Network Access (20%)

### Week 5 · Nov 2–8 — VLANs & Trunks
- [ ] 📖 VLANs, access, trunk, 802.1Q, native VLAN, voice VLAN, DTP, VTP
- [ ] 🧪 PT: 1 switch, VLAN 10/20/30
- [ ] 🖥️ Buy a switch (recommended: **used Cisco Catalyst 2960**, ~€30–60 — same CLI as the exam)
- [ ] 📝 `network/05-vlans-trunks.md`

### Week 6 · Nov 9–15 — Inter-VLAN + Discovery
- [ ] 📖 Router-on-a-stick, SVIs on an L3 switch
- [ ] 📖 CDP and LLDP
- [ ] 🧪 PT: Router + Switch + VLAN 10 USERS / 20 SERVERS / 30 IT working
- [ ] 📝 `network/06-inter-vlan-cdp-lldp.md`

### Week 7 · Nov 16–22 — STP
- [ ] 📖 STP, root bridge, port roles/states, RSTP, PortFast, BPDU Guard
- [ ] 🧪 PT: 3 switches in a triangle — predict and confirm root bridge and blocked port
- [ ] 🖥️ Physical switch: console access, real VLANs
- [ ] 📝 `network/07-stp-rstp.md`

### Week 8 · Nov 23–29 — EtherChannel + Wireless
- [ ] 📖 EtherChannel (LACP, PAgP, static)
- [ ] 📖 Wireless: architectures (autonomous, cloud, WLC-based / lightweight), AP modes, CAPWAP, WLC connections (ports, LAG, interfaces)
- [ ] 🧪 PT: LACP EtherChannel; WLC + AP + WPA2-PSK WLAN via GUI
- [ ] 📝 `network/08-etherchannel-wireless.md`

### 🎯 November checkpoint
- [ ] Rebuild the November VLAN topology from scratch, no notes, in < 45 min
- [ ] Confirm the exam is booked (~Jan 21) and check retake availability for Jan 27–29

---

## 🟧 DECEMBER — IP Connectivity (25%) + IP Services (10%)

### Week 9 · Nov 30 – Dec 6 — Routing
- [ ] 📖 Routing table (protocol code, prefix, mask, next hop, AD, metric, gateway of last resort)
- [ ] 📖 Longest prefix match, administrative distance
- [ ] 📖 IPv4 and IPv6 static routes: default, network, host, floating
- [ ] 🧪 PT: 3 routers, static routes only, IPv4 + IPv6
- [ ] 📝 `network/09-static-routing.md`

### Week 10 · Dec 7–13 — OSPFv2
- [ ] 📖 Single-area OSPF: neighbors, adjacencies, point-to-point, broadcast (DR/BDR), router ID, cost
- [ ] 🧪 PT: replace static routes with OSPF; `show ip ospf neighbor`, `show ip route ospf`
- [ ] 📝 `network/10-ospf.md`

### Week 11 · Dec 14–20 — FHRP + ACLs + NAT
- [ ] 📖 FHRP (HSRP, VRRP/GLBP concepts)
- [ ] 📖 Standard/extended ACLs, numbered/named
- [ ] 📖 Static NAT, pool, PAT
- [ ] 🧪 PT: ACL USERS ✗ IT; PAT to the "Internet"
- [ ] 📝 `network/11-fhrp-acl-nat.md`

### Week 12 · Dec 21–27 — IP Services (light week, Christmas)
- [ ] 📖 NTP, DHCP (+ relay `ip helper-address`), DNS
- [ ] 📖 SNMP, Syslog (severity levels!), QoS (classification, marking, queuing, policing/shaping)
- [ ] 📖 SSH, TFTP/FTP
- [ ] 🧪 PT: NTP + Syslog + DHCP relay
- [ ] 📝 `network/12-ip-services.md`

### Week 13 · Dec 28 – Jan 3 — Security Fundamentals (15%)
- [ ] 📖 Threats, vulnerabilities, exploits, mitigation; awareness programs
- [ ] 📖 Passwords, MFA, certificates, biometrics; AAA (RADIUS vs TACACS+)
- [ ] 📖 VPNs (site-to-site, remote access, IPsec)
- [ ] 📖 Port security, DHCP snooping, Dynamic ARP Inspection
- [ ] 📖 WPA, WPA2, WPA3
- [ ] 🧪 PT: port security + DHCP snooping + DAI; SSH with local user
- [ ] 📝 `network/13-security-fundamentals.md`

---

## 🟥 JANUARY — Automation + Exam

### Week 14 · Jan 4–10 — Automation & Programmability (10%)
- [ ] 📖 Traditional vs controller-based networking; SDN (underlay, overlay, fabric, northbound/southbound APIs)
- [ ] 📖 Catalyst Center (DNA Center) vs traditional management
- [ ] 📖 REST APIs (CRUD, HTTP verbs, encoding), JSON
- [ ] 📖 Ansible, Terraform; AI/ML in network operations
- [ ] 🧪 **Practice exam #1** (Boson) → list the 3 weakest domains
- [ ] 📝 `network/14-automation.md`

### Week 15 · Jan 11–17 — Weak spots
- [ ] Review weak domains from practice exam #1
- [ ] 🧪 Speed labs: VLANs + trunk + OSPF + ACL + NAT in one topology
- [ ] 🧪 **Practice exams #2 and #3**
- [ ] Target: > 85% on Boson before the exam

### Week 16 · Jan 18–24 — 🎯 EXAM
- [ ] Mon–Tue: light review, Anki, subnetting
- [ ] Wed: rest / very light review
- [ ] **Thu Jan 21: CCNA 200-301 EXAM**
- [ ] If online: test the Pearson VUE system in advance (webcam, empty room, ID)

### Week 17 · Jan 25–31 — Buffer
- [ ] ✅ Passed → update README and LinkedIn
- [ ] ❌ Didn't pass → review the score report by domain and retake on **Jan 27–29**

---

## 🧭 After the exam (February →)

1. **Physical lab:** Mini PC + OPNsense, VLANs 10 HOME / 20 SERVERS / 30 IoT / 40 GUEST / 99 MGMT, access matrix
2. **Linux** + OverTheWire Bandit
3. **Server:** Raspberry Pi / Mini PC with Docker, Pi-hole/AdGuard, WireGuard
4. **PortSwigger:** HTTP → Authentication → Access Control → SQLi → XSS → CSRF → SSRF → File Upload → API → JWT
5. Python → TryHackMe / Hack The Box → Pentesting
