# Lab 02 — Brute-Force Detection Using Wazuh Correlation

## Objective

The objective of this lab was to generate multiple failed Windows authentication attempts within a short time period and determine whether Wazuh could correlate the individual events into a higher-severity brute-force alert.

This lab extends Lab 01 by moving from single-event detection to event correlation.

```text
Repeated Failed Logons
        ↓
Windows Event ID 4625
        ↓
Wazuh Agent
        ↓
Multiple Authentication Failure Events
        ↓
Correlation Rule
        ↓
Rule 60204
        ↓
Brute-Force Alert
        ↓
SOC Investigation
```
| Component               | Configuration              |
| ----------------------- | -------------------------- |
| SIEM                    | Wazuh 4.14.x               |
| Wazuh Server            | Ubuntu Server 24.04 LTS    |
| Endpoint                | Windows 11                 |
| Endpoint Name           | WIN-ENDPOINT-01            |
| Virtualization          | Oracle VirtualBox          |
| Authentication Protocol | NTLM                       |
| Log Source              | Windows Security Event Log |
