# MISP-Threat-Intelligence Investigation

## Threat Intelligence Analysis of Ransomware, Threat Actors, and Enterprise Vulnerabilities

## Overview
This project documents a threat intelligence investigation conducted using the Malware Information Sharing Platform (MISP). The focus was on analyzing ransomware campaigns, nation-state threat actors, DDoS malware, and enterprise vulnerabilities using real-world threat intelligence data.
The goal of this project is to simulate a SOC Threat Intelligence Analyst workflow by analyzing indicators of compromise (IOCs), correlating adversary activity, and mapping findings to the MITRE ATT&CK framework.

##  Objectives
In this investigation, I worked on:
- Analyzing ransomware intelligence events (LockBit, Babuk)
- Investigating APT activity (Turla Group)
- Studying DDoS botnet malware (CoalaBot, Rhombus)
- Analyzing enterprise vulnerabilities (MiVoice CVE exploitation)
- Extracting and correlating Indicators of Compromise (IOCs)
- Mapping attacker behavior to MITRE ATT&CK framework


## Lab Environment
   Component         | Details                                                        |
| ------------------ | -------------------------------------------------------------- |
| Platform           | Malware Information Sharing Platform (MISP)                    |
| Investigation Type | Threat Intelligence Analysis                                   |
| Focus Areas        | Ransomware, Threat Actors, Malware, Vulnerability Intelligence |
| Framework          | MITRE ATT&CK                                                   |
| Role Simulated     | Threat Intelligence Analyst                                    |


## Tools & Frameworks
- MISP Threat Intelligence Platform
- Web-based threat intelligence research (inside lab environment)
- MITRE ATT&CK framework
- Threat actor and malware datasets

## Investigation Process

The investigation consisted of reviewing multiple threat intelligence events available within the MISP platform. Each event contained intelligence related to ransomware campaigns, malware families, threat actors, exploited vulnerabilities, and indicators of compromise.

The investigation included:

- Searching MISP threat feeds for ransomware-related events
- Reviewing intelligence reports associated with LockBit and Babuk ransomware
- Examining YARA rules used to identify malware artifacts
- Investigating Turla threat actor activity and associated phishing campaigns
- Reviewing MITRE ATT&CK mappings for adversary techniques
- Analyzing DDoS malware campaigns including CoalaBot and Rhombus
- Researching enterprise vulnerabilities affecting MiVoice Connect
- Correlating indicators, malware artifacts, and threat intelligence reports

## Investigation Highlights

### Ransomware Intelligence
- Analyzed LockBit and Babuk ransomware campaigns
- Extracted domains, file hashes, and malware artifacts
- Reviewed YARA rules for malware detection

Screenshot: Ransomware search results in MISP  
Screenshot: LockBit event page  
Screenshot: Babuk YARA rule  
Screenshot: IOC list (domains, hashes, IPs)

### Threat Actor Analysis (Turla Group)
- Investigated APT Turla (G0010)
- Reviewed phishing campaigns and decoy documents
- Mapped activity to MITRE ATT&CK techniques

Screenshot: Turla event page  
Screenshot: MITRE ATT&CK matrix  
Screenshot: Threat actor galaxy view  
Screenshot: Phishing decoy document

### DDoS Malware Intelligence
Examined botnet infrastructure associated with CoalaBot and Rhombus malware, 
identifying command-and-control communication patterns and indicators of compromised systems.

Screenshot: CoalaBot event  
Screenshot: Rhombus malware event  

### Vulnerability Intelligence (MiVoice / Lorenz)
- Investigated MiVoice Connect CVE exploitation
- Reviewed ransomware persistence techniques
- Analyzed Lorenz ransomware lifecycle

Screenshot: MiVoice CVE event  
Screenshot: Arctic Wolf report artifact  
Screenshot: Lorenz ransomware galaxy  

## MITRE ATT&CK Mapping

Observed adversary tactics included:
- Initial Access (phishing campaigns)
- Persistence
- Privilege Escalation
- Collection
- Command and Control
These tactics demonstrate a full attack lifecycle from initial access through persistence and data collection activities.

## Indicators of Compromise (IOCs)
- IP addresses  
- Domains  
- URLs  
- File hashes (MD5 / SHA256)  
- Malware filenames  
- CVE identifiers  

## Detection Opportunities
The investigation highlighted several opportunities for improving threat detection within a Security Operations Center.
Potential defensive actions include:
- Monitoring known malicious IP addresses and domains identified through threat intelligence feeds
- Deploying YARA signatures to detect ransomware artifacts
- Enriching SIEM alerts using MISP IOC feeds
- Monitoring endpoint activity associated with known ATT&CK techniques
- Prioritizing remediation of internet-facing systems affected by known CVEs
- Correlating IOC matches with endpoint and network telemetry to improve detection fidelity

## Key Takeaways

This project demonstrates how threat intelligence supports SOC operations by connecting raw indicators to real adversary behavior.
It reinforced the importance of correlating multiple intelligence sources (IOCs, malware data, ATT&CK mappings, and vulnerability reports) to understand attack campaigns rather than analyzing isolated artifacts.

## Skills Demonstrated
- Threat Intelligence Analysis  
- IOC Correlation  
- Malware Research  
- Threat Actor Analysis  
- MITRE ATT&CK Mapping  
- SOC Investigation Workflow  
- Vulnerability Intelligence  

## Screenshots
(See sections above for required screenshots)

## Lessons Learned
This investigation helped me understand that threat intelligence is not just about collecting indicators of compromise, but about building context around attacker behavior.
Working with MISP showed me how ransomware campaigns, threat actors, malware, and vulnerabilities are interconnected. I learned how to pivot between different intelligence sources to build a clearer picture of adversary activity rather than treating each indicator separately.
It also improved how I think about SOC investigations, especially the importance of documenting findings clearly so other analysts can quickly understand and act on the information. This experience strengthened my confidence in using threat intelligence as part of detection and incident response workflows, and it’s a skill I plan to continue developing.

## Notes

This investigation was completed in a controlled lab environment using MISP as part of SOC and Threat Intelligence training.

