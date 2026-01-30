# Firewall Logging

## Objective
To observe blocked traffic in Windows logs.



## Steps (Windows)

1. Open:
 >  Event Viewer → Windows Logs → Security

2. Enable firewall logging if required.



## Generate Traffic from Kali
Command :
> ping windows-ip

> nc -zv <windows-ip> 445



## Observation
Blocked connection attempts appear in logs.
Logs provide visibility and audit trail.
