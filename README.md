# Incident Response & Log Analysis Lab

## Overview
This project demonstrates a simulated incident response workflow using Windows system logs and PowerShell-based analysis techniques. The goal is to identify suspicious activity, analyze system events, and document findings in a structured cybersecurity report format aligned with operational intelligence practices.

---

## Objectives
- Detect and analyze suspicious system activity using Windows Event Logs
- Practice incident response workflow (identify → analyze → respond → document)
- Improve log filtering and anomaly detection efficiency
- Produce structured security incident reports

---

## Tools & Technologies
- Windows Event Viewer
- PowerShell
- Virtual Machine (Windows Server / Windows 10)
- Basic log analysis techniques
- Cybersecurity frameworks (NIST Incident Response lifecycle)

---

## Methodology

### 1. Log Collection
System logs were collected from Windows Event Viewer, focusing on:
- Security logs
- System logs
- Application logs

### 2. Event Filtering
PowerShell and built-in filters were used to isolate:
- Failed login attempts
- Unauthorized access patterns
- System errors and anomalies

Example PowerShell command:
```powershell
Get-EventLog -LogName Security -EntryType FailureAudit -Newest 50
