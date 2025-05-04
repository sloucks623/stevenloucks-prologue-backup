---
title: "Lab 1.0 – SOC Automation Home Lab"
layout: post
---

## Lab 1.0 – SOC Automation Home Lab

🎯 **Objective**:  
To simulate and explore the Tier 1 SOC Analyst role using freely available tools, with an emphasis on *automating routine alert triage and threat investigation workflows*.

🔧 **Tools Used**:
- Wazuh
- Sysmon
- TheHive
- Shuffle (SOAR)
- VirusTotal
- Windows 10 VM

📚 **Overview**:  
This lab recreates the investigative flow a SOC analyst follows when responding to potential security alerts. The emphasis is on *learning by doing* while also identifying opportunities for **automation** in tasks like IOC lookups, reputation checking, and documentation formatting.

The project is based on guidance from the video series by **MyDFIR**:  
🎥 [SOC Automation Lab Walkthrough – YouTube](https://youtu.be/XR3eamn8ydQ?si=WLR8_IjbkIGodCc5)  
💬 *Special thanks to MyDFIR for providing this outstanding hands-on tutorial series.*

---

## 📌 Part 1: Lab Setup & Automation Framework

### 🧭 Overview
Introduces the lab and toolset for simulating a Tier 1 SOC environment.

### 🧱 Architecture & Tool Stack
| Tool        | Role                                      |
|-------------|--------------------------------------------|
| Wazuh       | SIEM/EDR for log ingestion and alerting    |
| TheHive     | Incident case management                   |
| Shuffle     | SOAR automation between tools              |
| VirusTotal  | Threat enrichment for IOCs                 |
| Windows 10  | Endpoint for telemetry and attack simulation |

### 🔁 Flow Summary
1. Sysmon logs system activity on the Windows VM.
2. Wazuh ingests these logs.
3. Alerts trigger automated workflows in Shuffle.
4. Shuffle queries VirusTotal and creates cases in TheHive.

### 🎯 Objectives
- Learn tool integrations for detection & response
- Practice SOC triage and incident automation

---

## 📌 Part 2: Endpoint Telemetry & SIEM Integration

🎥 [Watch Part 2](https://youtu.be/YxpUx0czgx4?si=DLSAAvLUZrr-cCxa)

### 🧭 Overview
Configuring the Windows 10 VM with Sysmon and connecting it to Wazuh.

### 🪜 Step-by-Step
1. Set up Windows 10 VM.
2. Install Sysmon with config.
3. Install and configure Wazuh agent.
4. Confirm Wazuh is ingesting Sysmon events (IDs 1, 3, 11).

---

## 📌 Part 3: Attack Simulation & Automated Alerting

🎥 [Watch Part 3](https://youtu.be/VuSKMPRXN1M?si=DieWa0WIDELuj0Ac)

### 🧭 Overview
Run Mimikatz to simulate credential theft and validate alert generation + automation.

### 🪜 Step-by-Step
1. Run Mimikatz on the VM.
2. Wazuh logs and alerts.
3. Shuffle responds: enriches via VirusTotal, creates TheHive case.
4. Validate that data flows through the full pipeline.

---

## 📌 Part 4: Custom Detection Rules & Advanced Alerting

🎥 [Watch Part 4](https://youtu.be/amTtlN3uvFU?si=MZzUMpAihcALguaF)

### 🧭 Overview
Detect renamed or obfuscated threats using custom rules.

### 🪜 Step-by-Step
1. Rename Mimikatz to `notavirus.exe`.
2. Update Wazuh config for log archiving.
3. Create `local_rules.xml` rule matching original filename.
4. Test and confirm alert fires.

---

## 📌 Part 5: Advanced Telemetry & Rule Validation

🎥 [Watch Part 5](https://youtu.be/GNXK00QapjQ?si=P2KyGpLFmAk9K0PO)

### 🧭 Overview
Fine-tune telemetry inputs and detection logic.

### 🪜 Step-by-Step
1. Refine log source configs.
2. Re-test Mimikatz obfuscation.
3. Enhance rules for broader detection.
4. Validate alerts in Wazuh & TheHive.

---

## 🖼️ Supporting Diagrams & Slides

### 🧱 Lab Architecture Diagram
![SOC Lab Architecture Diagram](assets/images/soc-architecture.png)
> *Visual overview of how Wazuh, Shuffle, TheHive, and Sysmon integrate.*

---

### 🔁 Automation Workflow Diagram
![SOC Automation Flow](assets/images/shuffle-workflow.png)
> *Step-by-step automation: from alert detection to enrichment and case creation.*

---

### 📂 Presentation Slides
- [SOC Automation Lab – Slide Deck (PDF)](assets/slides/soc-lab-summary.pdf)
- [Wazuh Rule Customization Cheatsheet (PDF)](assets/slides/wazuh-rules-cheatsheet.pdf)
