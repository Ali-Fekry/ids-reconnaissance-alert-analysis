🛡️ IDS Alert Analysis – Reconnaissance Activity
📌 Overview

This project simulates a SOC investigation of IDS alerts triggered by reconnaissance activity. The objective is to identify abnormal network behavior, analyze evidence, map the activity to MITRE ATT&CK, and recommend containment actions.

🚨 Alert Description

An IDS alert was generated due to multiple TCP connection attempts across different ports from a single source IP within a short time window.

🔍 Investigation & Evidence

Tool used: nmap, tcpdump

Observed multiple SYN packets targeting sequential ports

No application-level session established

Open service discovered: SSH (port 22)

🧠 Analysis

Activity identified as port scanning

Behavior matches early-stage reconnaissance

No successful exploitation observed

🧩 MITRE ATT&CK Mapping

Tactic: Reconnaissance

Technique: Active Scanning (T1595)

⚠️ Severity

Low to Medium — early attack stage with potential risk escalation.

🧯 Recommended Response Actions

Block or rate-limit the source IP

Tune IDS signatures to detect scan patterns

Monitor for exploitation attempts

Escalate if repeated or targeting critical systems

📘 Lessons Learned

Early detection of reconnaissance allows organizations to prevent exploitation before system compromise occurs.
