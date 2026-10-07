<div align="center">

# 🌐 CCNA Journey

### From zero to Cisco Certified Network Associate — documented day by day

![Cert](https://img.shields.io/badge/Cisco-CCNA%20200--301%20v1.1-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Status](https://img.shields.io/badge/Status-Studying-orange?style=for-the-badge)
![Exam](https://img.shields.io/badge/Target%20exam-Jan%2021%2C%202027-blueviolet?style=for-the-badge)

![Topics](https://img.shields.io/badge/Topics%20studied-2%20%2F%2054-success?style=flat-square)
![Labs](https://img.shields.io/badge/Labs%20done-0-lightgrey?style=flat-square)
![Days](https://img.shields.io/badge/Study%20days-1-blue?style=flat-square)

</div>

---

## 👋 About this repo

This is my public study journal for the **Cisco CCNA 200-301** exam.

Instead of just collecting a certificate, I'm documenting **every topic, every lab and every mistake** — so anyone can follow the process, and so I can prove I actually understand the material.

After the CCNA, this repo grows into a **hands-on home lab and cybersecurity journey**: a segmented network with VLANs, firewall rules, internal services and security monitoring.

---

## 📈 Progress

```
Network Fundamentals      ██░░░░░░░░░░░░░░░░░░   2 / 14
Network Access            ░░░░░░░░░░░░░░░░░░░░   0 / 9
IP Connectivity           ░░░░░░░░░░░░░░░░░░░░   0 / 5
IP Services               ░░░░░░░░░░░░░░░░░░░░   0 / 9
Security Fundamentals     ░░░░░░░░░░░░░░░░░░░░   0 / 10
Automation                ░░░░░░░░░░░░░░░░░░░░   0 / 7
```

**Starting point (self-assessment, day 1):** 0 🟢 confident · 13 🟡 rusty · 40 🔴 new

👉 Full checklist with every exam topic: **[CCNA-BLUEPRINT.md](CCNA-BLUEPRINT.md)**

---

## 🗓️ Timeline

```mermaid
gantt
    title CCNA 200-301 study plan
    dateFormat YYYY-MM-DD
    axisFormat %b %d
    section Fundamentals
    Network Fundamentals (20%)        :active, 2026-10-07, 2026-11-01
    section Switching
    Network Access (20%)              :2026-11-02, 2026-11-29
    section Routing & Services
    IP Connectivity + IP Services     :2026-11-30, 2026-12-27
    Security Fundamentals (15%)       :2026-12-28, 2027-01-03
    section Final stretch
    Automation (10%)                  :2027-01-04, 2027-01-10
    Practice exams & review           :2027-01-11, 2027-01-20
    CCNA exam                         :milestone, 2027-01-21, 0d
```

👉 Week-by-week plan: **[ROADMAP.md](ROADMAP.md)**

---

## 📚 Study notes

| # | Topic | Quiz |
|---|---|---|
| 0.1 | [OSI & TCP/IP models](network/00-osi-tcpip.md) | 8/8 |
| 1.1 | [Network components](network/01-network-components.md) | 7/8 |

👉 Daily log with what I studied and what went wrong: **[STUDY-LOG.md](STUDY-LOG.md)**

---

## 🧠 How I study

```
📖 Learn the topic  →  ❓ Quiz (exam-style, in English)  →  🧪 Lab in Packet Tracer  →  📝 Write a note  →  🔁 Review 2 weeks later
```

Every note answers the same questions ([template](documentation/TEMPLATE.md)):
**What is it? · How does it work? · Why does it matter? · How did I configure it? · What went wrong? · How did I fix it?**

The *"What went wrong?"* part is on purpose — mistakes are where the real learning happens.

---

## 🗂️ Repository structure

```
ccna-journey/
├── README.md              ← you are here
├── ROADMAP.md             ← week-by-week plan
├── CCNA-BLUEPRINT.md      ← every exam topic + progress
├── STUDY-LOG.md           ← daily journal
├── network/               ← study notes (one per topic)
├── packet-tracer/         ← lab files (.pkt)
├── diagrams/              ← topology diagrams
├── screenshots/           ← proof of configs & tests
├── documentation/         ← note template
├── linux/                 ← after the exam
└── cybersecurity/         ← after the exam
```

---

## 🛠️ Tools & resources

| | |
|---|---|
| 🧪 **Labs** | Cisco Packet Tracer |
| 📖 **Reading** | *CCNA 200-301 Official Cert Guide* (Wendell Odom), study-ccna.com |
| 🎥 **When stuck** | Jeremy's IT Lab |
| 🔁 **Memory** | Anki flashcards |
| 📝 **Practice exams** | Boson ExSim-Max (January) |

---

## 🚀 After the CCNA

- 🖥️ Physical lab: managed switch + mini PC with OPNsense
- 🔀 Segmented network: HOME · SERVERS · IoT · GUEST · MANAGEMENT VLANs
- 🔐 Firewall rules and access matrix between segments
- 🐧 Linux + OverTheWire Bandit
- 🌐 Web security with PortSwigger Web Security Academy
- 🎯 TryHackMe / Hack The Box

---

<div align="center">

⭐ *If you're also studying for the CCNA, feel free to follow along!*

</div>
