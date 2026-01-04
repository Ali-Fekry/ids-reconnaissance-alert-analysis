# IDS Reconnaissance Alert Analysis

## Overview
This project demonstrates hands-on IDS alert analysis by detecting reconnaissance activity through network traffic inspection.

## Objective
- Identify suspicious network behavior
- Validate IDS alerts
- Recommend containment actions

## Tools Used
- Nmap
- tcpdump
- Linux (Ubuntu / WSL)

## Attack Scenario
A TCP SYN port scan was executed against the target system, generating abnormal traffic indicative of reconnaissance activity.

## Evidence
- Nmap Scan: evidence/nmap-scan.txt
- Packet Capture: evidence/tcpdump-capture.txt

## Analysis
- Rapid scanning across multiple ports
- Single source IP
- No successful exploitation

## MITRE ATT&CK
- Tactic: Reconnaissance
- Technique: Active Scanning (T1595)

## Outcome
The alert was classified as a true positive reconnaissance event and containment actions were recommended.

## Author
Ali Fekry  
Entry-Level SOC / IT Monitoring Analyst

