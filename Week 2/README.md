#  Week 2 - SOC Operations & Incident Response

##  Overview
This week focuses on mastering **alert prioritization, incident classification, and basic incident response** through both **theoretical knowledge** and **hands-on practical application**.  
The tasks align with industry standards such as **NIST SP 800-61**, **MITRE ATT&CK**, and **CVSS scoring** to simulate real-world SOC (Security Operations Center) workflows.

---

##  Learning Objectives
- Understand and apply **alert priority levels** (Critical, High, Medium, Low)
- Classify incidents using **MITRE ATT&CK**, **ENISA**, and **VERIS** frameworks
- Practice the **incident response lifecycle** from detection to recovery
- Gain hands-on experience with SOC tools like **Wazuh**, **TheHive**, **Velociraptor**, and **CrowdSec**
- Develop documentation, response templates, and communication workflows

---

##  Theoretical Knowledge

### 1. Alert Priority Levels
**Learn:**
- Severity levels and their criteria (Critical, High, Medium, Low)
- Prioritization using CVSS, asset criticality, and exploit likelihood  
- Use of CVSS scoring (e.g., Log4Shell CVSS 9.8 = Critical)

**References:**
- [FIRST CVSS Guide](https://www.first.org/cvss/)
- [NIST SP 800-61](https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final)
- CISA Alerts for real-world prioritization examples

---

### 2. Incident Classification
**Learn:**
- Categorization by incident type (malware, phishing, DDoS, insider threat, etc.)
- Use of standardized taxonomies:
  - **MITRE ATT&CK**
  - **ENISA Incident Taxonomy**
  - **VERIS Framework**
- Enriching incidents with metadata (IOCs, timestamps, affected assets)

**Practice:**  
Classify and enrich incidents using MITRE ATT&CK mappings.

---

### 3. Basic Incident Response
**Learn:**
- Phases: **Preparation → Identification → Containment → Eradication → Recovery → Lessons Learned**
- Key procedures: evidence collection, isolation, and SOAR automation
- Reference frameworks:
  - **NIST SP 800-61**
  - **SANS Incident Handler’s Handbook**

---

##  Practical Application

### 1. Alert Management Practice
**Tools:** Google Sheets, Wazuh, TheHive  
**Tasks:**
- Create an alert classification system (map alerts to MITRE techniques)
- Prioritize simulated alerts using CVSS scores
- Build a Wazuh dashboard for visualization
- Draft an incident ticket in TheHive
- Write a **100-word escalation email** to Tier 2 summarizing a Critical alert

---

### 2. Response Documentation
**Tools:** Google Docs, Draw.io  
**Tasks:**
- Develop an **Incident Response Template** (SANS format)
- Log investigation steps with timestamps
- Create a **Phishing Response Checklist**
- Conduct a **Post-Mortem** summarizing lessons learned (50 words)

---

### 3. Alert Triage Practice
**Tools:** Wazuh, VirusTotal, AlienVault OTX  
**Tasks:**
- Simulate triage on mock alerts (e.g., brute-force SSH attempts)
- Validate IOCs using threat intelligence platforms
- Document triage results and findings (50 words)

---

### 4. Evidence Preservation
**Tools:** Velociraptor, FTK Imager  
**Tasks:**
- Perform volatile data collection (e.g., `SELECT * FROM netstat`)
- Acquire and hash memory dumps for chain-of-custody tracking  
- Document evidence collection details in a structured table

---

### 5. Capstone Project: Full Alert-to-Response Cycle
**Tools:** Metasploit, Wazuh, CrowdSec, Google Docs  
**Workflow:**
1. **Simulate Attack:** Exploit Metasploitable2 (e.g., `vsftpd_234_backdoor`)
2. **Detect & Triage:** Use Wazuh to capture and analyze alerts
3. **Respond:** Isolate VM and block attacker IP with CrowdSec
4. **Report:** Write a 200-word incident report (SANS format)
5. **Briefing:** Draft a 100-word summary for non-technical management

---

## 🗂️ Repository Structure
