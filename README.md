# 🔐 Vendmo Tech — Cybersecurity Audit & Risk Assessment Report

![Security](https://img.shields.io/badge/Security-Audit-red?style=flat-square)
![Framework](https://img.shields.io/badge/Framework-NIST%20CSF-blue?style=flat-square)
![Standard](https://img.shields.io/badge/Standard-ISO%2027001%3A2022-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Final%20Report-green?style=flat-square)
![Version](https://img.shields.io/badge/Version-v1.0-lightgrey?style=flat-square)

---

## 📋 Overview

This repository contains a comprehensive **Cybersecurity Audit and Risk Assessment Report** for **Vendmo Tech** — a fictional mid-sized South African fintech company. The project was designed to demonstrate real-world security auditing skills, from threat identification through to prioritised remediation recommendations.

The report simulates a professional security engagement covering network infrastructure, web applications, identity management, data protection, and operational security practices.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `VendmoTech_Security_Audit_Report.docx` | Full security audit report (Word format) |
| `README.md` | This file |

---

## 📚 What's Inside the Report

The report is structured across **10 sections** and **3 appendices**:

| Section | Content |
|---------|---------|
| 1. Executive Summary | High-level risk overview, key findings, regulatory exposure |
| 2. Company Overview | Asset inventory, user categories, business context |
| 3. Methodology | Tools used, audit phases, frameworks applied |
| 4. Risk Assessment | Threat landscape, 5×5 risk matrix, risk register (10 risks) |
| 5. Audit Findings | Auth, network, web app, data protection, and ops security findings |
| 6. Vulnerability Findings | 14 vulnerabilities with CVSS scores, descriptions, and deep-dives |
| 7. Framework Mapping | NIST CSF + ISO 27001 Annex A control mapping for all findings |
| 8. Recommendations | 12 actionable recommendations in a 3-track remediation roadmap |
| 9. Conclusion | Final risk rating, compliance status, next steps |
| Appendices | Glossary, references, sign-off table |

---

## 🛠️ Tools & Frameworks Referenced

### Security Frameworks
- **NIST Cybersecurity Framework (CSF) v1.1** — Identify, Protect, Detect, Respond, Recover
- **ISO/IEC 27001:2022** — Information Security Management (Annex A controls)
- **OWASP Top 10 (2021)** — Web application vulnerability classification
- **CIS Controls v8** — Supporting reference for hardening guidance
- **PCI-DSS v4.0** — Payment card security compliance
- **POPIA (Act 4 of 2013)** — South African data privacy regulation

### Security Tools Used in the Audit
| Tool | Purpose |
|------|---------|
| **OWASP ZAP 2.14** | Web application vulnerability scanning (active & passive) |
| **Nmap 7.94** | Network discovery, port scanning, OS/version detection |
| **Wireshark 4.2** | Network traffic capture and plaintext data analysis |
| **Nessus 10.6** | Host-based vulnerability scanning |
| **Burp Suite Pro** | Manual web application testing and traffic interception |
| **Metasploit 6.3** | Controlled exploitation for proof-of-concept verification |
| **Active Directory Audit** | IAM review and privilege enumeration |

---

## 🚨 Key Findings Summary

| Severity | Count | Examples |
|----------|-------|---------|
| 🔴 **Critical** | 3 | No MFA, Unpatched Apache RCE (CVE-2021-41773), Plaintext PII storage |
| 🟠 **High** | 4 | SQL Injection, Default switch credentials, Data over HTTP, Firewall misconfiguration |
| 🟡 **Medium** | 5 | Missing HTTP headers, No patch management, Excessive privileges, No SIEM |
| 🟢 **Low** | 2 | Self-signed certs, No incident response plan |

**Overall Risk Rating: 🔴 HIGH**

---

## 🗺️ Remediation Roadmap

### Track 1 — Immediate (0–14 Days)
- Deploy MFA across all systems
- Patch Apache (CVE-2021-41773) within 24–48 hours
- Encrypt Customer PII database (AES-256)
- Enforce HTTPS/TLS 1.3, remediate SQL Injection

### Track 2 — Short-Term (15–60 Days)
- Harden firewall and network devices
- Implement RBAC and least privilege
- Deploy SIEM and centralised logging
- Launch security awareness training

### Track 3 — Strategic (61–180 Days)
- Initiate ISO 27001:2022 certification
- PCI-DSS self-assessment
- Implement DevSecOps pipeline (SAST/DAST)
- Deploy DLP tooling, conduct annual penetration test

---

## 🏢 About the Fictional Company

**Vendmo Tech** is a simulated fintech company used as the audit subject:
- **Industry:** Peer-to-peer payments & merchant gateway
- **Location:** Johannesburg, South Africa
- **Employees:** ~240 staff
- **Customers:** ~85,000 registered users
- **Monthly Volume:** ~R 120 million in transactions
- **Regulatory Scope:** POPIA, PCI-DSS, ISO 27001

> ⚠️ **Disclaimer:** Vendmo Tech is a fictional company created solely for educational and portfolio purposes. All vulnerabilities, findings, and data in this report are simulated. No real systems were tested.

---

## 🎯 Project Purpose

This project was built to demonstrate:
- Real-world security auditing and reporting methodology
- Risk assessment using industry-standard frameworks
- Vulnerability identification and CVSS scoring
- Practical mitigation strategy development
- Professional technical report writing

---

## 📄 Licence

This project is intended for educational and portfolio use. Feel free to use it as a reference or template for your own security audit work.

---

*Report Version: v1.0 — March 2026 | Information Security Department*
