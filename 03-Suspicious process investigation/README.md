# Windows Process Creation Investigation Using Wazuh

## Overview
This practical focuses on monitoring and investigating Windows process creation events using Wazuh. Sysmon or Windows Security auditing can provide process telemetry to help identify unusual executable paths, suspicious command-line activity, and unexpected parent-child process relationships.

## Objectives
- Understand Windows process creation monitoring.
- Collect and investigate Sysmon Event ID 1 or Windows Security Event ID 4688.
- Analyze executable paths, command lines, parent processes, and user context.
- Identify indicators of potentially suspicious process execution.
- Practice evidence-based alert triage and investigation reporting.

## Lab Environment
- SIEM: Wazuh
- Server: Ubuntu
- Endpoint: Windows 11
- Telemetry Source: Sysmon or Windows Security Event Log

## Investigation Workflow
1. Verify that process creation events are being generated on Windows.
2. Configure the Wazuh agent to collect the relevant event channel.
3. Generate normal process activity using applications such as Notepad and Calculator.
4. Search for process creation events in Wazuh.
5. Analyze executable paths, command lines, parent processes, and user accounts.
6. Assess whether the activity is expected or requires further investigation.
7. Document findings and the investigation conclusion.

## Skills Demonstrated
Windows Process Monitoring, Sysmon, Windows Event Logs, Wazuh SIEM, Endpoint Detection, Process Analysis, Security Event Investigation, and SOC Alert Triage.

## Disclaimer
This practical uses benign process activity in a controlled lab. Process creation alone does not establish malicious behavior.
