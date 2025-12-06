# 🛡️ Soc Azure Honeypot Project 🛡️ 
![Azure](https://github.com/user-attachments/assets/9c5bc8c5-3cdb-47e8-8285-d3d57efe0f72)


---

## Introduction
- In this project, I built a **basic home SOC in Microsoft Azure** from scratch. Using a free Azure subscription, I deployed a **Windows VM honeypot**, exposed it to the internet, and ingested its logs into **Azure Log Analytics Workspace**. I then integrated **Microsoft Sentinel** to analyze real-world attack traffic and visualize malicious activity.

- This project demonstrates Log analysis, Threat detection, and SOC operations in a real-world cloud environment.

---

## Project Steps

### 1. Azure Resource Setup  
- Created a Windows Virtual Machine (honeypot).  
- Configured networking to allow inbound RDP traffic, exposing the VM to attackers.  
- Configured networking to allow inbound RDP traffic, exposing the VM to attackers.

**VM Setup Overview**
<img width="2559" height="1170" alt="1st pic for azure soc project" src="https://github.com/user-attachments/assets/b3084b34-06cb-4b7d-afcd-483b7fca3657" />

**Resource Group Overview**
<img width="2557" height="1049" alt="2nd pic for azure soc project resource groups overview" src="https://github.com/user-attachments/assets/d6511bd9-2774-41fe-9d58-22789c245297" />

---

### 2. Log Analytics Workspace (LAW)
- Centralized all log data into LAW.  
- Connected the VM’s security logs for collection and monitoring.  
- Connected the VM’s security logs for collection and monitoring.

**Basic KQL LAW Overview (LAW)**
<img width="2553" height="1200" alt="3rd pic for azure soc project LAW" src="https://github.com/user-attachments/assets/0f403daf-0f29-4733-ac29-91fd37a4b133" />

**Advanced KQL LAW Overview (LAW)**
<img width="2304" height="1225" alt="4th pic for azure soc project Advanced LAW" src="https://github.com/user-attachments/assets/ebbf9f6d-3696-48ce-9d99-278a2643f2aa" />


---

### 3. Microsoft Sentinel Integration
- Linked Sentinel with LAW.  
- Built detection rules for failed login attempts.  
- Queried logs with **KQL (Kusto Query Language)**.  
- Queried logs with **KQL (Kusto Query Language)**.

**Watchlist Creation Overview** 
<img width="2259" height="1212" alt="5th pic watchlists" src="https://github.com/user-attachments/assets/7db60f57-4dae-44ad-b2d9-a35dde07de78" />

**Workbook Creation Overview**
<img width="2254" height="887" alt="6th pic workbooks" src="https://github.com/user-attachments/assets/5fee9411-46a7-4a72-8688-0e536c179b86" />

---

### 4. Attack Analysis and Visualization
- Queried failed RDP logins targeting the honeypot.
- Identified IP sources and geolocations.  
- Built a **Sentinel attack map** to visualize attacker origins in real-time.  

**Attack Map (Microsoft Sentinel)**
<img width="1283" height="753" alt="7th pic attack map" src="https://github.com/user-attachments/assets/8d32c536-04c8-4231-a118-64d7deeef4ab" />

**Attack Map (After 1HR) Overview**
<img width="1265" height="713" alt="8th pic finalk" src="https://github.com/user-attachments/assets/9f7494d7-911b-45be-b556-90d7a31023fa" />

---


---
## Key Findings
- Public-facing resources attract brute-force attempts quickly once exposed.
- Microsoft Sentinel offers strong monitoring and near real-time threat tracking.
- KQL proved essential for narrowing security logs and investigating events.
- Implementing security controls such as NSGs, firewalls, and IP restrictions greatly reduced incoming alerts.

---
## Skills Gained
- 🔹 Deployment and configuration of Azure resources with Sentinel integration
- 🔹 Log ingestion and management using Log Analytics Workspace
- 🔹 Crafting and executing KQL queries for threat investigation
- 🔹 Creating dashboards and attack maps for visual threat analysis
- 🔹 Applying defensive security techniques within Azure environments

---
## Conclusion
This project provided practical experience in cloud-based security operations by leveraging a deliberately vulnerable honeypot to collect real attacker telemetry. Using Sentinel and KQL, I was able to monitor, analyze, and visualize malicious activity, reinforcing the value of logging and network hardening strategies in threat detection and response.

This work demonstrates capabilities in:
- **Threat detection & cloud defense**
- **Log analysis**  
- **SOC monitoring workflows**  
- **Cloud security engineering**  

---

## 
---

## 🔗 References  
- [Cyber Home Lab from ZERO and Catch Attackers! Free, Easy, and REAL (Microsoft Sentinel 2025)](https://www.youtube.com/watch?v=g5JL2RIbThM)





