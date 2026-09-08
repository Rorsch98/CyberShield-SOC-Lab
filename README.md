# CyberShield SOC Lab

CyberShield is a hands-on Security Operations Center (SOC) lab built to develop practical skills in SIEM administration, security monitoring, threat detection, log analysis, and incident investigation.

The lab uses a self-hosted Wazuh environment to monitor endpoints and investigate security events generated inside a controlled environment.

## Lab Environment

- Wazuh SIEM 4.14.x
- Ubuntu Server 24.04 LTS
- Windows 11 endpoint
- Wazuh Windows Agent
- Oracle VirtualBox
- Windows Security Event Logs
- SSH administration

## Current Architecture

```text
Windows Endpoint
   WIN-ENDPOINT-01
          |
          | Wazuh Agent
          v
   Wazuh Manager
          |
          v
   Wazuh Indexer
          |
          v
   Wazuh Dashboard
          |
          v
   SOC Investigation
