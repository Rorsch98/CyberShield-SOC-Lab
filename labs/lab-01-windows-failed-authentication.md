# Lab 01 — Windows Failed Authentication Detection

## Objective

The objective of this lab was to generate a controlled Windows authentication failure, collect the corresponding Windows Security event using the Wazuh agent, detect the activity through Wazuh SIEM, and investigate the resulting alert.

This lab demonstrates the basic SOC workflow:

```text
Event Generation
      ↓
Log Collection
      ↓
Detection
      ↓
SIEM Alert
      ↓
Investigation
      ↓
Analyst Assessment

```
## Screenshots

### Wazuh Agent Connected

![Wazuh Agent Active](../screenshots/lab-01/01-agent-active.png)

### Failed Authentication Alert

![Failed Authentication Alert](../screenshots/lab-01/02-4625-alert.png)

### Event Details

![Event Details](../screenshots/lab-01/03-event-details.png)
