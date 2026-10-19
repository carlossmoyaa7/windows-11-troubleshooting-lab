# Windows 11 Troubleshooting Lab

### Hands-On IT Support | Windows Administration | System Diagnostics

A hands-on IT support project focused on diagnosing Windows 11 issues, analyzing network connectivity, monitoring system performance, and repairing corrupted system files.

This project demonstrates practical troubleshooting techniques, documentation skills, and problem-solving methods used in entry-level **IT Help Desk and Desktop Support** roles.

---

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Windows 11 Home |
| Processor | AMD Ryzen 7 9800X3D |
| Memory | 32 GB DDR5 |
| Environment | Local Windows desktop |
| Tools | Command Prompt, Task Manager, Event Viewer, SFC |

## Project Objectives

- Diagnose common Windows networking issues.
- Test connectivity and DNS resolution.
- Investigate Windows Event Viewer warnings.
- Monitor CPU and memory utilization.
- Identify and repair Windows system file corruption.
- Document troubleshooting procedures and results.

---

## Troubleshooting Case Studies

| Case | Topic | Result |
|---|---|---|
| [001](04-Ticket-Documentation/Case-001-Network-Configuration.md) | Network Configuration | Completed |
| [002](04-Ticket-Documentation/Case-002-Connectivity-DNS.md) | Connectivity and DNS | Completed |
| [003](04-Ticket-Documentation/Case-003-Event-Viewer.md) | Windows Event Viewer | Investigated |
| [004](04-Ticket-Documentation/Case-004-Performance-Monitoring.md) | Performance Monitoring | Completed |
| [005](04-Ticket-Documentation/Case-005-Memory-Analysis.md) | Memory Analysis | Completed |
| [006](04-Ticket-Documentation/Case-006-System-File-Repair.md) | System File Repair | Resolved |

Each case study includes troubleshooting steps, findings, results, and supporting screenshots.

---

## Featured Case: Windows System File Repair

**Issue:** System File Checker detected Windows system file integrity violations.

**Investigation:**
1. Attempted an SFC integrity scan.
2. Identified the need for administrator permissions.
3. Ran an elevated integrity scan.
4. Confirmed integrity violations were present.

**Resolution:**

Executed `sfc /scannow` in an elevated Command Prompt.

**Verification:**

Ran `sfc /verifyonly` again and confirmed that Windows Resource Protection found no integrity violations.

**Outcome:** Successfully repaired corrupted Windows system files and verified the result.

[View Full Case Study](04-Ticket-Documentation/Case-006-System-File-Repair.md)

---

## Commands Used

| Command | Purpose |
|---|---|
| `ipconfig /all` | Review network adapter configuration |
| `ping 192.168.1.1` | Test local gateway connectivity |
| `ping 8.8.8.8` | Test external network connectivity |
| `nslookup google.com` | Verify DNS resolution |
| `sfc /verifyonly` | Check Windows system file integrity |
| `sfc /scannow` | Scan and repair corrupted system files |

---

## Project Structure

```text
Windows-11-Troubleshooting-Lab/
│
├── README.md
│
├── 01-System-Information/
│
├── 02-Network-Troubleshooting/
│
├── 03-System-Diagnostics/
│
└── 04-Ticket-Documentation/
    ├── Case-001-Network-Configuration.md
    ├── Case-002-Connectivity-DNS.md
    ├── Case-003-Event-Viewer.md
    ├── Case-004-Performance-Monitoring.md
    ├── Case-005-Memory-Analysis.md
    └── Case-006-System-File-Repair.md
```

---

## Skills Demonstrated

**Windows Support:** Windows 11, Command Prompt, administrator privileges, Event Viewer, System File Checker

**Networking:** IPv4, DHCP, DNS, default gateways, connectivity testing

**Diagnostics:** CPU monitoring, memory analysis, system log review, integrity verification

**IT Documentation:** Troubleshooting case reports, evidence collection, problem identification, resolution verification

---

## Project Outcome

Completed six documented troubleshooting exercises involving Windows 11 networking, system diagnostics, performance analysis, and system file repair.

The project includes a successfully resolved Windows system file integrity issue, verified through a follow-up SFC scan.

**Project Focus:** Building practical skills for entry-level IT Help Desk and Desktop Support positions.
