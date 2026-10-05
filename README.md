# SOC Analyst Lab - Sysmon + Splunk

## Objective
Build a Windows SOC lab and investigate process activity using Sysmon and Splunk.

## Lab Setup
- VMware Workstation Pro
- Windows 11
- Sysmon
- Splunk Enterprise

## Investigation
Observed process chain:

explorer.exe
→ powershell.exe
→ whoami.exe
→ ipconfig.exe

## Findings
- `whoami.exe` checked the logged-in user.
- `ipconfig.exe` checked network configuration.
- PowerShell launched both processes.

## MITRE ATT&CK
- T1033 - System Owner/User Discovery
- T1016 - System Network Configuration Discovery

## Classification
- Benign Positive
- Severity: Low

## Skills Demonstrated
- Sysmon log analysis
- Splunk searching
- Process investigation
- Timeline analysis
- Alert triage
- MITRE ATT&CK mapping
- Incident documentation

## Conclusion
The activity was intentionally generated for the SOC lab. No malicious activity was confirmed.