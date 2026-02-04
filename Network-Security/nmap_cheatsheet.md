Since **Nmap** (Network Mapper) is the "Swiss Army Knife" of cybersecurity, it's the perfect first content file for your `/Network-Security` folder. It demonstrates that your repo provides immediate, practical value.

Create a file named `nmap_cheatsheet.md` and paste this in:

---

# 🔍 Nmap Discovery & Scanning Cheat Sheet

Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses.

## 🚀 The "Big Three" Scans

These are the most common starting points for any engagement.

* **Stealth Scan (Default):** `$ nmap -sS <target>`
* *Why:* Fast and relatively unobtrusive; it doesn't complete the 3-way TCP handshake.


* **Service Version Detection:** `$ nmap -sV <target>`
* *Why:* Probes open ports to determine what software and version are actually running.


* **Default Script Scan:** `$ nmap -sC <target>`
* *Why:* Runs a collection of safe, helpful scripts to find common vulnerabilities.



---

## 🛠️ Tactical Flags

| Flag | Action | Use Case |
| --- | --- | --- |
| `-O` | **OS Detection** | Attempts to identify the operating system of the target. |
| `-p-` | **All Ports** | Scans all 65,535 ports instead of just the top 1,000. |
| `-T4` | **Aggressive Timing** | Speeds up the scan (use `T5` for labs, `T2` for stealth). |
| `-Pn` | **No Ping** | Skips host discovery; assumes the target is online (bypasses ICMP blocks). |
| `-oN` | **Normal Output** | Saves results to a standard text file for your report. |

---

## 🧪 Advanced One-Liners

### 1. The "Standard Enumeration"

A solid balance of speed and depth.

```bash
nmap -sV -sC -T4 -oN initial_scan.txt <target_ip>

```

### 2. Vulnerability Scanning

Uses the Nmap Scripting Engine (NSE) to check for known CVEs.

```bash
nmap --script vuln <target_ip>

```

### 3. Fast UDP Scan

UDP is often overlooked but hosts critical services like DNS (53) and SNMP (161).

```bash
nmap -sU -T4 --top-ports 20 <target_ip>

```

---

## ⚠️ Important Note

**TCP 3-Way Handshake Logic:**
Nmap's `-sS` (SYN scan) works by sending a SYN packet. If the port is open, the target sends SYN/ACK. Nmap then sends an **RST** (Reset) instead of an ACK to terminate the connection before it's fully established, which is why it's called a "half-open" scan.

---

**Would you like me to show you how to set up the GitHub Action I mentioned earlier to automatically check for broken links in your repo?**