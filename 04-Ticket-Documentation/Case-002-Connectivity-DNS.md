# Case 002: Network Connectivity and DNS Verification

**Category:** Networking  
**Environment:** Windows 11 Home  
**Tools:** Command Prompt, ping, nslookup  
**Status:** Completed — Tests passed

## Objective
Verify communication with the local gateway, an external IP address, and a DNS resolver.

## Troubleshooting Steps
1. Executed `ping 192.168.1.1` to test the local gateway.
2. Executed `ping 8.8.8.8` to test external IP connectivity.
3. Executed `nslookup google.com` to verify DNS resolution.
4. Reviewed the responses and packet statistics.

## Findings
**Local gateway:**
- Packets sent: 4
- Packets received: 4
- Packet loss: 0%
- Average latency: 3 ms

**External connectivity:**
- Packets sent: 4
- Packets received: 4
- Packet loss: 0%
- Average latency: 10 ms

**DNS:**
- Successfully resolved google.com to IPv4 and IPv6 addresses.
- DNS server: 192.168.1.1
- The server hostname displayed as Unknown, but DNS resolution succeeded.

## Resolution
No connectivity issue was identified during testing. No changes were required.

## Verification
All three diagnostic tests completed successfully.

## Skills Demonstrated
Network connectivity testing, DNS resolution, ping analysis, and TCP/IP troubleshooting.

## Evidence
- [Gateway Ping](../02-Network-Troubleshooting/gateway-ping.png)
- [External Ping](../02-Network-Troubleshooting/external-ping.png)
- [DNS Lookup](../02-Network-Troubleshooting/dns-lookup.png)


