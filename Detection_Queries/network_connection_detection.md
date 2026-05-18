# Network Connection Detection

## Event ID
3

## Objective
Monitor outbound and inbound network connections to identify suspicious communication activity from endpoints.

---

## Detection Logic
Sysmon Event ID 3 captures network connection events including:
- Source IP address
- Destination IP address
- Source port
- Destination port
- Associated process name

---

## Example Activity
- chrome.exe connecting to external websites
- powershell.exe making outbound connections
- ping.exe generating ICMP traffic

---

## Why It Matters
Attackers often establish outbound connections for:
- Command and Control (C2)
- Malware downloads
- Data exfiltration
- Remote access

Monitoring network connections helps identify suspicious communications and unusual endpoint behavior.

---

## Investigation Focus
- Unexpected outbound connections
- PowerShell network activity
- Connections to unknown external IPs
- Unusual ports and protocols
- Repeated connection attempts

---

## Example Indicators
- powershell.exe connecting externally
- cmd.exe initiating network activity
- Unknown process communicating over the internet

---

## Skills Demonstrated
- Network traffic monitoring
- Endpoint telemetry analysis
- Threat detection
- SOC investigation workflow
- Windows event analysis
