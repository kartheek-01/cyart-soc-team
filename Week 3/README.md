Week 3 - Advanced SOC Operations & Threat Intelligence
Overview

This week focuses on mastering advanced log analysis, threat intelligence integration, and incident escalation workflows through both theoretical knowledge and hands-on practical application.
The tasks align with industry standards such as MITRE ATT&CK, STIX/TAXII, and NIST SP 800-61, simulating real-world SOC operations with enriched alerts and automated escalation.

Learning Objectives

Analyze and correlate logs from multiple sources to identify complex threats

Integrate threat intelligence into SOC workflows for proactive detection

Execute incident escalation using structured workflows and communication protocols

Perform alert triage and evidence preservation while maintaining chain-of-custody

Complete a full SOC workflow simulation from attack detection to management briefing

Theoretical Knowledge
1. Advanced Log Analysis

Learn:

Log Correlation: Correlate logs from endpoints, firewalls, and applications to detect attack patterns (e.g., Event ID 4625 failed logins with suspicious outbound traffic)

Anomaly Detection: Identify unusual activities such as abnormal login times or high-volume data transfers

Log Enrichment: Add context to logs (e.g., geolocation, user roles) to improve analysis

References:

SANS Reading Room: Effective Log Analysis

Elastic Security documentation

CISA case studies (e.g., Equifax breach)

2. Threat Intelligence Integration

Learn:

Threat Intelligence Types: IOCs (IP, hashes), TTPs, and threat feeds (STIX/TAXII)

SOC Integration: Enrich SIEM alerts automatically (e.g., suspicious IP mapped to known C2 server)

Threat Hunting: Proactively search for TTPs (e.g., T1078 - Valid Accounts misuse)

References:

MITRE ATT&CK for TTPs

OASIS STIX/TAXII standards

AlienVault OTX threat feeds

3. Incident Escalation Workflows

Learn:

Escalation Tiers: SOC Tier 1 (triage), Tier 2 (investigation), Tier 3 (advanced analysis) and escalation criteria

Communication Protocols: Structured reporting (e.g., SITREPs) and stakeholder briefings

Automation: Use SOAR tools for auto-assignment and alert enrichment

References:

NIST SP 800-61

SANS Incident Handler’s Handbook

Splunk SOAR documentation

Practical Application
1. Advanced Log Analysis

Tools: Elastic Security, Security Onion, Google Sheets
Tasks:

Correlate logs to detect attack patterns

Detect anomalies and enrich log data with contextual information

Document findings in structured tables

Example:

Timestamp	Event ID	Source IP	Destination IP	Notes
2025-08-18 12:00:00	4625	192.168.1.100	8.8.8.8	Suspicious DNS request
2. Threat Intelligence Integration

Tools: Wazuh, AlienVault OTX, TheHive
Tasks:

Import threat feeds into SOC tools

Enrich alerts with threat intelligence

Hunt for TTPs and summarize findings

Example:

Alert ID	IP	Reputation	Notes
003	192.168.1.100	Malicious (OTX)	Linked to C2 server
3. Incident Escalation Practice

Tools: TheHive, Google Docs
Tasks:

Simulate escalation of High-priority alerts

Draft SITREPs and stakeholder briefings

Automate alert assignment with SOAR tools

Example:

Escalate High-priority alert to Tier 2 with 100-word summary

Draft Situation Report for mock incident:

Title: Unauthorized Access on Server-Y

Summary: Detected 2025-08-18 13:00, IP: 192.168.1.200, MITRE T1078

Actions: Isolated server, escalated to Tier 2

4. Alert Triage with Threat Intelligence

Tools: Wazuh, VirusTotal, AlienVault OTX
Tasks:

Triage alerts and validate IOCs

Document triage results

Example:

Alert ID	Description	Source IP	Priority	Status
004	PowerShell Execution	192.168.1.101	High	Open
5. Evidence Preservation and Analysis

Tools: Velociraptor, FTK Imager
Tasks:

Collect volatile data and memory dumps

Hash evidence and maintain chain-of-custody

Document in structured table

Example:

Item	Description	Collected By	Date	Hash Value
Memory Dump	Server-Y Dump	SOC Analyst	2025-08-18	<SHA256>
6. Capstone Project: Full SOC Workflow Simulation

Tools: Metasploit, Wazuh, CrowdSec, TheHive, Google Docs
Workflow:

Simulate Attack: Exploit Metasploitable2 vulnerability (e.g., Samba usermap script)

Detect & Triage: Configure Wazuh alerts; document in table:

Timestamp	Source IP	Alert Description	MITRE Technique
2025-08-18 14:00:00	192.168.1.101	Samba exploit	T1210

Respond: Isolate VM, block attacker IP with CrowdSec

Escalate: Tier 2 case in TheHive with 100-word summary

Report: 200-word SANS-format report (Executive Summary, Timeline, Recommendations)

Briefing: Draft 100-word summary for non-technical management

🗂️ Repository Structure
