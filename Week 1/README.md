Week 1 - SOC Fundamentals, Monitoring & Incident Response

This week introduces the foundational concepts of Security Operations Centers (SOC), including their purpose, workflow, tools, and incident response processes. Students will gain hands-on experience in log collection, analysis, alert configuration, and documentation within a mini-SOC lab environment.

Learning Objectives

* Understand SOC structure, roles, and responsibilities
* Learn key security monitoring and log management fundamentals
* Explore core security tools such as SIEM, EDR, IDS/IPS, and vulnerability scanners
* Apply basic security concepts including the CIA triad, threats, vulnerabilities, and risk
* Follow standard SOC workflows and incident response lifecycles
* Practice documenting security events, creating dashboards, and configuring alerts

Theoretical Knowledge

SOC Fundamentals and Operations
Learn:

* Purpose: Proactive threat detection, incident response, continuous monitoring
* Roles: Tier 1/2/3 analysts, SOC manager, threat hunters
* Key Functions: Log analysis, alert triage, threat intelligence integration
* References: NIST frameworks, MITRE ATT&CK, SOC walkthrough videos (IBM SOC, Microsoft SOC)

Security Monitoring Basics
Learn:

* Objectives: Detect anomalies, unauthorized access, and policy violations
* Tools: SIEM (Splunk, Elastic), network traffic analyzers (Wireshark)
* Key Metrics: False positives/negatives, mean time to detect (MTTD)
* References: Elastic SIEM guides, Boss of the SOC datasets

Log Management Fundamentals
Learn:

* Log Lifecycle: Collection, normalization, storage, retention, analysis
* Common Log Types: Windows Event Logs, Syslog, HTTP server logs
* Tools: Fluentd, Logstash
* References: KQL in Elastic SIEM, JSON/CEF log formats

Security Tools Overview
Learn:

* SIEM: Splunk, QRadar
* EDR: CrowdStrike
* IDS/IPS: Snort
* Vulnerability Scanners: Nessus
* References: Splunk Free, Wazuh, Osquery, Nessus Essentials

Basic Security Concepts
Learn:

* CIA Triad: Confidentiality, Integrity, Availability
* Threat vs Vulnerability vs Risk
* Defense-in-Depth, Zero Trust
* References: Anki flashcards, Equifax breach case study

Security Operations Workflow
Learn:

* Detection: Alerts from SIEM/EDR
* Triage: Prioritize based on severity
* Investigation: Correlate logs, hunt IOCs
* Response: Containment, eradication
* References: TheHive platform simulations

Incident Response Basics
Learn:

* IR Lifecycle: Preparation → Identification → Containment → Eradication → Recovery → Lessons Learned
* References: NIST SP 800-61, tabletop exercises (ransomware scenario)

Documentation Standards
Learn:

* Incident reports, runbooks, SOPs, post-mortems
* References: SANS Incident Handler’s Handbook

Practical Application

Log Analysis Practice
Tools: Windows Event Viewer, Eric Zimmerman Tools, Elastic SIEM, LogParser Lizard
Tasks:

* Filter Event ID 4625 (failed login) and 7045 (new service creation)
* Detect brute-force attacks
* Parse browser history for malicious URLs
* Advanced: Generate failed logins in VM, export results to CSV; parse Chrome history using LECmd

Document Security Events
Tasks:

* Use template: Date/Time | Source IP | Event ID | Description | Action Taken
* Document mock events (e.g., multiple failed logins from a test IP)

Set Up Monitoring Dashboards
Tools: Kibana, Grafana
Tasks:

* Visualize top 10 source IPs generating alerts
* Track frequency of critical Event IDs
* Use pre-built dashboards (Sigma rules)

Configure Alert Rules
Tools: Elastic SIEM, Wazuh
Tasks:

* Detect 5+ failed logins in 5 minutes (Elastic SIEM)
* Create custom alert in Wazuh for 3+ failed logins in 2 minutes
* Test and validate alerts; document rule effectiveness

Learning Approach

* Build a mini-SOC lab with Wazuh (SIEM) + Osquery (endpoint visibility)
* Map alerts to MITRE ATT&CK adversary tactics (e.g., T1059 for PowerShell attacks)
* Integrate practical exercises with theoretical knowledge for end-to-end SOC understanding

