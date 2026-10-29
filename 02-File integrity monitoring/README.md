# File Integrity Monitoring Using Wazuh

## Overview
This practical demonstrates how to configure and validate File Integrity Monitoring (FIM) on a Windows 11 endpoint using Wazuh. The lab monitors a dedicated test directory and investigates file creation, modification, and deletion events.

## Objectives
- Configure Wazuh FIM to monitor a Windows directory.
- Detect file creation, modification, and deletion.
- Review file paths, timestamps, and available file hashes.
- Investigate unexpected file changes and assess their potential security impact.
- Document findings as part of a SOC investigation.

## Lab Environment
- SIEM: Wazuh
- Server: Ubuntu
- Endpoint: Windows 11
- Feature: File Integrity Monitoring
- Test Directory: C:\SOC-Lab

## Investigation Workflow
1. Create a dedicated test directory and sample files.
2. Configure real-time FIM monitoring through the Wazuh agent.
3. Restart the agent and verify the monitoring configuration.
4. Create, modify, and delete test files.
5. Review the resulting events in the Wazuh dashboard.
6. Examine file paths, timestamps, and available hash information.
7. Document whether the changes were expected or require further investigation.

## Skills Demonstrated
File Integrity Monitoring, Endpoint Monitoring, File Change Detection, Hash Analysis, Wazuh Agent Configuration, Event Investigation, and Incident Documentation.

## Disclaimer
This practical was performed using test files in an authorized lab environment.
