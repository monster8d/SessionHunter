# SessionHunter

<p align="center">
  <img src="docs/images/icon.png" width="220">
</p>

<h3 align="center">
Reconstruct Every Session. Trace Every Action. Prove Every Event.
</h3>

<p align="center">
Enterprise Digital Forensics & Incident Response Platform
</p>

---

## Overview

SessionHunter is an advanced Digital Forensics & Incident Response (DFIR) platform designed to reconstruct user activity across Linux infrastructure.

The platform enables investigators, SOC teams, CERT teams, internal audit teams, and forensic analysts to determine:

- Who logged in
- From where they connected
- Which commands they executed
- Which files were accessed
- Which files were modified
- What persistence mechanisms were created
- Whether data was exfiltrated
- What happened before, during, and after an incident

Unlike traditional log viewers, SessionHunter correlates multiple forensic artifacts into a unified investigation timeline.

---

## Dashboard

![Dashboard](docs/images/dashboard.png)

The dashboard provides:

- Host inventory
- Event timeline
- Session correlation
- Geo-IP intelligence
- Actor attribution
- Evidence search
- Live forensic collection

---

## Interactive Timeline Reconstruction

![Timeline](docs/images/timeline.png)

SessionHunter reconstructs activity from:

- SSH logs
- Auditd
- Journalctl
- Bash History
- Sudo Logs
- Auth Logs
- System Logs

Analysts can investigate:

- User sessions
- Source IPs
- Authentication methods
- Commands executed
- Timeline context

---

## Investigation Map

![Map](docs/images/map.png)

Visualize:

- Login locations
- Source IP clustering
- User activity by geography
- High-risk locations
- Geo-IP intelligence

---

## Session Reconstruction

Determine:

- Login time
- Logout time
- Source IP
- User account
- TTY used
- Session duration
- Commands executed

Supported sources:

- Auditd
- SSH
- Bash
- ZSH
- Journalctl
- Sudo

---

## File Access & Modification Analysis

Investigate:

- Files modified
- Sensitive files accessed
- Recently changed files
- Ownership changes
- Permission changes
- Webroot modifications

Examples:

- /etc/passwd
- /etc/shadow
- /etc/sudoers
- SSH keys
- Web application files

---

## Authentication & Account Forensics

Analyze:

- SSH activity
- Failed logins
- Brute force attempts
- New users
- Privilege escalation
- Sudo execution
- Account modifications

---

## Process & Memory Forensics

Investigate:

- Running processes
- Suspicious executables
- Parent-child relationships
- Deleted binaries
- Open handles
- Memory artifacts

Compatible with:

- AVML
- LiME
- Volatility

---

## Network Forensics

Analyze:

- Established connections
- Listening services
- DNS configuration
- Routing tables
- ARP cache
- Firewall rules

Detect:

- Reverse shells
- Unauthorized listeners
- External communications
- Suspicious endpoints

---

## Persistence Hunting

Detect:

- Cron jobs
- Systemd services
- Timers
- Startup scripts
- SSH key persistence
- Shell profile persistence
- LD_PRELOAD abuse

---

## Filesystem & Malware Hunting

Capabilities:

- Hidden files
- Executables in temp folders
- SUID binaries
- SGID binaries
- Linux capabilities
- YARA scanning
- Malware indicators

---

## Log Forensics

Analyze:

- auth.log
- secure
- syslog
- journalctl
- kernel logs
- application logs

Build complete incident timelines.

---

## Web Server Forensics

Supported:

- Apache
- Nginx
- PHP
- PHP-FPM

Investigate:

- Web shells
- Suspicious uploads
- Command execution
- SQL injection attempts
- Path traversal attempts

---

## Package & Software Analysis

Identify:

- Recently installed software
- Unauthorized packages
- Package integrity violations
- Dependency abuse

Supported:

- RPM
- DNF
- YUM
- APT
- DPKG

---

## Data Exfiltration Detection

Detect:

- SCP transfers
- SFTP usage
- Rsync activity
- Rclone
- Cloud uploads
- Archive creation

Indicators include:

- Large archives
- Recent exports
- External transfers
- Data staging activity

---

## Container Forensics

Supported:

- Docker
- Kubernetes

Investigate:

- Container modifications
- Runtime changes
- Privileged containers
- Suspicious images
- Kubernetes events

---

## Architecture

Agent Philosophy:

> Agent is a Sensor. Server is the Analyst.

The endpoint performs lightweight collection while forensic intelligence remains centralized.

Benefits:

- Low endpoint footprint
- Reduced attack surface
- Centralized correlation
- Faster investigations

---

## Intended Users

- DFIR Teams
- SOC Analysts
- CERT Teams
- Government Agencies
- Internal Audit Teams
- Incident Responders
- Security Operations Centers

---

## License

Proprietary Software

Copyright © SessionHunter
