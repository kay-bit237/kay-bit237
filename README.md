# Hi, I'm Rosmaine Nkouankam 👋

I am a **SOC Analyst** working on the frontline of security operations. I monitor alerts, review logs, and investigate suspicious activity to catch threats early. I handle alert triage, escalate when needed, and support response efforts to help contain and resolve incidents quickly.

I also work on improving detection by tuning alerts, cutting down false positives, and keeping our security posture aligned with internal policies and regulatory requirements.

Outside of my day to day work, I build hands on labs in Microsoft Azure, Microsoft Defender, Microsoft Sentinel, and Tenable Nessus to keep sharpening the same skills I use in the SOC. Every project below is documented with objectives, methodology, screenshots, findings, and lessons learned.

All testing documented here was performed in personal lab environments that I own and control.

<br>

## 🔐 Cybersecurity Projects

### Microsoft Defender: Brute Force Detection and Incident Response

Built a complete detection and response workflow using Microsoft Defender, Microsoft Sentinel, and Log Analytics, from data collection through to containment.

* Configured continuous export from Defender for Cloud to a Log Analytics workspace
* Enabled full Windows security event collection and installed the Windows Security Events solution from the Sentine l Content Hub
* Built a custom Sentinel analytics rule to detect repeated failed logon attempts, which triggered 16+ alerts
* Investigated a real Defender XDR incident using the incident graph and process tree analysis
* Traced an unexpected outbound connection from `notepad.exe` and validated the remote IP in VirusTotal
* Applied the principle that a clean IP reputation does not clear suspicious behavior
* Isolated the affected device as a containment action and documented the full workflow

**Skills:** EDR, SIEM, detection engineering, incident investigation, threat intelligence, containment

[View Project](https://github.com/kay-bit237/Defender-Brute-Force-Incident-Response)

<br>

### Nessus Vulnerability Assessment: Windows Server 2022

Performed a self directed vulnerability assessment of a Windows Server 2022 VM using Tenable Nessus, focused on the same triage method I use on production hosts.

* Verified scan authentication status first (Auth: N/A) and documented what an unauthenticated scan can and cannot show
* Triaged 133 findings and prioritized SSL, the highest finding count on the host
* Analyzed two Medium findings (CVSS 6.5): an untrusted certificate and a self signed certificate
* Explained the real world impact beyond the score, including silent man in the middle exposure
* Identified a cross protocol pattern across SSL, TLS, HTTP, and SMB that pointed to a configuration hygiene problem
* Documented a follow up scan with failed authentication that surfaced 199 findings, including 6 Critical and 16 High

**Skills:** vulnerability management, CVSS analysis, risk prioritization, SSL/TLS security, reporting

[View Project](https://github.com/kay-bit237/Nessus-Vulnerability-Assessment-Windows-Server)

<br>

### Azure Log Flow and Monitoring with Microsoft Sentinel

Built a log pipeline in Azure to answer one question: if something happens in the environment right now, do I know where to trace it?

* Routed subscription Activity Logs to a Log Analytics workspace using diagnostic settings
* Deployed Microsoft Sentinel on the workspace for SIEM analysis
* Wrote KQL queries to detect repeated failed logons (Event ID 4625) grouped by source IP
* Reviewed process creation (Event ID 4688) and privileged service call (Event ID 4673) events
* Compared proactive and reactive monitoring and documented what to look for in logs
* Mapped the logging controls to NIST 800-53, ISO 27001, and PCI DSS

**Skills:** KQL, Log Analytics, Microsoft Sentinel, threat hunting, log analysis

[View Project](https://github.com/kay-bit237/Azure-Log-Flow-Monitoring-Lab)

<br>

### Azure Storage Accounts: Redundancy and Security Configuration

Provisioned and reviewed Azure Storage Accounts to understand how early configuration choices affect durability, availability, and security.

* Documented LRS, ZRS, GRS, GZRS, and RA GRS and when each one fits
* Configured an account with RA GRS across East US 2 and Central US
* Reviewed security settings including secure transfer, blob anonymous access, key access, and minimum TLS 1.2
* Analyzed four Azure Advisor recommendations from a SOC perspective: zone redundancy, shared key access, network restrictions, and private link
* Flagged a logging gap where only blob diagnostics were enabled

**Skills:** cloud security, configuration review, data resilience, risk analysis

[View Project](https://github.com/kay-bit237/Azure-Storage-Accounts-Lab)

<br>

### Microsoft Entra ID: Role Based Access Control

Implemented least privilege access in Microsoft Entra ID by creating users and assigning department specific roles.

* Created three users and mapped each to a department
* Assigned **Security Reader** to the Security user for read only visibility
* Assigned **Agent ID Developer** to the Development user for scoped development tasks
* Assigned **Global Reader** to the HR user for broad oversight with no modification rights
* Documented permissions, restrictions, and the justification for each role
* Tied the design to NIST 800-53 and ISO 27001 access control principles

**Skills:** identity and access management, RBAC, least privilege, cloud governance

[View Project](https://github.com/kay-bit237/Microsoft-Entra-ID)

<br>

## 🛠 Tools and Technologies

| Category | Tools |
|---|---|
| **SIEM and Detection** | Splunk, Microsoft Sentinel, KQL |
| **Endpoint Security** | Microsoft Defender XDR, EDR |
| **Vulnerability Management** | Tenable Nessus |
| **Cloud and Identity** | Microsoft Azure, Microsoft Entra ID, Log Analytics, Azure Advisor |
| **Threat Intelligence** | MITRE ATT&CK, VirusTotal |
| **Ticketing and Awareness** | ServiceNow, KnowBe4 |
| **Networking** | TCP/IP |

<br>

## 📋 Frameworks and Compliance

`MITRE ATT&CK` `NIST 800 53` `ISO 27001` `PCI DSS`

<br>

## 🎯 Threats I Investigate

Phishing, smishing, social engineering, brute force attacks, ransomware, trojans, and denial of service.

<br>

## 🔍 What I Do Day to Day

* Monitor alerts and review logs across SIEM and EDR platforms
* Triage alerts, escalate when needed, and support incident response
* Tune detections to cut false positives and improve signal quality
* Support compliance with internal policies and regulatory requirements
* Run security awareness training to reduce human risk

<br>

## 📌 Current Focus

* Phishing and smishing analysis and investigation playbooks
* Detection tuning and alert quality
* Cloud and identity security in Azure
* Vulnerability triage and remediation validation
* Building a documented, evidence based security portfolio

<br>



## 🌟 Beyond the SOC

Tennis, reading, community volunteering, time with family, and staying current on emerging cyber threats.

<br>

## 📫 Connect

[LinkedIn](https://www.linkedin.com/in/rosmaine-nkouankam/)

<br>

<p align="center"><i>Stay alert, stay secure.</i></p>
