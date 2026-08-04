# Course 6 — Sound the Alarm: Detection and Response

## Overview
How security teams detect, investigate, and respond to
security incidents using SIEM tools, IDS, and structured
incident response processes.

## Key Concepts Learned
- Incident response lifecycle
  - Preparation → Identification → Containment
  - Eradication → Recovery → Lessons Learned
- SIEM tools — Splunk and Chronicle hands-on
- Writing Splunk SPL queries for threat detection
- Suricata IDS — reading and writing rules
- Network packet analysis with Wireshark
- Log analysis — types and sources
- Incident escalation procedures
- Documentation and chain of custody

## Key Splunk Queries Practiced
```spl
# Failed login detection
index=security EventCode=4625
| stats count by src_ip, user
| where count > 5

# Suspicious outbound traffic
index=network dest_port=4444
| table src_ip, dest_ip, dest_port

# Malware communication detection
index=proxy category=malware
| stats count by src_ip, url
```

## Key Suricata Rule Structure
action protocol src_ip src_port ->
dest_ip dest_port (msg:"Alert name";
sid:1000001; rev:1;)

## SOC Relevance
This is the most directly relevant course to SOC work.
SIEM queries, IDS alerts, and incident response are the
core daily activities of every SOC analyst. Splunk SPL
is used in almost every Pakistani enterprise SOC.

## Date Completed
July 30, 2026 
