# 🛡️ Enterprise SOC Lab

A hands-on Security Operations Center (SOC) lab environment for practicing detection engineering, threat hunting, and incident response against real-world attack techniques targeting Active Directory environments.

---

## 📋 Overview

This lab simulates an enterprise Windows environment with a full logging pipeline, SIEM integration, and realistic adversary emulation. All attack simulations are based on real-world TTPs mapped to the MITRE ATT&CK framework.

**Target Audience:** SOC Analysts (Tier 1–3), Detection Engineers, Threat Hunters, Incident Responders

---

## 🏗️ Lab Components

| Component | Description |
|---|---|
| Windows Server 2022 DC | Domain Controller (corp.local) |
| Windows 10/11 Workstations | 3x endpoint clients |
| Kali Linux | Attacker machine |
| Splunk Enterprise | SIEM (v9.x) |
| Sysmon | Endpoint telemetry |
| Winlogbeat | Log shipping |

---

## 📁 Repository Structure

```
enterprise-soc-lab/
├── 01_lab_architecture/       # Network topology & logging pipeline
├── 02_attack_simulations/     # Step-by-step attack walkthroughs
├── 03_detection_engineering/  # SPL queries and detection logic
├── 04_threat_hunting/         # Proactive hunting playbooks
├── 05_soc_dashboards/         # Splunk dashboard screenshots
├── 06_incident_response_playbooks/  # IR runbooks
└── 07_mitre_mapping/          # MITRE ATT&CK coverage matrix
```

---

## 🚀 Quick Start

1. **Set up the lab** – Follow `01_lab_architecture/network_topology.md`
2. **Configure logging** – Follow `01_lab_architecture/logging_pipeline.md`
3. **Run an attack** – Pick a simulation from `02_attack_simulations/`
4. **Detect it** – Apply SPL queries from `03_detection_engineering/`
5. **Hunt proactively** – Use playbooks in `04_threat_hunting/`
6. **Respond** – Follow runbooks in `06_incident_response_playbooks/`

---

## ⚠️ Disclaimer

All techniques in this repository are for **educational and authorized lab use only**. Do not use against systems you do not own or have explicit written permission to test.

---

## 📌 MITRE ATT&CK Techniques Covered

- T1558.003 – Kerberoasting
- T1550.002 – Pass the Hash
- T1021.002 – SMB Lateral Movement
- T1059.001 – PowerShell Abuse

---

## 🤝 Contributing

Pull requests welcome. Please follow the existing format and map all new content to MITRE ATT&CK where applicable.
