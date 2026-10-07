# 0.1 — OSI & TCP/IP Models

**Date:** 2026-10-07 · **Blueprint:** foundation topic (not numbered, assumed everywhere) · **Quiz:** 8/8

## What is it?
Models that split network communication into **layers**, each with one job. Sending = data goes **down** the layers (7→1). Receiving = data goes **up** (1→7).

## Why layers?
- **Standardization** — different vendors interoperate
- **Independence** — change one layer (cable → Wi-Fi) without touching the others
- **Troubleshooting** — isolate problems layer by layer

## OSI model (7 layers)

| # | Layer | Job | Examples | Device | PDU |
|---|---|---|---|---|---|
| 7 | Application | Protocols apps use to talk | HTTP/S, DNS, DHCP, SMTP, FTP, SSH | — | Data |
| 6 | Presentation | Format, **encryption**, compression | JPEG, ASCII, MP4 | — | Data |
| 5 | Session | Open / maintain / close conversations | — | — | Data |
| 4 | **Transport** | Deliver to the right **application (port)**; segmentation; reliability | **TCP, UDP** | Firewall | **Segment** |
| 3 | **Network** | **Logical addressing (IP)** + **routing** between networks | IPv4, IPv6, ICMP, OSPF | **Router** | **Packet** |
| 2 | **Data Link** | Delivery to the **next device** using **MAC**; error detection (FCS); media access | Ethernet, 802.11 | **Switch**, AP | **Frame** |
| 1 | Physical | Send **bits** as electricity / light / radio | Cables, RJ45, fiber | Cables, hub | **Bits** |

🧠 1→7: **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way
🧠 PDUs 4→1: **S**ome **P**eople **F**ear **B**irthdays (Segment, Packet, Frame, Bits)

### Layer 4 detail
- **Port** = identifies the application inside a device (IP = building address, port = apartment number). → 1.5
- **TCP** = reliable (acknowledges, retransmits, ordered) — web, email, downloads
- **UDP** = fast, no acknowledgement — voice, video calls, gaming

### Layer 2 detail
- Frame carries the MAC of the **next hop only**, not the final destination.
- **FCS** (trailer) detects errors → bad frame is **discarded** (not retransmitted; TCP handles that).
- Media access: on shared media (Wi-Fi) devices take turns to avoid **collisions**. Full-duplex cabled links have no collisions. → 1.4, 1.11

## TCP/IP model (5 layers — used by Cisco)

| OSI | TCP/IP |
|---|---|
| 7 Application, 6 Presentation, 5 Session | 5 Application |
| 4 Transport | 4 Transport |
| 3 Network | 3 Network (called **Internet** in the old 4-layer model) |
| 2 Data Link | 2 Data Link |
| 1 Physical | 1 Physical |

Old 4-layer version merges L1+L2 into **Link / Network Access**.

## Encapsulation
- **Header** = info a layer adds in front · **Trailer** = info added at the end (only L2: **FCS**)
- **Encapsulation** = sender adds headers going down (7→1)
- **De-encapsulation** = receiver removes headers going up (1→7)

```
L4  [TCP hdr][data]                          → Segment
L3  [IP hdr][TCP hdr][data]                  → Packet
L2  [Eth hdr][IP hdr][TCP hdr][data][FCS]    → Frame
L1  0101101001...                            → Bits
```

> ⭐ Along the path: **destination IP stays the same**, **MAC addresses change at every hop** (each router builds a new frame).

## What went wrong?
Nothing in the quiz. Needed a simpler explanation of media access ("who talks now") and of what a PDU is.
