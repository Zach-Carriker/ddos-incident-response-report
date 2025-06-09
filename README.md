# ddos-incident-response-report

# 🚨 DDoS Incident Report & Analysis

This project documents the investigation and mitigation of a **Distributed Denial of Service (DDoS)** attack targeting a fictional organization's internal network. The report follows the **five core functions of the NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)** and provides actionable insights based on post-incident analysis.

---

## 📌 Summary of the Incident

- **Attack Type**: ICMP flood (DDoS attack)  
- **Impact**: Internal network was inaccessible for ~2 hours  
- **Initial Vector**: Unconfigured firewall allowed external ICMP traffic  
- **Response**: Blocked ICMP traffic, stopped non-critical services, restored core functionality

---

## 🛠 NIST CSF Breakdown

### 🕵️ Identify
- Discovered that ICMP flood traffic exploited an **unconfigured firewall**
- Attackers were able to overwhelm the network via a public-facing vulnerability

### 🔐 Protect
- Implemented firewall rules to limit ICMP packets
- Deployed **IDS/IPS** to monitor and block suspicious ICMP activity

### 📡 Detect
- Introduced **source IP verification** for incoming traffic
- Deployed new **network monitoring tools** to identify abnormal patterns

### 🚑 Respond
- Reconfigured affected firewall
- Provided team training on:
  - Configuration validation
  - Log analysis
- Instituted **end-of-day backup log policies**

### ♻️ Recover
- Restored lost data using backup procedures
- Updated end-user communication and recovery documentation
- Scheduled retraining on **restoration protocols**

---

## 🧠 Reflection

> “Working through each of the five NIST CSF functions gave me a clearer, more structured view of incident response. Breaking things down step-by-step made complex security incidents feel more manageable and helped me better understand the flow of professional security operations.”

---

## 📎 Supporting Document

- [📄 Incident_Report_Analysis.pdf](Incident_Report_Analysis.pdf)

This document includes the full incident report, technical analysis, mitigation efforts, and personal reflections on the exercise.

---

> 🗒️ *This project is based on a fictional incident and used for educational purposes.*
