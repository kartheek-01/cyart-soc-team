Week 4 - Threat Hunting, SOAR Automation & SOC Improvement

This week focuses on proactive threat hunting, advanced SOAR automation, post-incident analysis, adversary emulation, and SOC performance metrics. Students will apply theoretical knowledge to hands-on tasks simulating real-world SOC operations, improving detection, automation, response, and reporting workflows.

Learning Objectives

* Develop and execute threat hunting methodologies using hypothesis-driven approaches
* Design and implement SOAR playbooks for automated SOC responses
* Conduct post-incident analysis, root cause investigations, and continuous improvement
* Simulate adversary TTPs to test SOC detection and response capabilities
* Calculate and present advanced SOC metrics for executive reporting
* Complete a full SOC incident response simulation integrating detection, triage, response, and reporting

Theoretical Knowledge

Threat Hunting Methodologies
Learn:

* Proactive Threat Hunting: Hypothesis-driven hunting vs. reactive incident response (e.g., anomalous privilege escalation)
* Hunting Frameworks: SqRR (Search, Query, Retrieve, Respond) and TaHiTI (Targeted Hunting integrating Threat Intelligence)
* Data Sources: EDR logs, network traffic, threat feeds
* References: SANS Threat Hunting papers, MITRE ATT&CK case studies, Elastic Security guides

Advanced SOAR Automation
Learn:

* SOAR Components: Orchestration, automation, response
* Playbook Development: Automate repetitive tasks such as IP blocking or phishing response
* Integration with SIEM/EDR: Tools like Wazuh and Elastic
* References: Splunk SOAR documentation, TheHive playbook examples, CISA automation case studies

Post-Incident Analysis & Continuous Improvement
Learn:

* Root Cause Analysis (RCA): 5 Whys, Fishbone Diagram
* Lessons Learned: Post-mortems for process, tool, and training improvements
* SOC Metrics: MTTD, MTTR, dwell time
* References: SANS Reading Room, NIST SP 800-61, CISA Cybersecurity Metrics

Adversary Emulation Techniques
Learn:

* Emulation of attacker TTPs (e.g., T1566 - Phishing, T1210 - Exploitation of Remote Services)
* Emulation Frameworks: MITRE Caldera
* Red-Blue Team Collaboration: Improve detection and controls
* References: MITRE Caldera guides, Red Canary emulation case studies, MITRE ATT&CK

Security Metrics & Executive Reporting
Learn:

* Advanced SOC Metrics: False positive rate, dwell time, incident resolution rate
* Executive Reporting: Present metrics and incident summaries clearly
* Continuous Improvement: Identify gaps and recommend solutions
* References: SANS Reading Room (“Measuring SOC Success”), CISA reporting frameworks, SANS templates

Practical Application

Threat Hunting Practice
Tools: Elastic Security, Velociraptor, AlienVault OTX
Tasks:

* Develop a hunting hypothesis (e.g., unauthorized privilege escalation)
* Query logs and validate findings
* Use threat intelligence to cross-reference IOCs
  Example Table:

| Timestamp           | User     | Event ID | Notes                 |
| ------------------- | -------- | -------- | --------------------- |
| 2025-08-18 15:00:00 | testuser | 4672     | Unexpected admin role |

SOAR Playbook Development
Tools: Splunk Phantom, TheHive, Google Docs
Tasks:

* Design playbooks for automated incident response
* Test playbook execution on simulated alerts
  Example Table:

| Playbook Step | Status  | Notes                          |
| ------------- | ------- | ------------------------------ |
| Check IP      | Success | IP flagged as malicious        |
| Block IP      | Success | CrowdSec blocked 192.168.1.102 |

Post-Incident Analysis
Tools: Google Sheets, Draw.io
Tasks:

* Conduct RCA and lessons learned
* Create Fishbone Diagram
* Calculate MTTD and MTTR
  Example Table (5 Whys):

| Question              | Answer                      |
| --------------------- | --------------------------- |
| Why was email opened? | User clicked malicious link |
| Why clicked link?     | Weak email filtering        |

Alert Triage with Automation
Tools: Wazuh, VirusTotal, TheHive
Tasks:

* Triage alerts and validate automatically with threat intelligence
  Example Table:

| Alert ID | Description   | Source IP     | Priority | Status |
| -------- | ------------- | ------------- | -------- | ------ |
| 005      | File Download | 192.168.1.102 | High     | Open   |

Evidence Analysis
Tools: Velociraptor, FTK Imager
Tasks:

* Analyze evidence and maintain chain-of-custody
  Example Table:

| Item        | Description  | Collected By | Date       | Hash Value |
| ----------- | ------------ | ------------ | ---------- | ---------- |
| Network Log | Server-Z Log | SOC Analyst  | 2025-08-18 | <SHA256>   |

Adversary Emulation Practice
Tools: MITRE Caldera, Wazuh
Tasks:

* Simulate TTPs and test SOC detection
  Example Table:

| Timestamp           | TTP   | Detection Status | Notes                  |
| ------------------- | ----- | ---------------- | ---------------------- |
| 2025-08-18 17:00:00 | T1566 | Detected         | Phishing email blocked |

Security Metrics & Executive Reporting
Tools: Elastic Security, Google Sheets, Google Docs
Tasks:

* Calculate metrics (MTTD, MTTR, dwell time)
* Draft executive summary reports
* Build dashboards
  Example: MTTD = 2 hours, MTTR = 4 hours

Capstone Project: Comprehensive SOC Incident Response
Tools: Metasploit, Wazuh, CrowdSec, TheHive, MITRE Caldera, Elastic Security, Google Docs
Workflow:

* Attack Simulation: Exploit Metasploitable2 vulnerability
* Adversary Emulation: Simulate TTPs (T1210, T1566) and document detection
* Detection & Triage: Configure Wazuh alerts, triage in TheHive
* Response & Containment: Isolate VM, block attacker IP, verify
* SOAR Automation: Automate IP blocking and ticket creation
* Post-Incident Analysis: Conduct RCA, create Fishbone Diagram
* Metrics Reporting: MTTD, MTTR, dwell time, dashboards
  
* Reporting: 300-word SANS-format report + 150-word executive briefing
