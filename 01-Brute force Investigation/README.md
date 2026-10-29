# Windows Failed Login Investigation Using Wazuh SIEM

## Overview
This practical focuses on detecting and investigating failed Windows authentication attempts using Wazuh SIEM. The lab uses a Windows 11 endpoint connected to a Wazuh server running on Ubuntu to collect and analyze Windows Security events.

## Objectives
- Monitor Windows authentication events using Wazuh.
- Identify failed logon attempts using Windows Event ID 4625.
- Investigate usernames, source IP addresses, timestamps, and logon types.
- Correlate multiple failed attempts to identify potential brute-force activity.
- Practice SOC Analyst L1 alert triage and incident documentation.

## Lab Environment
- SIEM: Wazuh
- Server: Ubuntu
- Endpoint: Windows 11
- Log Source: Windows Security Event Log

## Investigation Workflow
1. Verify Windows agent connectivity to the Wazuh server.
2. Generate controlled failed login attempts on the lab endpoint.
3. Search for Event ID 4625 in Wazuh.
4. Analyze event details and identify suspicious authentication patterns.
5. Assess the evidence and document the investigation findings.

## Skills Demonstrated
Wazuh SIEM, Windows Event Log Analysis, Authentication Monitoring, Brute-Force Detection, Alert Triage, Incident Investigation, and Security Event Correlation.

## Disclaimer
This practical was conducted in a controlled lab environment for educational purposes.
