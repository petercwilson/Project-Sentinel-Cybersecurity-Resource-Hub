# 🛡️ Project Sentinel: Cybersecurity Resource Hub

A curated collection of tools, cheat sheets, and learning paths for the modern security researcher. This repository is designed to bridge the gap between "beginner" and "practitioner."

---

## 📑 Table of Contents
* [Learning Paths & Certifications](#-learning-paths--certifications)
* [Offensive Security (Red Teaming)](#-offensive-security-red-teaming)
* [Defensive Security (Blue Teaming)](#-defensive-security-blue-teaming)
* [Cheat Sheets & Payloads](#-cheat-sheets--payloads)
* [Labs & Practice Environments](#-labs--practice-environments)
* [Contributing](#-contributing)

---

## 🎓 Learning Paths & Certifications
Resources for structured learning and industry-recognized credentials.

* **The OSI Model Revisited** - A deep dive into networking fundamentals for security.
* **CompTIA Security+ Roadmap** - My personal notes and study guide for the SY0-701 exam.
* **OSCP Preparation** - A curated list of "TJ Null" style boxes.

---

## 🚩 Offensive Security (Red Teaming)
Tools and techniques for penetration testing and ethical hacking.

* **Reconnaissance:**
    * [Nmap Cheat Sheet](./Network-Security/nmap_cheatsheet.md) - Common flags for stealth and aggressive scanning.
    * [Subfinder](https://github.com/projectdiscovery/subfinder) - Fast passive subdomain enumeration tool.
* **Web Exploitation:**
    * [OWASP Top 10 Checklist](./Web-App-Sec/owasp_checklist.md) - A manual testing guide for web vulnerabilities.
    * [Burp Suite Tips](./Web-App-Sec/burp_pro_tips.md) - Automating repetitive tasks with intruder and extender.

### 🛠️ Essential Offensive Tools (2026)
| Tool | Category | Key Use Case |
| :--- | :--- | :--- |
| **[Nuclei](https://github.com/projectdiscovery/nuclei)** | Vuln Scanner | Template-based scanning for the latest CVEs. |
| **[Sliver](https://github.com/BishopFox/sliver)** | C2 Framework | Modern, Go-based Command & Control for red teaming. |
| **[BloodHound](https://github.com/BloodHoundAD/BloodHound)** | AD Enumeration | Mapping attack paths in Active Directory via Graph Theory. |
| **[Feroxbuster](https://github.com/epi052/feroxbuster)** | Fuzzing | Ultra-fast recursive directory/file discovery. |
| **[Caido](https://caido.io/)** | Web Proxy | Lightweight, high-performance alternative to Burp Suite. |

---

## 🛡️ Defensive Security (Blue Teaming)
Focusing on detection, response, and hardening.

* **Incident Response:**
    * [The Incident Response Hierarchy](./Blue-Teaming/IR_steps.md) - A step-by-step guide from detection to recovery.
* **SIEM & Logging:**
    * [Splunk Search Cheat Sheet](https://example.com) - Essential SPL queries for hunting threats.

---

## 📝 Cheat Sheets & Payloads
*Quick-access files for the heat of the moment.*

| Category | Resource Link | Description |
| :--- | :--- | :--- |
| **Linux** | [Linux-PrivEsc.md](./Scripts/privesc.md) | Common paths for local privilege escalation. |
| **SQLi** | [SQL-Injection-Payloads.txt](./Web-App-Sec/sqli.txt) | Auth bypass and error-based payloads. |
| **Reverse Shells** | [One-Liners.md](./Scripts/shells.md) | Python, Bash, and PHP reverse shell commands. |

---

## 🏗️ Labs & Practice Environments
Where to legally break things.

* **[TryHackMe](https://tryhackme.com)** - Gamified learning for all levels.
* **[HackTheBox](https://www.hackthebox.com)** - Advanced "Capture The Flag" style machines.
* **[VulnHub](https://www.vulnhub.com)** - Offline VMs for local practice.

---

## 🤝 Contributing
Contributions are welcome! Please read the `CONTRIBUTING.md` file for details on our code of conduct and the process for submitting pull requests.

## ⚖️ Disclaimer
*This repository is for educational purposes only. Unauthorized access to computer systems is illegal. Always obtain written permission before testing any network or application.*
