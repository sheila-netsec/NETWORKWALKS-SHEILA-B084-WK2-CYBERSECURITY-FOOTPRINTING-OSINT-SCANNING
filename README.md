# NETWORKWALKS-SHEILA-B084-WK2-CYBERSECURITY-FOOTPRINTING-OSINT-SCANNING

Cybersecurity & Ethical Hacking internship project — Week 2 (Networkwalks, Batch B084).

This repository documents four Week 2 modules covering the footprinting / OSINT
phase and the active network scanning phase of a penetration testing engagement,
performed against course-assigned, authorized targets and my own local network.

## ⚠️ Scope & Authorization

All activities were performed strictly within an educational, authorized scope:

- `networkwalks.com` and `microsoft.com` were course-assigned targets used for
  **passive, public-source information gathering only** (WHOIS, DNS, HTTP headers,
  public OSINT sources). No system was accessed, modified, or exploited.
- Active host-discovery scanning (Zenmap/Nmap) was run **only against my own home
  LAN**, which I own.

This work is for education and research purposes only. See the full liability
disclaimer in [`Final-Report/W2-Final_Combined_Report.pdf`](./Final-Report).

## 📁 Repository Structure

| Folder | Module | Tool(s) | Summary |
|---|---|---|---|
| [`W2-PM1-Kali-Tools`](./W2-PM1-Kali-Tools) | W2-PM1 | whois, whatweb, nslookup, curl, wafw00f, dnsrecon | Command-line footprinting of networkwalks.com |
| [`W2-PM3-Maltego`](./W2-PM3-Maltego) | W2-PM3 | Maltego Graph | Graph-based OSINT — email addresses linked to networkwalks.com |
| [`W2-PM4-theHarvester`](./W2-PM4-theHarvester) | W2-PM4 | theHarvester | Automated OSINT — emails, sub-domains and IPs for microsoft.com |
| [`W2-PM5-Zenmap`](./W2-PM5-Zenmap) | W2-PM5 | Zenmap (Nmap GUI) | Active host discovery on my own home LAN |
| [`Final-Report`](./Final-Report) | — | — | Combined pentest-style report covering all four modules |

## 🔑 Key Findings (high level)

- **W2-PM1:** Identified hosting provider, DNS posture (open recursion, unsigned
  DNSSEC), exact CMS/plugin versions, and an active WAF (ModSecurity).
- **W2-PM3:** Linked two email addresses to the target domain via Maltego transforms,
  distinguishing an organisational contact from a registrar contact.
- **W2-PM4:** theHarvester surfaced 868 sub-domains and 3 role-based email addresses
  for microsoft.com using only free, keyless OSINT sources.
- **W2-PM5:** Discovered 3 live hosts on my home LAN via a ping scan, with IP/MAC
  identification and a topology diagram.

Full findings, a consolidated risk table, and recommendations are in the
[final report](./Final-Report).

## 🛠️ Tools Used

Kali Linux · WHOIS · WhatWeb · Nslookup · Curl · Wafw00f · DNSRecon ·
Maltego Graph (Desktop) · theHarvester · Zenmap (Nmap GUI) · Windows CMD

## 👤 Author

**Sheila Chepkoech**
Cybersecurity Professional — B084, Networkwalks
[LinkedIn](https://www.linkedin.com/in/sheila-chepkoech-b59b902b4)

---
*Educational project — Networkwalks Cybersecurity & Ethical Hacking program.*
