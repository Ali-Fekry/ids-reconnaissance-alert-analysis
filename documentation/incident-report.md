# IDS Alert Analysis – Reconnaissance Activity

## Incident Summary
Multiple TCP SYN packets were detected from a single source IP within a short time window, indicating reconnaissance activity.

## Detection Method
- Network traffic captured using tcpdump
- Port scanning performed using Nmap
- Behavioral IDS-style analysis

## Indicators of Compromise (IOCs)
- Source IP: 172.25.73.208
- Activity: Port scanning
- Protocol: TCP

## Analysis
Rapid connection attempts across multiple ports without establishing full sessions were observed. This behavior matches reconnaissance activity rather than normal application traffic.

## MITRE ATT&CK Mapping
- Tactic: Reconnaissance
- Technique: Active Scanning (T1595)

## Severity
Low to Medium – No exploitation detected.

## Recommended Containment Actions
- Temporarily block the source IP
- Enable IDS/IPS rate-limiting rules
- Monitor for repeated scanning behavior

## Lessons Learned
Early detection of reconnaissance activity helps prevent future exploitation and improves network security posture.
