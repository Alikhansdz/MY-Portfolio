# Course 7 — Automate Cybersecurity Tasks with Python

## Overview
Using Python to automate repetitive security tasks including
log parsing, file handling, and security tool automation.

## Key Concepts Learned
- Python fundamentals for security
- Functions, loops, conditionals
- Regular expressions for log parsing
- File I/O — reading and writing security logs
- String manipulation for data parsing
- Debugging Python scripts
- Automating repetitive security tasks

## Key Python Skills Practiced
```python
# Parse failed logins from log file
import re

with open('auth.log', 'r') as f:
    logs = f.read()

failed = re.findall(
    r'Failed password for (\w+) from ([\d.]+)',
    logs
)
for user, ip in failed:
    print(f"Failed login: {user} from {ip}")
```

```python
# Count occurrences of each IP
from collections import Counter

ips = [match[1] for match in failed]
ip_counts = Counter(ips)

for ip, count in ip_counts.most_common(10):
    print(f"{ip}: {count} attempts")
```

## SOC Relevance
Python automation saves hours of manual log analysis.
SOC analysts who can write scripts to parse large log
files and flag suspicious patterns are significantly
more valuable than those who cannot.

## Date Completed
August 4, 2026
