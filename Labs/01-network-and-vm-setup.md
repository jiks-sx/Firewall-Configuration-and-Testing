# Network and VM Setup

## Objective
To establish connectivity between Windows host and Kali Linux VM.

## Steps

### On Windows
Open Command Prompt:
> ipconfig

Note your IPv4 address.


### On Kali Linux
Open Command Prompt:
> ip a

Confirm Kali IP is in the same subnet.


## Test Connectivity (From Kali)
Open Command(Terminal) Prompt:
> ping <windows-ip>

### Expected Result
Ping should work.
This confirms network connectivity.
