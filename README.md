
# 🛡️ SOC Task 2 – Security Alert Monitoring & Incident Response Simulation

### 👨‍💻 Intern: Jagadeesh Kommineni  
### 📅 Date: June 28, 2025

---

## 📌 Project Overview

This project simulates the day-to-day responsibilities of a Security Operations Center (SOC) analyst. The goal was to monitor security alerts, analyze suspicious activity, and simulate an incident response workflow using real SIEM (Security Information and Event Management) tooling — specifically, the Elastic Stack (ELK).

Logs included authentication events, malware alerts, system activities, and network traffic. Key findings were documented in a professional incident response report.

---

## 🛠️ Tools & Environment

| Tool                 | Description                                                |
|----------------------|------------------------------------------------------------|
| **Kali Linux**       | Linux environment used for SIEM setup                      |
| **Docker**           | Containerized ELK deployment                               |
| **Elastic Stack**    | Open-source SIEM for log ingestion, storage, and visualization |
| **Kibana**           | Web UI for query, visualization, and dashboard creation    |
| **Python**           | Used to create synthetic logs for malware, auth, and network |
| **Visual Studio Code** | Used for editing code, queries, and documentation         |

---

## 📂 Project Structure

```
SOC-Task2/
│
├── logs/                          # Simulated log data (auth, malware, network)
├── docker-compose.yml            # Docker stack configuration for ELK
├── incident-report.docx          # Final incident report (IR)
├── screenshots/                  # Screenshots from Kibana & alerts
├── README.md                     # This file
└── kibana_saved_objects.ndjson   # Saved visualizations and dashboards
```

---

## 🧠 What I Learned

- **Log Analysis**: Parsing, querying, and pattern matching using Kibana  
- **SIEM Operation**: Data indexing, dashboard building, alert filtering  
- **Threat Identification**: Brute force attacks, malware detection, network scans  
- **Incident Response Simulation**: Severity classification, escalation prep, and remediation steps  
- **Documentation & Communication**: Drafted and structured a technical IR report like a real SOC analyst  

---

## 🧪 Steps to Reproduce

1. **Install Docker** on Kali Linux (if not already installed)

2. **Deploy ELK Stack**  
   ```bash
   docker network create elk
   docker-compose up -d
   ```

3. **Verify Access**  
   - Elasticsearch: [http://localhost:9200](http://localhost:9200)  
   - Kibana: [http://localhost:5601](http://localhost:5601)

4. **Import Logs**  
   Upload simulated logs to Elasticsearch using a Python script or manually via Kibana.

5. **Analyze Data in Kibana**  
   - Use *Discover* tab to query logs  
   - Create visualizations and dashboards

6. **Identify Suspicious Events**  
   - Filter by `log_type: malware_alert`, `auth_failure`, or high connection count

7. **Write Report**  
   - Document alerts, categorize by severity, propose mitigation

---

## 🖼️ Screenshots

📸 Add the following to your `screenshots/` folder:
- Kibana Discover View (filtered for suspicious events)
- Network scan pattern visualization
- Malware detection dashboard
- Example of log structure & timestamps

---

## 🧾 Incident Response Report

Includes:
- Timeline of events  
- Detected threats and severity  
- Affected IPs and users  
- Suggested remediation and lessons learned  

📄 File: `incident-report.docx`

---

## ✅ Deliverables

- ✅ Dockerized ELK stack  
- ✅ 1,000+ sample logs across categories  
- ✅ Kibana dashboard & visualizations  
- ✅ Incident report with screenshot references  
- ✅ Alert classification table  
- ✅ README with setup instructions and learning summary

---

## 🚧 Future Improvements

- Automate alerting rules in Elasticsearch  
- Integrate threat intelligence feeds  
- Export alerts to a Slack/Email channel  
- Use Logstash for real-time ingestion  

---

## 🔐 Keywords

`SIEM` · `Kibana` · `Elastic Stack` · `Log Analysis` · `Cybersecurity` · `Incident Response` · `SOC` · `Docker` · `Threat Hunting` · `Kali Linux`
