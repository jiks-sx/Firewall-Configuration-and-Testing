# Blocking Kali IP Address

## Objective
To simulate containment of suspicious activity.



## Steps (Windows)

1. Create New Inbound Rule
2. Scope → Remote IP address
3. Add Kali IP
4. Action: Block



## Test from Kali
Commands:
> ping windows-ip

> nc -zv <windows-ip> 22

### Expected Result
All traffic blocked.



## Security Insight
IP blocking is useful for temporary containment.
