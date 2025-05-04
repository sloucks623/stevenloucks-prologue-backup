
---
title: "Lab 1.0 – SOC Automation Home Lab"
layout: post
---

## Lab 1.0 – SOC Automation Home Lab

🎯 **Objective**:  
To simulate and explore the Tier 1 SOC Analyst role using freely available tools, with an emphasis on *automating routine alert triage and threat investigation workflows*.

🔧 **Tools Used**:
- Splunk (Free edition)
- VirusTotal
- AbuseIPDB
- MITRE ATT&CK Navigator
- Any.run sandbox
- Custom scripts and workflows to streamline common tasks

📚 **Overview**:  
This lab recreates the investigative flow a SOC analyst follows when responding to potential security alerts. The emphasis is on *learning by doing* while also identifying opportunities for **automation** in tasks like IOC lookups, reputation checking, and documentation formatting.

The project is based on guidance from the video by **My Fdir**:  
🎥 [SOC Analyst Lab Walkthrough – YouTube](https://youtu.be/Lb_ukgtYK_U?si=-2941ZdhRNAbT2rm)  
💬 *Special thanks to My Fdir for creating accessible, hands-on content for aspiring cybersecurity professionals.*

---

🚧 **Work in Progress**  
This is an evolving lab. As automation scripts and new tools are integrated, updates will be pushed to this repository. Future versions may include Python scripting, SIEM log parsing automation, and enrichment integrations with APIs like VirusTotal or AbuseIPDB.
---
title: "Lab 1.0 – SOC Automation Home Lab"
layout: post
---

## Lab 1.0 – SOC Automation Home Lab

🎯 **Objective**:  
To simulate and explore the Tier 1 SOC Analyst role using freely available tools, with an emphasis on *automating routine alert triage and threat investigation workflows*.

🔧 **Tools Used**:
- Splunk (Free edition)
- VirusTotal
- AbuseIPDB
- MITRE ATT&CK Navigator
- Any.run sandbox
- Custom scripts and workflows to streamline common tasks

📚 **Overview**:  
This lab recreates the investigative flow a SOC analyst follows when responding to potential security alerts. The emphasis is on *learning by doing* while also identifying opportunities for **automation** in tasks like IOC lookups, reputation checking, and documentation formatting.

The project is based on guidance from the video by **MyDFIR**:  
🎥 [SOC Automation Lab Walkthrough – YouTube](https://youtu.be/XR3eamn8ydQ?si=WLR8_IjbkIGodCc5)  
💬 *Special thanks to MyDFIR for creating accessible, hands-on content for aspiring cybersecurity professionals.*

---

## 📌 Part 1: Lab Setup & Automation Framework

> **Credit**: Special thanks to *MyDFIR* on YouTube for providing this outstanding hands-on tutorial series.

### 🧭 Overview

This lab is designed to simulate a real-world Tier 1 SOC environment using **open-source tools** and **automated workflows**. In Part 1, the foundational environment is built, setting the stage for ingesting security events, triggering automated threat intelligence lookups, and managing incidents through structured case tracking.

### 🧱 Architecture & Tool Stack

| Tool        | Role in the Lab                                                  |
|-------------|------------------------------------------------------------------|
| **Wazuh**   | SIEM/EDR – collects Windows security logs and raises alerts      |
| **TheHive** | Incident response platform – organizes cases and investigations  |
| **Shuffle** | SOAR – automates tasks like IOC lookups and alert forwarding     |
| **VirusTotal** | External threat intelligence enrichment                       |
| **Windows 10 VM** | Simulates an endpoint, generates real attack telemetry via Sysmon |

### 🔁 How It Works
### 🚧 Status

> ✅ Part 2 complete: Endpoint telemetry pipeline active and ready for detection testing  
> 🔜 Coming next: Executing test attacks and analyzing alert behavior

---

### 🪜 Part 2: Step-by-Step Breakdown

1. Prepare the Windows 10 VM...
2. Install Sysmon...
...

1. A simulated endpoint (Windows 10 + Sysmon) triggers a suspicious event (e.g., Mimikatz).
2. **Wazuh** detects the event and forwards it for analysis.
3. **Shuffle** parses the alert, automates enrichment tasks (like calling VirusTotal).
4. **TheHive** opens a structured case, giving the analyst a starting point for investigation.

### 🎯 Learning Objectives

- Understand the components of a modern SOC stack
- Deploy and configure open-source tools used in enterprise-grade SOCs
- Automate repetitive investigation steps using SOAR logic
- Practice real-world triage flows, from detection to case management

### 🚧 Status

> ✅ Part 1 complete: Base architecture, data flow, and automation triggers established  
> 🔜 Coming next: Testing real-world attack scenarios (e.g., Mimikatz) to validate pipeline
