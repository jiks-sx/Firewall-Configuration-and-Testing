# Port Allow and Deny 

## Objective
To control access using firewall rules.



## Steps (Windows)

1. Open:
   Windows Defender Firewall → Advanced settings

2. Create New Inbound Rule:
   - Type: Port
   - Protocol: TCP
   - Port: 22 (example)
   - Action: Allow



## Test from Kali
Command:
> nc -zv <windows-ip> 22

### Expected Result
> Connection succeeds.



## Block a Port
Create inbound rule → Block TCP port 445

Test again from Kali:
Command:
> nc -zv windows-ip 445

### Expected Result
> Connection fails.
