# PowerShell Activity Detection

## Event ID
1

## Objective
Monitor PowerShell execution activity to identify suspicious scripting behavior and potential attacker techniques.

---

## Detection Logic
Sysmon Event ID 1 captures process creation events including:
- Process name
- Command-line arguments
- Parent process
- User account context

The focus of this investigation was monitoring powershell.exe activity.

---

## Example Activity
- Opening PowerShell manually
- Running basic PowerShell commands
- Executing administrative tasks
- Monitoring command execution behavior

---

## Why It Matters
PowerShell is commonly abused by attackers for:
- Fileless malware execution
- Remote command execution
- Persistence mechanisms
- Downloading malicious payloads
- Privilege escalation

Monitoring PowerShell activity is critical in SOC environments.

---

## Investigation Focus
- Suspicious PowerShell execution
- Encoded commands
- Unusual parent-child relationships
- Administrative PowerShell usage
- Network-enabled PowerShell commands

---

## Example Indicators
- powershell.exe launched from cmd.exe
- Encoded command execution
- PowerShell spawning child processes
- External network communication from PowerShell

---

## Skills Demonstrated
- Endpoint monitoring
- Process investigation
- Threat hunting fundamentals
- Windows telemetry analysis
- SOC alert investigation
