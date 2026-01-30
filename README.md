# Task 10: Firewall Configuration & Testing  
## (Windows Host + Kali Linux in VMware)

---

## Overview

This repository documents **Task 10: Firewall Configuration & Testing**
performed as part of a cybersecurity internship.

The task focuses on **understanding firewall concepts deeply** and
**performing hands-on practical testing** using:

- **Windows laptop as the firewall-protected system**
- **Kali Linux (VMware) as a controlled testing machine**

The firewall used in this task is **Windows Defender Firewall**.
All testing is performed in an **isolated, legal, and safe lab environment**.

---

## Lab Environment

### Systems Used

| System | Role |
|------|-----|
| **Windows (Host OS)** | Firewall-configured system |
| **Kali Linux (VMware)** | Network testing machine |

---

### Network Configuration

- VMware Network Mode: **Host-Only Adapter** (preferred)
- No direct internet exposure
- Example IPs:
  - Windows Host: `192.168.XX.XXX`
  - Kali Linux VM: `192.168.XX.XX`

This setup ensures ethical testing and prevents accidental access
to external systems.

---

## Objectives

The objectives of this task are:

- Understand firewall fundamentals and working principles
- Study how **Windows Defender Firewall** filters network traffic
- Learn **stateful firewall behavior**
- Configure inbound firewall rules
- Allow and block specific network ports
- Test firewall rules from Kali Linux
- Observe blocked and allowed traffic
- Analyze firewall logs
- Simulate IP-based blocking
- Understand firewall impact and limitations

---

## Tools & Technologies Used

- **Windows Defender Firewall**
- **Windows Event Viewer** (log analysis)
- **Kali Linux (VMware)**
- Kali Linux tools:
  - `ping` – connectivity testing
  - `nmap` – port visibility testing (local lab only)
  - `netcat (nc)` – port allow/deny verification
- VMware Workstation / Player

---

## Key Firewall Concepts Covered

### Firewall Fundamentals
- Network traffic filtering
- Trust boundary between systems
- Default deny principle
- Least privilege networking

---

### Stateful Firewall Behavior
- Connection tracking
- Session awareness
- Automatic handling of return traffic

---

### Inbound Firewall Rules
- Controlling incoming traffic
- Port-based access control
- Reducing attack surface

---

### Firewall Logging & Monitoring
- Visibility into blocked connections
- Understanding traffic patterns
- Supporting investigation and troubleshooting

---

### IP Blocking
- Blocking a specific source IP
- Temporary containment of suspicious activity
- Understanding limitations of IP-based filtering

---

## Practical Activities Performed

The following practical steps were completed:

- Verified network connectivity between Kali VM and Windows host
- Performed baseline connectivity and port testing
- Enabled Windows Defender Firewall
- Observed default inbound traffic blocking
- Created inbound firewall rules
- Allowed specific ports and blocked unused ports
- Tested allowed and blocked ports from Kali Linux
- Enabled and reviewed firewall logs
- Blocked Kali VM IP to simulate suspicious behavior
- Verified complete traffic blocking
- Analyzed security and operational impact

Each practical step includes **commands, observations, and security reasoning**.

---

## Learning Outcomes

By completing this task, the following skills were developed:

- Practical understanding of Windows Firewall
- Hands-on firewall rule configuration
- Safe use of Kali Linux for defensive testing
- Network access control validation
- Firewall log analysis
- Blue-team and SOC-oriented security mindset

---

## Deliverables

- Deep theoretical documentation (`docs/`)
- Step-by-step practical labs (`labs/`)
- Firewall configuration and testing results
- Interview-ready understanding of firewall concepts

---

## Disclaimer

All testing performed in this repository:

- Was conducted on self-owned systems
- Used isolated virtual machines
- Was done strictly for educational and internship purposes

Testing real-world or unauthorized systems is illegal and unethical.

---

## Conclusion

Firewalls are a critical defensive security control used to reduce
network-based threats.  
This task demonstrates how firewalls are **configured, tested, monitored,
and analyzed** using **Windows Defender Firewall** and **Kali Linux**
in a controlled virtual environment.

Firewalls alone cannot stop all attacks, but when properly configured
and tested, they significantly reduce an organization’s attack surface.
