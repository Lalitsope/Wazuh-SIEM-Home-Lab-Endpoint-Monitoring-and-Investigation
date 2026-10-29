Wazuh SOC Home Lab — Hands-on Security Investigations

📌 Project Overview

This project documents my hands-on SOC Analyst L1 practice using Wazuh SIEM. I built a home lab with an Ubuntu-based Wazuh server and a Windows 11 endpoint to practice security monitoring, event analysis, alert investigation, and incident documentation.

The goal is to understand how a SOC analyst monitors endpoint activity, investigates suspicious events, and identifies potential security threats.

🏗️ Lab Architecture

Component

Description

Ubuntu

Wazuh server and dashboard

Windows 11

Endpoint with Wazuh agent

Wazuh SIEM

Security event monitoring and investigation

Sysmon (Practical 3)

Optional source of detailed process telemetry

Log flow: Windows 11 → Wazuh Agent → Ubuntu Wazuh Server → Dashboard Investigation

🔬 Practical Investigations

1. Windows Failed Login Investigation

Objective: Investigate failed authentication attempts and identify patterns consistent with potential brute-force activity.

Activities performed:

Monitored Windows Security events.

Investigated Event ID 4625 (failed logon).

Reviewed usernames, timestamps, source IP addresses, and logon types where available.

Correlated authentication events to assess suspicious login patterns.

Documented investigation findings.

Key skills: Windows Event Log Analysis, Authentication Monitoring, Brute-Force Detection, SIEM Investigation, Alert Triage.

📂 Folder: 01-failed-login-investigation/

2. File Integrity Monitoring (FIM)

Objective: Monitor a Windows directory and investigate file creation, modification, and deletion.

Activities performed:

Configured Wazuh FIM for a dedicated test directory.

Generated controlled file changes.

Investigated file integrity events in the Wazuh dashboard.

Reviewed file paths, timestamps, and available hash information.

Assessed whether file changes were expected or required further investigation.

Key skills: File Integrity Monitoring, Endpoint Security, File Change Detection, Hash Analysis, Event Investigation.

📂 Folder: 02-file-integrity-monitoring/

3. Windows Process Creation Investigation

Objective: Investigate process execution events and understand how endpoint telemetry can help identify suspicious activity.

Activities performed:

Reviewed process creation telemetry using Sysmon Event ID 1 or Windows Security Event ID 4688.

Investigated executable paths, command lines, parent processes, and user context where available.

Examined normal process activity to understand expected behavior.

Practiced identifying process activity that might require additional investigation.

Documented evidence and conclusions.

Key skills: Windows Process Monitoring, Sysmon, Endpoint Detection, Process Analysis, Security Event Investigation.

📂 Folder: 03-process-creation-investigation/

🛠️ Tools and Technologies

Wazuh SIEM

Ubuntu Linux

Windows 11

Wazuh Agent

Windows Event Viewer

Sysmon (for process monitoring, where configured)

File Integrity Monitoring (FIM)

📸 Screenshots and Evidence

Each practical folder can include screenshots showing:

Lab configuration

Relevant Windows events

Wazuh dashboard search results

Alert or event details

Investigation findings

Screenshots should demonstrate actual lab results. Sensitive information, credentials, and private IP details should be redacted before publishing.

🎯 Learning Outcomes

Through these practicals, I am developing skills in:

Security event monitoring and investigation

Windows endpoint log analysis

Authentication anomaly investigation

File integrity monitoring

Process execution analysis

Alert triage and evidence collection

Basic incident documentation and escalation

⚠️ Disclaimer

This project is intended for educational purposes and authorized security testing in a controlled home lab. Testing is limited to systems I own or have permission to investigate.

👨‍💻 Author

Aspiring SOC Analyst L1 | Cybersecurity | Blue Team | SIEM Monitoring | Incident Investigation
