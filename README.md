# 🕵️ ShadowTrace

> Automated Threat Hunting Lab powered by Python, Splunk, and MITRE ATT&CK

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Splunk](https://img.shields.io/badge/Splunk-Free-black?style=flat-square&logo=splunk)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=flat-square)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=flat-square)

---

## 📌 Overview

**ShadowTrace** is a personal cybersecurity lab designed to simulate, detect, and analyze real-world attack techniques using open-source tools. The project automates the process of log ingestion, threat detection, and report generation — mapping findings directly to the MITRE ATT&CK framework.

This lab was built to develop hands-on skills in:
- Threat hunting and log analysis
- Python-based security automation
- Incident detection and response
- MITRE ATT&CK technique mapping

---

## 🏗️ Architecture

```
Kali Linux VM  →  Attack Simulation (Metasploit)
      ↓
   Log Generation
      ↓
Splunk (Log Ingestion & Search)
      ↓
Python Script (Threat Detection Engine)
      ↓
Automated PDF Report (MITRE ATT&CK Mapped)
```

---

## 🔍 Attack Techniques Simulated

| Technique ID | Name | Tactic |
|---|---|---|
| T1110 | Brute Force | Credential Access |
| T1046 | Network Service Scanning | Discovery |
| T1078 | Valid Accounts | Defense Evasion |
| T1059 | Command and Scripting Interpreter | Execution |
| T1003 | OS Credential Dumping | Credential Access |

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| Kali Linux | Attack simulation environment |
| Metasploit Framework | Exploit and attack simulation |
| Splunk Free | Log ingestion and SIEM |
| Python 3.10+ | Threat detection automation |
| MITRE ATT&CK | Threat intelligence framework |

---

## 📂 Project Structure

```
shadowtrace/
├── hunter/
│   ├── splunk_connector.py     # Splunk API integration
│   ├── threat_detector.py      # Detection logic
│   ├── mitre_mapper.py         # Maps findings to ATT&CK
│   └── report_generator.py     # Generates PDF report
├── logs/
│   └── sample_logs/            # Sample log files for testing
├── reports/
│   └── sample_report.pdf       # Example output report
├── requirements.txt
└── README.md
```

---

## 🚀 Roadmap

- [x] Lab architecture design
- [x] MITRE ATT&CK technique mapping
- [ ] Kali Linux + Splunk environment setup
- [ ] Attack simulation with Metasploit
- [ ] Python Splunk API connector
- [ ] Threat detection engine
- [ ] MITRE ATT&CK mapper
- [ ] Automated PDF report generator
- [ ] Dashboard visualization

---

## 👤 Author

**André Rogério Da Silva Filho**  
IT Support & Infrastructure Analyst | Cybersecurity Enthusiast  
[LinkedIn](https://linkedin.com/in/andré-silvaf) · [Email](mailto:andrerogeriofilho@outlook.com)

---

> *"The best defense starts with understanding the offense."*
