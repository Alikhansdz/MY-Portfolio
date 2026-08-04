# Course 4 — Tools of the Trade: Linux and SQL

## Overview
Practical hands-on skills in Linux command line and SQL
database querying — two essential tools for security analysts.

## Key Linux Commands Learned
```bash
# Navigation
pwd / ls / cd / mkdir / rm / cp / mv

# File operations  
cat / grep / find / chmod / chown

# Process management
ps aux / kill / top / systemctl

# Network commands
ping / traceroute / netstat / ifconfig

# User management
sudo / useradd / passwd / /etc/passwd
```

## Key SQL Concepts
```sql
-- Basic queries
SELECT * FROM logs WHERE event_type = 'failed_login';

-- Filtering
SELECT user, COUNT(*) FROM auth_logs 
WHERE status = 'failed'
GROUP BY user
HAVING COUNT(*) > 5;
```

## SOC Relevance
Linux is the OS of most servers and security tools. SQL is
used to query security databases and SIEM backends. Both
are used daily in SOC investigations.

## Date Completed
July 9, 2026
