# Incident Report: T1046 Network Service Discovery (Port Scan)

## Incident Overview
* **Date:** 2026
* **Detector / SIEM:** Wazuh SIEM & Nmap
* **Status:** Analyzed and Documented

## 1. Detection & Timeline
* **Alert Trigger:** Nmap stealth and SYN scans executed against target hosts, captured and flagged by Wazuh and Wireshark.
* **Timeline:** Scan initiated and successfully logged, mapping over 10 open services across 3 virtual machines.

## 2. Indicators of Compromise (IOCs)
* **Scanner Source:** Kali Linux VM
* **Scanned Targets:** Windows and Ubuntu VMs
* **Signatures:** Rapid TCP SYN packets directed across multiple sequential ports.

## 3. Response & Mitigation Steps
1. **Identification:** Mapped out all exposed ports and verified unauthorized reconnaissance activity.
2. **Hardening:** Closed unused ports, tightened local firewall configurations, and re-scanned to confirm remediation.
3. **Rule Tuning:** Validated detection rules mapped to MITRE ATT&CK framework (T1046).
