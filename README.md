# 🕵️ ShadowTrace

> Automated Threat Hunting Lab powered by Python, Splunk, and MITRE ATT&CK

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Splunk](https://img.shields.io/badge/Splunk-Free-black?style=flat-square&logo=splunk)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=flat-square)
![Flask](https://img.shields.io/badge/Flask-Dashboard-green?style=flat-square&logo=flask)
![Streamlit](https://img.shields.io/badge/Streamlit-Visualization-ff4b4b?style=flat-square&logo=streamlit)
![VirusTotal](https://img.shields.io/badge/VirusTotal-API-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=flat-square)

---

## 📌 Overview

**ShadowTrace** is a personal cybersecurity lab designed to simulate, detect, and analyze real-world attack techniques using open-source tools. The project automates the entire threat hunting pipeline — from log ingestion and anomaly detection to real-time alerting and executive report generation — mapping every finding directly to the MITRE ATT&CK framework.

This lab was built to develop hands-on skills in:
- Threat hunting and log analysis
- Python-based security automation
- Incident detection and response
- MITRE ATT&CK technique mapping
- Machine learning applied to anomaly detection
- Real-time alerting and dashboard visualization

---

## 🏗️ Architecture

```
Kali Linux VM  →  Attack Simulation (Metasploit)
      ↓
   Log Generation
      ↓
Splunk (Log Ingestion & SIEM)
      ↓
Python Threat Detection Engine
  ├── Anomaly Detection (Machine Learning / sklearn)
  ├── MITRE ATT&CK Mapper
  ├── VirusTotal API (IP/Hash enrichment)
  └── Alert Engine (Email + Telegram)
      ↓
Streamlit Dashboard (Real-time visualization)
      ↓
Automated PDF Report
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
| T1071 | Application Layer Protocol | Command & Control |
| T1055 | Process Injection | Defense Evasion |

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| Kali Linux | Attack simulation environment |
| Metasploit Framework | Exploit and attack simulation |
| Splunk Free | Log ingestion and SIEM |
| Python 3.10+ | Threat detection automation |
| scikit-learn | Machine learning anomaly detection |
| Streamlit | Real-time threat dashboard |
| Flask | Web API for alert management |
| VirusTotal API | IP and hash enrichment |
| Telegram Bot API | Real-time threat alerts |
| MITRE ATT&CK | Threat intelligence framework |

---

## 📂 Project Structure

```
shadowtrace/
├── hunter/
│   ├── splunk_connector.py       # Splunk API integration
│   ├── threat_detector.py        # Core detection logic
│   ├── anomaly_detector.py       # ML-based anomaly detection (sklearn)
│   ├── mitre_mapper.py           # Maps findings to ATT&CK techniques
│   ├── virustotal_enricher.py    # VirusTotal IP/hash lookup
│   ├── alert_engine.py           # Email + Telegram alerts
│   └── report_generator.py       # Automated PDF report generation
├── dashboard/
│   └── app.py                    # Streamlit real-time dashboard
├── logs/
│   └── sample_logs/              # Sample log files for testing
├── reports/
│   └── sample_report.pdf         # Example output report
├── models/
│   └── anomaly_model.pkl         # Trained ML model
├── requirements.txt
└── README.md
```

---

## 📊 Dashboard Preview

> Real-time threat visualization built with Streamlit

- Live attack timeline
- MITRE ATT&CK heatmap
- Top suspicious IPs with VirusTotal enrichment
- Alert history and severity classification

---

## 🚨 Alert System

ShadowTrace sends real-time alerts when a threat is detected:

- **Email alerts** with attack summary and MITRE technique
- **Telegram Bot** notifications with severity level
- **PDF Report** auto-generated after each hunting session

---

## 🤖 Machine Learning Module

Uses **Isolation Forest** (scikit-learn) to detect behavioral anomalies in log data:

- Detects unusual login patterns (time, frequency, location)
- Flags abnormal network traffic volumes
- Identifies privilege escalation attempts
- Continuously improves with new log data

---

## 🚀 Roadmap

- [x] Lab architecture design
- [x] MITRE ATT&CK technique mapping
- [ ] Kali Linux + Splunk environment setup
- [ ] Attack simulation with Metasploit
- [ ] Python Splunk API connector
- [ ] Core threat detection engine
- [ ] Machine learning anomaly detector (Isolation Forest)
- [ ] MITRE ATT&CK mapper
- [ ] VirusTotal API enrichment
- [ ] Telegram + Email alert system
- [ ] Streamlit real-time dashboard
- [ ] Automated PDF report generator
- [ ] Flask API for alert management
- [ ] Full lab documentation with screenshots

---

## 👤 Author

**André Rogério Da Silva Filho**  
IT Support & Infrastructure Analyst | Cybersecurity Enthusiast  
[LinkedIn](https://linkedin.com/in/andré-silvaf) · [Email](mailto:andrerogeriofilho@outlook.com)

---

> *"The best defense starts with understanding the offense."*
