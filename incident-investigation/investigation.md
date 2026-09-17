# Incident Investigation

## Alert 1 — Multiple Failed Logons

| Field | Value |
|---|---|
| Event ID | 4625 |
| Timestamp | Replace with actual value |
| Account | Replace with actual value |
| Failure Reason | Replace with actual value |
| Logon Type | Replace with actual value |
| Workstation | Replace with actual value |
| Source Address | Replace with actual value |
| Initial Severity | Medium |
| Final Assessment | Expected/Benign lab activity |

### Analyst Conclusion

The failed authentication events were intentionally generated during controlled lab testing. The activity should therefore be classified as expected laboratory activity after verification of the account, time, and source context.

## Alert 2 — PowerShell Process Creation

| Field | Value |
|---|---|
| Event ID | 4688 |
| Timestamp | Replace with actual value |
| New Process | Replace with actual value |
| Parent Process | Replace with actual value |
| User | Replace with actual value |
| Process ID | Replace with actual value |
| Initial Severity | Medium |
| Final Assessment | Expected/Benign lab activity |

### Analyst Conclusion

The process-creation event was generated intentionally during controlled testing. PowerShell is a legitimate administrative tool; the event was reviewed in context and classified as expected lab activity.

## Potential IOCs to Record

Do not invent indicators. Record only values observed in the actual events:

- Repeated authentication failures
- Unexpected account
- Unexpected source address
- Unusual login time
- Unexpected process
- Suspicious executable path
- Unexpected parent process
