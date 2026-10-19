# Case 001: Network Configuration Assessment

**Category:** Networking  
**Environment:** Windows 11 Home  
**Tools:** Command Prompt, ipconfig  
**Status:** Completed — No configuration issue identified

## Objective
Inspect the computer's network configuration and identify its assigned IP address, subnet mask, default gateway, DHCP server, and DNS server.

## Troubleshooting Steps
1. Opened Windows Command Prompt.
2. Executed `ipconfig /all`.
3. Examined the active Ethernet adapter and network settings.
4. Identified the VirtualBox host-only network adapter.

## Findings
- IPv4 address: 192.168.1.74
- Subnet mask: 255.255.255.0
- Default gateway: 192.168.1.1
- DHCP enabled: Yes
- DHCP server: 192.168.1.1
- DNS server: 192.168.1.1
- VirtualBox host-only adapter: 192.168.56.1

## Resolution
No configuration changes were required. The Ethernet adapter had a plausible private IPv4 configuration.

## Verification
Network connectivity and DNS resolution were tested separately in Case 002.

## Skills Demonstrated
TCP/IP configuration, DHCP, DNS configuration, and Windows network diagnostics.

## Evidence
[IP Configuration Screenshot](../02-Network-Troubleshooting/ipconfig.png)

