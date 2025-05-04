
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
---

### 🪜 Part 2: Step-by-Step Breakdown

#### ✅ Goal: Get your Windows endpoint to forward Sysmon logs into Wazuh

---

#### 🪜 Step 1: Prepare the Windows 10 Virtual Machine
- Set up a fresh **Windows 10 VM**
- (Optional) Install **VirtualBox Guest Additions** or **VMware Tools** for easier clipboard/file sharing

---
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

---

## 📌 Part 2: Endpoint Telemetry & SIEM Integration

🎥 [Watch Part 2](https://youtu.be/YxpUx0czgx4?si=DLSAAvLUZrr-cCxa)

### 🧭 Overview

In Part 2, the focus shifts to configuring the Windows 10 endpoint to generate detailed telemetry using Sysmon and integrating this data into the Wazuh SIEM. This is a critical step in building a functioning SOC lab because it lays the groundwork for capturing suspicious behavior and triggering automated workflows.

### 🛠️ Tools and Configuration

- **Sysmon**: A Windows tool that logs detailed system activity (process creation, network connections, file changes).
- **Wazuh Agent**: Installed on the Windows 10 VM to forward logs to the Wazuh server.
- **Wazuh Manager**: Parses logs from the agent, correlates events, and applies detection rules.

### ⚙️ Workflow Recap

1. Sysmon logs process execution and other key system behaviors.
2. Wazuh Agent forwards these logs to the Wazuh server.
3. Alerts are generated based on detection rules for known malicious behavior.

### 🎯 Learning Objectives

- Install and configure Sysmon for endpoint visibility
- Deploy and connect the Wazuh Agent
- Understand the log flow and detection rule processing
- Prepare the lab for real-world attack simulation (e.g., Mimikatz)

### 🚧 Status

> ✅ Part 2 complete: Endpoint telemetry pipeline active and ready for detection testing  
> 🔜 Coming next: Executing test attacks and analyzing alert behavior

---

### 🪜 Part 2: Step-by-Step Breakdown

#### ✅ Goal: Get your Windows endpoint to forward Sysmon logs into Wazuh

#### 🪜 Step 1: Prepare the Windows 10 Virtual Machine
- Set up a fresh **Windows 10 VM**
- (Optional) Install **VirtualBox Guest Additions** or **VMware Tools** for easier clipboard/file sharing

#### 🪜 Step 2: Install Sysmon
- Download `Sysmon.exe` from Microsoft’s Sysinternals Suite
- Use a trusted config file like `sysmon-config.xml` from [SwiftOnSecurity’s GitHub](https://github.com/SwiftOnSecurity/sysmon-config)
- Install using:
  ```powershell
  sysmon.exe -accepteula -i sysmon-config.xml
  ```
- Once running, Sysmon will log:
  - Process creation
  - Network connections
  - File creation timestamps
  - Registry events

#### 🪜 Step 3: Install the Wazuh Agent
- Download the **Wazuh Agent for Windows** from [Wazuh’s download page](https://wazuh.com/download/)
- During setup:
  - Input your Wazuh Manager’s IP address
  - Choose a unique agent name (e.g., `win10-lab`)
  - Accept the default group or select a policy if available

#### 🪜 Step 4: Start the Agent & Confirm Connection
- Start the agent:
  ```powershell
  sc start wazuh-agent
  ```
- Log into your **Wazuh dashboard**
- Confirm the Windows agent appears as **connected**

#### 🪜 Step 5: Validate Sysmon Logs in Wazuh
- Perform basic tasks on the Windows VM (e.g., open Notepad, run PowerShell)
- In Wazuh → go to **Security Events** or **Logs**
- Look for:
  - **Event ID 1** – Process creation
  - **Event ID 3** – Network connections
  - **Event ID 11** – File creation

#### 🧠 Bonus: Customize Detection Rules
- Review Wazuh rules for Sysmon event types
- Adjust detection thresholds or write custom rules for better visibility
- This prepares you for alert automation using **Shuffle** in the next part

---

## 📌 Part 3: Attack Simulation & Automated Alerting

🎥 [Watch Part 3](https://youtu.be/VuSKMPRXN1M?si=DieWa0WIDELuj0Ac)

### 🧭 Overview

In Part 3, we simulate a real-world attack using **Mimikatz** to test the detection and automation capabilities of our SOC setup. This exercise validates the integration between **Sysmon**, **Wazuh**, **Shuffle**, and **TheHive**.

### 🪜 Step-by-Step Breakdown

#### 🧪 Step 1: Simulate an Attack with Mimikatz
- **Objective**: Generate malicious activity on the Windows 10 VM.
- **Action**: Execute Mimikatz to simulate credential dumping.
- **Result**: Sysmon logs the suspicious activity, capturing details like process creation and command-line arguments.

#### 📤 Step 2: Sysmon Logs Forwarded to Wazuh
- **Objective**: Ensure Sysmon logs reach the SIEM.
- **Action**: Wazuh Agent on the Windows VM forwards logs to the Wazuh Manager.
- **Result**: Wazuh processes the logs and applies detection rules.

#### 🚨 Step 3: Wazuh Detects and Alerts
- **Objective**: Detect the simulated attack.
- **Action**: Wazuh's rules identify Mimikatz activity based on process names and behaviors.
- **Result**: An alert is generated within Wazuh.

#### 🔁 Step 4: Shuffle Automates Response
- **Objective**: Automate incident response.
- **Action**: Shuffle receives the alert from Wazuh and initiates a predefined workflow.
  - Queries **VirusTotal** for additional context.
  - Creates a case in **TheHive** with relevant details.
- **Result**: The incident is enriched and documented automatically.

#### 📂 Step 5: TheHive Case Management
- **Objective**: Manage and investigate the incident.
- **Action**: TheHive receives the case from Shuffle, containing:
  - Alert details from Wazuh.
  - Enrichment data from VirusTotal.
- **Result**: Analysts can now investigate and respond to the incident within TheHive.

### 🎯 Learning Objectives

- Understand how simulated attacks can test SOC detection capabilities.
- Observe the flow of data from detection to automated response.
- Validate the integration between Sysmon, Wazuh, Shuffle, and TheHive.

#### 🪜 Step 2: Install Sysmon
- Download `Sysmon.exe` from Microsoft’s Sysinternals Suite
- Use a trusted config file like `sysmon-config.xml` from [SwiftOnSecurity’s GitHub](https://github.com/SwiftOnSecurity/sysmon-config)
- Install using:
  ```powershell
  sysmon.exe -accepteula -i sysmon-config.xml
