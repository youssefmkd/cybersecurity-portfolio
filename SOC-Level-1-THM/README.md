---
layout: default
title: TryHackMe SOC Level 1
---

# 🛡️ TryHackMe SOC Level 1

This folder contains my **TryHackMe SOC Level 1 labs, exercises, and case studies**, covering SOC fundamentals, SIEM investigations, threat hunting, and incident response.

---

## 📂 TryHackMe SOC Level 1 Sections

### 1. [Cyber Defense Frameworks](CDF/README.md)
- **Completed Modules:** Junior Security Analyst Intro, Pyramid of Pain, Cyber Kill Chain, Unified Kill Chain, Diamond Model, MITRE, Summit, Eviction
- **Case Studies:**  
  1. [MITRE ATT&CK Mapping](CDF/case-study-mitre.md) – Mapped real-world incidents to MITRE ATT&CK tactics and techniques to identify detection gaps.  
  2. [Cyber Kill Chain Simulation](CDF/case-study-killchain.md) – Analyzed attack stages in a simulated environment to practice early detection and response strategies.  
  3. [Diamond Model Analysis](CDF/case-study-diamond.md) – Applied the Diamond Model to investigate threat actor infrastructure, capabilities, and objectives.
     
 

### 2. [Cyber Threat Intelligence](CTI/README.md)
- **Completed Modules:** Intro to Cyber Threat Intel, Threat Intelligence Tools, Yara, OpenCTI, MISP, Friday Overtime, Trooper
- **Case Studies:**  
  1. [YARA Threat Detection](CTI/case-study-yara.md) – Created and applied YARA rules to detect malware patterns and indicators of compromise.  
  2. [MISP Intelligence Analysis](CTI/case-study-misp.md) – Leveraged MISP to aggregate threat intelligence and analyze correlations between incidents.  
  3. [OpenCTI Threat Investigation](CTI/case-study-opencti.md) – Tracked threat actor TTPs using OpenCTI, identifying actionable intelligence for defense.

     
 
### 3. [Network Security & Traffic Analysis](Network/README.md)
- **Completed Modules:** Traffic Analysis Essentials, Snort, Snort Challenge - The Basics, Snort Challenge - Live Attacks, NetworkMiner, Zeek, Zeek Exercises, Brim, Wireshark: The Basics, Wireshark: Packet Operations, Wireshark: Traffic Analysis, TShark: The Basics, TShark: CLI Wireshark Features, TShark Challenge I: Teamwork, TShark Challenge II: Directory
- **Case Studies:**  
  1. [Snort Live Attacks Challenge](Network/case-study-snort-live.md) – Detected and analyzed simulated network attacks using Snort IDS rules and alert patterns.  
  2. [Wireshark Traffic Analysis](Network/case-study-wireshark.md) – Examined packet captures to identify anomalies, suspicious protocols, and potential data exfiltration.  
  3. [Zeek Network Monitoring](Network/case-study-zeek.md) – Leveraged Zeek logs to track host activity, detect suspicious connections, and analyze network flows.
 


### 4. [Endpoint Security Monitoring](Endpoint/README.md)
- **Completed Modules:** Intro to Endpoint Security, Core Windows Processes, Sysinternals, Windows Event Logs, Sysmon, Osquery: The Basics, Wazuh, Monday Monitor, Retracted  
- **Case Studies:**  
  1. [Core Windows Processes Analysis](Endpoint/case-study-core-processes.md) – Investigated critical Windows processes to differentiate between normal and malicious activity.  
  2. [Sysinternals for Threat Hunting](Endpoint/case-study-sysinternals.md) – Leveraged Sysinternals tools to analyze running processes, network connections, and persistence techniques.  
  3. [Sysmon Event Analysis](Endpoint/case-study-sysmon.md) – Built detections and investigated suspicious behavior using Sysmon logs.  
  4. [Endpoint Visibility with Osquery](Endpoint/case-study-osquery.md) – Queried endpoint artifacts for process, file, and user activity to detect anomalies.  
  5. [Endpoint Detection with Wazuh](Endpoint/case-study-wazuh.md) – Used Wazuh to collect and analyze endpoint logs for intrusion detection and monitoring.



### 5. [Security Information and Event Management](SIEM/README.md)
- **Completed Modules:** Intro to SIEM, Investigating with ELK101, ItsyBitsy (Splunk), Splunk Basics, Incident Handling with Splunk, Investigating with Splunk, Benign  
- **Case Studies:**  
  1. [Investigating with ELK 101](SIEM/case-study-elk.md) – Built queries and dashboards to analyze authentication logs and detect anomalies.  
  2. [ItsyBitsy (Splunk) Investigation](SIEM/case-study-itsybitsy.md) – Conducted hands-on analysis using Splunk to identify suspicious events and patterns.  
  3. [Incident Handling with Splunk](SIEM/case-study-incident-handling.md) – End-to-end incident investigation including detection, analysis, and reporting.  
  4. [Investigating with Splunk](SIEM/case-study-investigating.md) – Detailed investigations on scenarios like brute-force attempts and unauthorized access.
  


### 6. [Digital Forensics & Incident Response (DFIR)](DFIR/README.md)
- **Completed Modules:** DFIR: An Introduction, Windows Forensics 1 & 2, Linux Forensics, Autopsy, Redline, KAPE, Volatility, Velociraptor, TheHive Project, Intro to Malware Analysis, Unattended, Disgruntled, Critical, Secret Recipe  
- **Case Studies:**  
  1. [Unattended](DFIR/case-study-unattended.md) – Investigated unauthorized access by analyzing Windows event logs, registry artifacts, and user activity.  
  2. [Disgruntled](DFIR/case-study-disgruntled.md) – Insider threat case involving forensic analysis of file access and potential data exfiltration.  
  3. [Critical](DFIR/case-study-critical.md) – Malware investigation using memory and disk forensics with Volatility and Redline.  
  4. [Secret Recipe](DFIR/case-study-secret-recipe.md) – Full end-to-end DFIR case involving malware, insider activity, and lateral movement; solved using multiple forensic tools.  



### 7. [Phishing Analysis & Prevention](Phishing/README.md)
- **Completed Modules:** Phishing Analysis Fundamentals, Phishing Emails in Action, Phishing Analysis Tools, Phishing Prevention, The Greenholt Phish, Snapped Phish-ing Line, Phishing Unfolding  
- **Case Studies:**  
  1. [The Greenholt Phish](Phishing/case-study-greenholt.md) – Analyzed a simulated phishing campaign to identify malicious emails, extract IOCs, and recommend mitigation strategies.  
  2. [Snapped Phish-ing Line](Phishing/case-study-snapped-phish.md) – Tracked phishing email headers, sender spoofing, and delivery vectors to reconstruct the attack flow.  
  3. [Phishing Unfolding](Phishing/case-study-unfolding.md) – Performed full campaign analysis, identifying end-user impact, malware attachments, and phishing infrastructure.  



### 8. [SOC Level 1 Capstone Challenges](SOC/README.md)
- **Completed Modules:** Tempest, Boogeyman 1, Boogeyman 2, Boogeyman 3, Upload and Conquer, Hidden Hooks, BlackCat
- **Case Studies:**  
  1. [Boogeyman Series Investigations](SOC/case-study-boogeyman.md) – Conducted multi-step SOC investigations to detect, analyze, and respond to simulated attacks.  
  2. [Upload and Conquer Challenge](SOC/case-study-upload.md) – Examined malicious file uploads and network traffic to identify indicators of compromise (IOCs).  
  3. [Hidden Hooks Analysis](SOC/case-study-hiddenhooks.md) – Detected stealthy malware hooks and traced attacker activity within endpoints.  
  4. [BlackCat Incident Response](SOC/case-study-blackcat.md) – Performed end-to-end response for ransomware-style attack simulations.

---

## 📌 Skills Demonstrated
- **SIEM & Log Analysis**: Splunk, ELK  
- **Incident Response & DFIR**: Volatility, Autopsy  
- **Endpoint Monitoring**: Sysmon, Wazuh  
- **Phishing Analysis**: Email header & attachment triage  
- **Network Defense**: Snort, Zeek  
- **Threat Intelligence**: Yara, OpenCTI, MISP  
