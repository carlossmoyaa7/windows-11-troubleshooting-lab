\# Case 006: Windows System File Integrity Repair



\*\*Category:\*\* Windows System Administration



\*\*Operating System:\*\* Windows 11 Home



\*\*Tools Used:\*\* Command Prompt, System File Checker (SFC)



\*\*Status:\*\* Resolved — Repair successfully verified



\## Problem Description



During a Windows system integrity assessment, System File Checker detected integrity violations affecting protected Windows system files.



The objective was to identify the issue, repair the affected files, and verify that the system passed a follow-up integrity check.



\## Initial Troubleshooting



1\. Opened Windows Command Prompt.

2\. Executed `sfc /verifyonly`.

3\. Received an error indicating that administrator privileges were required.

4\. Reopened Command Prompt using Run as administrator.

5\. Executed `sfc /verifyonly` again.

6\. The scan completed and reported integrity violations.



\## Root Cause Analysis



The initial command failed because Command Prompt was not running with administrator privileges.



After elevating Command Prompt, SFC identified corrupted or inconsistent protected Windows system files. The specific underlying cause of the file integrity violations was not determined.



\## Resolution



Executed the following command in an elevated Command Prompt:



`sfc /scannow`



Windows reported:



"Windows Resource Protection found corrupt files and successfully repaired them."



\## Verification



After the repair, executed:



`sfc /verifyonly`



The verification completed successfully and reported:



"Windows Resource Protection did not find any integrity violations."



\## Outcome



Successfully identified and repaired protected Windows system file integrity violations using System File Checker.



Confirmed the repair by running a follow-up verification scan that detected no remaining integrity violations.



\## Skills Demonstrated



\- Windows troubleshooting

\- Administrator permissions

\- System File Checker (SFC)

\- System integrity diagnostics

\- Windows system file repair

\- Root cause investigation

\- Post-repair verification

\- Technical documentation



\## Evidence



\- \[Administrator Permission Error](../03-System-Diagnostics/sfc-permission-error.png)

\- \[Initial Integrity Violations](../03-System-Diagnostics/sfc-integrity-violations.png)

\- \[Successful SFC Repair](../03-System-Diagnostics/sfc-repair.png)

\- \[Final Verification](../03-System-Diagnostics/sfc-verification.png)

