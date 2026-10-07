# 1.1 — Network Components

**Date:** 2026-10-07 · **Blueprint:** 1.1 (+ intro to 1.7) · **Quiz:** 7/8

## What is it?
The devices that make up a network and the role each one plays.

## Key concepts
- **LAN** = local network (home, office, building). **WAN** = connects distant sites (→ 1.2).
- **Layer 2** = communication inside the same LAN, uses **MAC addresses**, unit = **frame**.
- **Layer 3** = communication between different networks, uses **IP addresses**, unit = **packet**.
- **Unicast** (one) · **Broadcast** (everyone on the LAN) · **Multicast** (a group).
- **Broadcast domain** = the set of devices that receive the same broadcast. Switches forward broadcasts; **routers block them**.

## Devices

| Device | Layer | What it does |
|---|---|---|
| **Endpoint** | — | Source/destination of data (PC, phone, printer, IP camera, IP phone) |
| **Server** | — | Endpoint that provides a service (web, DNS, DHCP, file, email) |
| **Switch (L2)** | 2 | Connects devices **in the same LAN**; forwards frames by **MAC**; many ports; one broadcast domain by default |
| **Router (L3)** | 3 | Connects **different networks** (not only the Internet); forwards packets by **IP** using the routing table; separates broadcast domains |
| **L3 / multilayer switch** | 2+3 | Switch that also routes (between VLANs) in hardware; many ports, fewer WAN features (NAT, VPN) |
| **Firewall** | 3–4 | Filters traffic with rules; **stateful** (return traffic allowed, outside-initiated blocked); zones: inside / outside / **DMZ** |
| **NGFW** | 3–7 | Firewall + **application awareness** + **integrated IPS** + **URL filtering** + **malware protection** |
| **IPS** | — | **Inline**, matches attack **signatures**, **blocks** |
| **IDS** | — | Gets a **copy** of traffic, **alerts only** |
| **Access Point (AP)** | 2 | Connects wireless clients to the wired network; wired to a switch; broadcasts SSIDs |
| **WLC** | — | Centrally manages many (**lightweight**) APs: config, channels, power, SSIDs, roaming (→ 2.6, 2.7) |

> ⭐ **Switch = same network (MAC) · Router = between networks (IP)**

## PoE (Power over Ethernet)
- **PSE** (Power Sourcing Equipment) = provides power → usually the **switch**
- **PD** (Powered Device) = receives power → AP, IP phone, IP camera
- Switch has a total **power budget**

| Standard | Name | Max power |
|---|---|---|
| 802.3af | PoE | 15.4 W |
| 802.3at | PoE+ | 30 W |
| 802.3bt | UPoE / PoE++ | 60 W / 100 W |

## Private IPv4 (RFC 1918) — preview of 1.7
| Range | From – To |
|---|---|
| 10.0.0.0/8 | 10.0.0.0 – 10.255.255.255 |
| 172.16.0.0/12 | 172.**16**.0.0 – 172.**31**.255.255 |
| 192.168.0.0/16 | 192.168.0.0 – 192.168.255.255 |

⚠️ `172.32.x.x` is **public**. Special: `127.0.0.0/8` loopback · `169.254.0.0/16` APIPA (DHCP failed).

## Why is it important?
Every other topic builds on knowing which device does what. Exam asks "which device fits this scenario?" and IPS vs IDS.

## What went wrong?
- Quiz Q1: said the router is "for the Internet" → it connects **any** different networks.
- Quiz Q7: missed that `172.20.1.1` is private.

## Real-world example
A home "router" = router + switch + AP + basic firewall + DHCP server in one box. In a company, each is a separate device.
