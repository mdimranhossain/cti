# 🛡️ Cyber Threat Intelligence (CTI) Automation & Sharing - PoC

A full-featured Proof-of-Concept (PoC) platform for Cyber Threat Intelligence (CTI) automation, enrichment, sharing, and analytics. Designed to demonstrate secure, intelligent, and scalable CTI management through integration with MISP, TAXII, AI/NLP, and STIX format with multi-user access.

---

## 📌 Features

✅ CTI Data Ingestion & STIX Bundle Generation  
✅ TAXII 2.1 Server Integration  
✅ MISP Integration using PyMISP  
✅ AI-Powered Threat Enrichment (OpenAI or local NLP)  
✅ Threat Scoring Algorithm with Visual Dashboards  
✅ Role-Based Access Control using Flask-Security  
✅ Multi-user Authentication and Session Management  
✅ Export CTI Reports as PDF  
✅ PostgreSQL Database  
✅ Job Scheduler for Automated Feeds  
✅ Docker Support & `.env` Configuration  
✅ Frontend built with Bootstrap for Analysts

---

## 🔧 Tech Stack

| Layer         | Technologies Used                                      |
|--------------|--------------------------------------------------------|
| Backend      | Python, Flask, Flask-SQLAlchemy, Flask-Security        |
| Frontend     | Bootstrap, jQuery, Chart.js                            |
| Database     | PostgreSQL                                             |
| CTI Exchange | MISP, TAXII (cabby, medallion)                         |
| AI Enrichment| OpenAI API or spaCy/NLTK for NLP tagging               |
| Auth System  | Flask-Security with roles: Admin, Analyst, Viewer      |
| Export       | ReportLab for PDF export                               |
| Deployment   | Docker + CPanel (manual), VPS supported                |

---

## 📁 Project Structure

```bash
cti/
├── app/
│   ├── __init__.py
│   ├── routes/
│   ├── models/
│   ├── templates/
│   ├── static/
│   └── utils/
├── migrations/
├── instance/
│   └── config.py
├── .env
├── run.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── README.md
└── .gitignore