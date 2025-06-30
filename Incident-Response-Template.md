---
title: "Cyber Incident Response Report Template"
author: ["incidentresponse@youremailaddress.com"]
date: "2024-01-01"
subject: "Markdown"
keywords: [Markdown, Example]
subtitle: "Cyber Incident Response"
lang: "en"
titlepage: true
titlepage-color: "108062"
titlepage-text-color: "FFFAFA"
titlepage-rule-color: "FFFAFA"
titlepage-rule-height: 2
book: true
classoption: oneside
code-block-font-size: \scriptsize
---

# Document Control  

| Version | Date       | Author             | Reviewer / Approver | Comments                  |
|---------|------------|-------------------|--------------------|--------------------------|
| 1.0     | 2025-06-30 | John Doe (IR Lead) | Jane Smith (CISO)   | Initial version           |
| 1.1     | 2025-07-01 | John Doe (IR Lead) | Jane Smith (CISO)   | Added forensic findings   |
| 1.2     | 2025-07-03 | John Doe (IR Lead) | Jane Smith (CISO)   | Final version for approval|

## Document Classification  
Confidentiality Level: CONFIDENTIAL  

# Incident Overview and Executive Briefing  

## Executive Summary  
This section provides a high-level summary of the incident for executive and non-technical audiences.  
It briefly describes what happened, the business and operational impact, and the major actions taken by the response team.  
It concludes with the current status of the incident, highlighting whether the situation has been resolved or if monitoring continues.

- **Incident Overview:** Brief description of the incident.
- **Business and Operational Impact:** Summary of impact to systems, services, data, or reputation.
- **Summary of Actions Taken:** Key containment, eradication, and recovery efforts.
- **Current Status:** Final state of the incident (e.g., resolved, under monitoring).

## Timeline of Events  
This section provides a chronological record of significant events related to the incident.  
It helps stakeholders understand how the situation unfolded, what the attacker did, and how defenders responded.

- **Threat Intelligence Timeline:** External advisories, CVE disclosures, or bulletins relevant to the incident.
- **Intrusion Timeline:** Major attacker activities within the environment.
- **Incident Response Timeline:** Key detection, containment, eradication, and recovery milestones.
- **Communications Timeline:** Internal and external notifications, including regulatory reports.

## Threat Intelligence  
This section summarizes the threat intelligence that informed detection, response, and mitigation efforts.  
It includes details about known vulnerabilities, external advisories, attribution efforts, and observed attacker techniques.

### Known Vulnerabilities  
Describe vulnerabilities exploited or targeted.  
Include CVEs, public exploit availability, and patch status at the time of the incident.

### External Communications and Bulletins  
Summarize external advisories, vendor bulletins, or ISAC notifications relevant to the incident.

### Threat Actor Attribution  
Describe any suspected threat actors or groups.  
Include confidence level and connections to known campaigns.

### Observed Tactics, Techniques, and Procedures (TTPs)  
Summarize attacker behaviors mapped to frameworks like MITRE ATT&CK.

# Technical Investigation and Findings  

## Attack Path and Activity  
Detail how the attacker gained access, moved within the environment, escalated privileges, maintained persistence, and deployed tools or malware.

- Initial access vector
- Lateral movement
- Privilege escalation
- Persistence mechanisms
- Malware/tools deployed  

## Forensic and Log Analysis  
This section presents findings from the technical investigation, including methods used to collect and analyze evidence.  
It highlights key discoveries that supported response actions and informs future defenses.  
It ensures transparency and defensibility for audit, regulatory, or legal purposes.

Multiple data sources were examined, including disk images, memory captures, and log files from impacted systems.  
Supporting artifacts such as file hashes, configuration files, and screenshots were collected to create a verifiable record of the investigation.

- Disk, memory, and log analysis results
- Key artifacts (e.g., binaries, scripts, configs)
- Supporting evidence (hashes, screenshots, timeline artifacts)

# Recommendations  
This section provides actionable guidance for strengthening defenses and preventing similar incidents in the future.  
It should address containment, eradication, recovery, and longer-term prevention measures.

- **Containment Recommendations:** Immediate steps to improve isolation.
- **Eradication Recommendations:** Actions to fully remove the threat.
- **Recovery Recommendations:** Measures to restore operations securely.
- **Lessons Learned:** Key insights from the incident.
- **Future Prevention Measures:** Long-term improvements (e.g., tooling, processes, training).

## Resolution and Next Steps  
Summarize the closure status of the incident and planned follow-up actions.  
Include the final state of the environment, confidence in remediation, and ongoing monitoring efforts.

- Final state of the environment (e.g., secured, under monitoring)
- Confidence in remediation
- Ongoing monitoring or follow-up plans  

# Detection Opportunities  
This section outlines actionable detection materials identified or developed during the investigation.  
It includes indicators, behavioral patterns, and detection rules that support monitoring, hunting, and prevention.

### Atomic Indicators  
- IP addresses  
- Domain names / URLs  
- Email addresses  
- File names  

### Computed Indicators  
- File hashes (MD5, SHA256)  
- Registry keys  
- File paths  

### Detection Rules and Capabilities  
- YARA rules  
- Sigma rules  
- Snort / Suricata signatures  
- Custom scripts or queries  

### Tactics, Techniques, and Procedures (TTPs)  
- Mapped MITRE ATT&CK tactics and techniques  
- Tools or frameworks used  
- Persistence and lateral movement behaviors  
