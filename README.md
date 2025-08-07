# Cyber Threat Intelligence (CTI) Automation and Sharing Platform

> A comprehensive and extensible platform for collecting, enriching, scoring, visualizing, and sharing cyber threat intelligence using STIX, TAXII, MISP, OpenAI, and PostgreSQL.

---

## 🔐 Project Summary

This CTI Automation and Sharing Proof of Concept (PoC) is built to demonstrate a real-world, research-backed implementation of Cyber Threat Intelligence sharing with automation, enrichment, and collaboration support. It integrates several threat sources, uses AI-assisted enrichment, enables STIX 2.x bundle handling, supports TAXII protocol, and includes a Bootstrap-powered frontend for analysts and researchers.

---

## ⚙️ Key Features

### 🧠 AI & Enrichment
- Automatic enrichment of threat indicators using OpenAI
- Entity tagging (malware families, techniques, actors)
- Threat scoring and classification

### 📡 CTI Integration
- Import from **MISP**, **MITRE ATT&CK**, **VirusTotal**, and other feeds
- Export as STIX bundles
- TAXII 2.1 API support for automated sharing

### 📊 Dashboard & Visualization
- STIX bundle analytics dashboard (indicators, tactics, trends)
- Threat statistics by time, source, and severity
- Bootstrap-powered responsive UI

### 🛡️ User Management
- Flask-Security for login, registration, and roles
- Admins, analysts, and viewers
- Session management and password reset

### 📄 Reporting
- PDF export of threat reports (STIX bundles or custom summaries)

---

## 🗂️ Project Structure

cti/
├── app/
│ ├── init.py
│ ├── routes/
│ │ ├── dashboard.py
│ │ ├── auth.py
│ │ └── api.py
│ ├── models/
│ │ └── stix_entities.py
│ ├── templates/
│ │ ├── dashboard.html
│ │ └── ...
│ └── static/
│ └── css/
├── scheduler/
│ └── fetch_from_misp.py
├── pdf_export/
│ └── report_generator.py
├── ai_enrichment/
│ └── enrich.py
├── taxii/
│ └── taxii_server.py
├── run.py
├── requirements.txt
├── .env
└── README.md