# ✅ CCNA 200-301 — Blueprint Checklist

Every official exam topic. When everything is checked, nothing is missing.

> This list follows **v1.1**, valid until **Feb 2, 2027**.

**Columns:**
- **Before** — self-assessment on day 1, *before* studying: 🟢 can explain & configure · 🟡 seen it, rusty · 🔴 never seen / don't know
- **Studied** · **Lab** (configured in Packet Tracer) · **Reviewed** (still know it 2+ weeks later)
- "Describe/Explain" topics have no lab → `—`

---

## 0. Foundation topics (not numbered in the blueprint, but assumed throughout the exam)

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 0.1 | OSI & TCP/IP models: layers, PDUs, encapsulation | 🔴 | [x] | — | [ ] |

## 1.0 Network Fundamentals (20%) — October

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 1.1 | Network components: routers, L2/L3 switches, NGFW & IPS, APs, controllers (WLC), endpoints, servers, PoE | 🟡 | [x] | — | [ ] |
| 1.2 | Topology architectures: 2-tier, 3-tier, spine-leaf, WAN, SOHO, on-premise and cloud | 🔴 | [ ] | — | [ ] |
| 1.3 | Physical interfaces and cabling: single-mode fiber, multimode fiber, copper; shared media vs point-to-point | 🔴 | [ ] | — | [ ] |
| 1.4 | Interface and cable issues: collisions, errors, duplex and speed mismatch | 🔴 | [ ] | [ ] | [ ] |
| 1.5 | TCP vs UDP | 🟡 | [ ] | — | [ ] |
| 1.6 | Configure and verify IPv4 addressing and subnetting | 🟡 | [ ] | [ ] | [ ] |
| 1.7 | Private IPv4 addressing | 🟡 | [ ] | — | [ ] |
| 1.8 | Configure and verify IPv6 addressing and prefix | 🔴 | [ ] | [ ] | [ ] |
| 1.9 | IPv6 address types: global unicast, unique local, link-local, anycast, multicast, modified EUI-64 | 🔴 | [ ] | [ ] | [ ] |
| 1.10 | Verify IP parameters on Windows, macOS, Linux | 🟡 | [ ] | [ ] | [ ] |
| 1.11 | Wireless principles: non-overlapping channels, SSID, RF, encryption | 🔴 | [ ] | — | [ ] |
| 1.12 | Virtualization fundamentals: VMs, containers, VRFs | 🔴 | [ ] | — | [ ] |
| 1.13 | Switching concepts: MAC learning and aging, frame switching, flooding, MAC address table | 🔴 | [ ] | [ ] | [ ] |

## 2.0 Network Access (20%) — November

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 2.1 | VLANs across multiple switches: access ports (data and voice), default VLAN, inter-VLAN connectivity | 🟡 | [ ] | [ ] | [ ] |
| 2.2 | Interswitch connectivity: trunks, 802.1Q, native VLAN | 🟡 | [ ] | [ ] | [ ] |
| 2.3 | Layer 2 discovery protocols: CDP and LLDP | 🔴 | [ ] | [ ] | [ ] |
| 2.4 | L2/L3 EtherChannel (LACP) | 🔴 | [ ] | [ ] | [ ] |
| 2.5 | Rapid PVST+: root bridge (primary/secondary), root port, port roles and states, PortFast, Root Guard, Loop Guard, BPDU Filter, BPDU Guard | 🔴 | [ ] | [ ] | [ ] |
| 2.6 | Cisco wireless architectures and AP modes | 🔴 | [ ] | — | [ ] |
| 2.7 | WLAN physical infrastructure: AP, WLC, access/trunk ports, LAG | 🔴 | [ ] | — | [ ] |
| 2.8 | Device management access: Telnet, SSH, HTTP/HTTPS, console, TACACS+/RADIUS, cloud managed | 🔴 | [ ] | — | [ ] |
| 2.9 | WLC GUI: WLAN creation, security settings, QoS profiles, advanced settings | 🔴 | [ ] | [ ] | [ ] |

## 3.0 IP Connectivity (25%) — December

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 3.1 | Routing table: protocol code, prefix, mask, next hop, AD, metric, gateway of last resort | 🔴 | [ ] | [ ] | [ ] |
| 3.2 | Forwarding decision: longest prefix match, AD, metric | 🔴 | [ ] | — | [ ] |
| 3.3 | IPv4 and IPv6 static routing: default, network, host, floating static | 🔴 | [ ] | [ ] | [ ] |
| 3.4 | Single-area OSPFv2: adjacencies, point-to-point, broadcast (DR/BDR), router ID | 🔴 | [ ] | [ ] | [ ] |
| 3.5 | First hop redundancy protocols (HSRP, VRRP, GLBP) | 🔴 | [ ] | — | [ ] |

## 4.0 IP Services (10%) — December

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 4.1 | Inside source NAT: static and pools (+ PAT) | 🟡 | [ ] | [ ] | [ ] |
| 4.2 | NTP client and server mode | 🔴 | [ ] | [ ] | [ ] |
| 4.3 | Role of DHCP and DNS | 🟡 | [ ] | — | [ ] |
| 4.4 | SNMP | 🔴 | [ ] | — | [ ] |
| 4.5 | Syslog: facilities and severity levels (0–7) | 🔴 | [ ] | — | [ ] |
| 4.6 | DHCP client and relay | 🟡 | [ ] | [ ] | [ ] |
| 4.7 | QoS per-hop behavior: classification, marking, queuing, congestion, policing, shaping | 🔴 | [ ] | — | [ ] |
| 4.8 | Remote access with SSH | 🔴 | [ ] | [ ] | [ ] |
| 4.9 | TFTP/FTP | 🔴 | [ ] | — | [ ] |

## 5.0 Security Fundamentals (15%) — Dec/Jan

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 5.1 | Threats, vulnerabilities, exploits, mitigation | 🔴 | [ ] | — | [ ] |
| 5.2 | Security program: user awareness, training, physical access control | 🔴 | [ ] | — | [ ] |
| 5.3 | Device access control with local passwords | 🔴 | [ ] | [ ] | [ ] |
| 5.4 | Password policies: management, complexity, MFA, certificates, biometrics | 🔴 | [ ] | — | [ ] |
| 5.5 | IPsec remote access and site-to-site VPNs | 🔴 | [ ] | — | [ ] |
| 5.6 | Access control lists | 🟡 | [ ] | [ ] | [ ] |
| 5.7 | Layer 2 security: DHCP snooping, DAI, port security | 🔴 | [ ] | [ ] | [ ] |
| 5.8 | AAA: authentication, authorization, accounting | 🟡 | [ ] | — | [ ] |
| 5.9 | WPA, WPA2, WPA3 | 🔴 | [ ] | — | [ ] |
| 5.10 | Configure a WLAN in the GUI with WPA2-PSK | 🔴 | [ ] | [ ] | [ ] |

## 6.0 Automation & Programmability (10%) — January

| # | Topic | Before | Studied | Lab | Reviewed |
|---|---|---|---|---|---|
| 6.1 | How automation impacts network management | 🔴 | [ ] | — | [ ] |
| 6.2 | Traditional vs controller-based networking | 🔴 | [ ] | — | [ ] |
| 6.3 | SDN: overlay, underlay, fabric | 🔴 | [ ] | — | [ ] |
| 6.4 | AI (generative and predictive) and machine learning in network operations | 🔴 | [ ] | — | [ ] |
| 6.5 | REST APIs: authentication, CRUD, HTTP verbs, data encoding | 🔴 | [ ] | — | [ ] |
| 6.6 | Ansible and Terraform | 🔴 | [ ] | — | [ ] |
| 6.7 | JSON components | 🔴 | [ ] | — | [ ] |

---

## 🚫 Not on the exam

Not part of 200-301 v1.1, so not in the plan: EIGRP, RIP, multi-area OSPF, VTP in depth, PPP/HDLC/Frame Relay, BGP.
