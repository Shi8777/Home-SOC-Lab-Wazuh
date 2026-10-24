# Home SOC Lab: Wazuh SIEM & Threat Detection

## Overview
Built a home SOC lab featuring a 3-VM architecture (Kali Linux, Windows, Ubuntu) inside VirtualBox and centralized all log streams into Wazuh SIEM.

## Key Implementation Steps
* **Reconnaissance & Hardening:** Conducted network reconnaissance using Nmap, mapping 10+ open services across 3 hosts, followed by target system hardening and re-scanning to confirm remediation.
* **Network Traffic Analysis:** Captured live traffic using Wireshark to identify protocols and verify attack signatures such as port scans and brute force attempts.
* **Threat Simulation & Detection:** Simulated 2 distinct attack scenarios and authored/tuned 2 detection rules mapped directly to the MITRE ATT&CK framework (T1110 Brute Force, T1046 Network Service Discovery).
* **Incident Reporting:** Published 2 structured incident reports detailing timelines, Indicators of Compromise (IOCs), and step-by-step response procedures.

## Tools & Technologies
* **SIEM:** Wazuh
* **Virtualization:** VirtualBox
* **Operating Systems:** Kali Linux, Windows, Ubuntu
* **Analysis & Scanning:** Wireshark, Nmap
* **Frameworks:** MITRE ATT&CK
