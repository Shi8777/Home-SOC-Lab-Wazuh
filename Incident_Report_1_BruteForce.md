# Incident Report: T1110 Brute Force Attack

## Incident Overview
* **Date:** 2026
* **Detector / SIEM:** Wazuh SIEM
* **Status:** Detected, Analyzed, and Mitigated

## 1. Detection & Timeline
* **Alert Trigger:** Wazuh generated a high-severity alert indicating multiple failed login attempts originating from a suspicious IP address targeting the Windows virtual machine.
* **Timeline:** Anomaly detected at 02:15 AM; triage initiated within 5 minutes.

## 2. Indicators of Compromise (IOCs)
* **Attacker IP:** 192.168.1.105 (Kali Linux VM)
* **Target Service:** SSH / RDP (Port 3389 / 22)
* **Event Logs:** Windows Security Event ID 4625 (An account failed to log on)

## 3. Response & Mitigation Steps
1. **Isolation:** Immediately isolated the affected service endpoint during the simulation phase.
2. **Analysis:** Investigated packet captures using Wireshark to confirm brute-force signatures.
3. **Hardening:** Implemented account lockout policies and tuned Wazuh detection rules (MITRE ATT&CK T1110) to alert instantly on subsequent attempts.
