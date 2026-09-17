# SOC Lab Implementation

A beginner-friendly, controlled Security Operations Center (SOC) lab focused on defensive security monitoring, Windows event logs, detection rules, alert investigation, and incident documentation.

## Objectives

- Collect and inspect Windows security logs
- Generate controlled authentication and process events
- Analyze Event ID 4625 and Event ID 4688
- Create basic detection rules
- Investigate alerts and identify potential IOCs
- Assign an initial severity and document findings
- Recommend defensive security improvements

## Lab Environment

- Windows 11 Home
- Windows Event Viewer
- PowerShell
- Windows Audit Policy / `auditpol`
- Optional: Sysmon

## Lab Workflow

```text
Controlled Activity
       ↓
Windows Event Logs
       ↓
Event Analysis
       ↓
Detection Rules
       ↓
Alert
       ↓
Investigation
       ↓
IOC / Severity
       ↓
Documentation
```

## Events Investigated

### Event ID 4625 — Failed Logon

Used to investigate failed authentication attempts.

Detection example:

> 5 or more failed logons within 5 minutes → generate an alert for investigation.

### Event ID 4688 — Process Creation

Used to investigate newly created processes.

Detection example:

> PowerShell process creation → generate an alert for review.

PowerShell is legitimate software, so the event is not automatically malicious. Context and correlation are required.


## Detection Rules

See [`detection-rules/rules.md`](detection-rules/rules.md).

## Incident Investigation

See [`incident-investigation/investigation.md`](incident-investigation/investigation.md).

## Important Note

All events in this project are generated and analyzed in an authorized personal/test environment. Expected lab activity should not be presented as a real security incident.
