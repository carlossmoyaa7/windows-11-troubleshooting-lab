\# Windows 11 Troubleshooting Lab



\## Project Overview



This project demonstrates hands-on IT support and troubleshooting skills through a series of practical exercises performed on a Windows 11 computer.



The goal was to develop experience diagnosing network connectivity issues, analyzing Windows system logs, monitoring computer performance, and identifying and repairing corrupted system files.



Each exercise was documented with screenshots, diagnostic results, and troubleshooting notes.



\## Lab Environment



\- \*\*Operating System:\*\* Windows 11 Home

\- \*\*Processor:\*\* AMD Ryzen 7 9800X3D

\- \*\*Memory:\*\* 32 GB DDR5 RAM

\- \*\*Environment:\*\* Local Windows computer

\- \*\*Tools:\*\* Command Prompt, Event Viewer, Task Manager, System File Checker (SFC)



\## Troubleshooting Exercises



\### 1. Network Configuration and Connectivity



\*\*Objective:\*\* Verify network configuration and test local and external connectivity.



\*\*Commands used:\*\*



`ipconfig /all`



`ping 192.168.1.1`



`ping 8.8.8.8`



`nslookup google.com`



\*\*Results:\*\*

\- Verified the computer's IPv4 address, subnet mask, default gateway, DHCP, and DNS configuration.

\- Successfully pinged the default gateway with 0% packet loss and 3 ms average latency.

\- Successfully pinged an external IP address with 0% packet loss and 10 ms average latency.

\- Confirmed DNS resolution for google.com.



\*\*Skills demonstrated:\*\* TCP/IP networking, DNS troubleshooting, DHCP configuration analysis, and network connectivity testing.



\### 2. Windows Event Viewer Analysis



\*\*Objective:\*\* Examine Windows system logs and identify potential system issues.



\*\*Tools used:\*\* Event Viewer



\*\*Results:\*\*

\- Reviewed Windows System event logs.

\- Identified DistributedCOM Warning Event ID 10016.

\- Investigated the warning and determined that it did not establish a confirmed system malfunction.

\- Documented the warning without making unnecessary configuration changes.



\*\*Skills demonstrated:\*\* Event log analysis, Windows diagnostics, and troubleshooting documentation.



\### 3. System Performance Monitoring



\*\*Objective:\*\* Analyze computer performance and resource utilization.



\*\*Tools used:\*\* Windows Task Manager



\*\*Results:\*\*

\- CPU utilization: 7%

\- Memory utilization: 50%

\- Disk utilization: 0%

\- Installed memory: 32 GB DDR5

\- Available memory: 15.6 GB



The captured measurements did not indicate an obvious CPU, disk, or memory bottleneck.



\*\*Skills demonstrated:\*\* Performance monitoring, resource utilization analysis, and basic system diagnostics.



\### 4. Windows System File Repair



\*\*Objective:\*\* Detect and repair protected Windows system file integrity issues.



\*\*Commands used:\*\*



`sfc /verifyonly`



`sfc /scannow`



`sfc /verifyonly`



\*\*Troubleshooting process:\*\*

1\. Initially attempted to run System File Checker without administrator privileges.

2\. Identified the permission requirement and reopened Command Prompt as administrator.

3\. Ran `sfc /verifyonly`, which detected integrity violations.

4\. Executed `sfc /scannow`, which successfully repaired corrupted system files.

5\. Performed a final verification scan.



\*\*Final result:\*\*



Windows Resource Protection did not find any integrity violations.



\*\*Skills demonstrated:\*\* Windows administration, permission troubleshooting, system integrity verification, and repair validation.



\## Project Documentation



Screenshots and troubleshooting documentation are organized into the following directories:



\- `01-System-Information/` — Windows hardware and operating system information

\- `02-Network-Troubleshooting/` — IP configuration, connectivity tests, and DNS resolution

\- `03-System-Diagnostics/` — Event Viewer, Task Manager, and system file repair evidence

\- `04-Ticket-Documentation/` — Troubleshooting case reports and resolutions



\## Key Skills Developed



\- Windows 11 administration and troubleshooting

\- TCP/IP and DNS diagnostics

\- Command-line troubleshooting

\- Windows Event Viewer analysis

\- CPU and memory performance monitoring

\- System File Checker (SFC)

\- Troubleshooting documentation

\- Root cause investigation and verification



\## Conclusion



This project provided hands-on experience with Windows troubleshooting tools commonly used in entry-level IT support environments.



The most significant result was identifying corrupted Windows system files, successfully repairing them, and verifying the repair through a follow-up integrity scan.



The project also reinforced the importance of documenting findings, interpreting diagnostic results, and verifying solutions rather than making assumptions.

