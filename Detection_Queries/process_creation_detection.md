# Process Creation Detection

## Event ID
1

## Objective
Monitor newly created processes to identify suspicious execution activity.

## Detection Logic
Sysmon Event ID 1 captures process creation events including:
- Process name
- Parent process
- Command line arguments
- User context

## Example Activity
- powershell.exe
- cmd.exe
- chrome.exe

## Why It Matters
Attackers commonly abuse PowerShell and command shells for execution and persistence.

## Investigation Focus
- Suspicious parent-child process relationships
- Encoded PowerShell commands
- Unexpected command-line arguments
