# Firewall Configuration & Testing (Practical – VM Based)

## Overview

The task focuses on understanding **firewall concepts**, **rule configuration**,
and **practical testing using virtual machines**.

The practical implementation is carried out using:
- **Kali Linux** as a testing machine
- **Linux (Ubuntu)** as a firewall-protected system

All activities are **defensive, legal, and performed in a controlled lab environment**.

---

## Objectives

The objectives of this task are:

- Understand firewall fundamentals and working principles
- Learn stateful and stateless firewall behavior
- Configure firewall rules using UFW
- Allow and deny specific ports
- Test connectivity from Kali Linux
- Observe firewall logs
- Block a malicious IP address
- Analyze the impact of firewall rules

---

## Lab Architecture

### Virtual Machines Used

| VM | Role |
|----|----|
| Kali Linux | Connectivity tester / security testing machine |
| Ubuntu Linux | Firewall-configured target system |

### Network Configuration

- Host-Only Adapter or Internal Network
- No internet-facing exposure
- Example IPs:
  - Kali Linux: `192.168.56.101`
  - Ubuntu Linux: `192.168.56.102`

This setup ensures **safe, legal, and isolated testing**.

---

## Tools Used

- **UFW (Uncomplicated Firewall)** – Linux host-based firewall
- **iptables** (conceptual understanding)
- **Kali Linux utilities**:
  - ping
  - ssh
  - nmap
  - netcat (nc)
- **Ubuntu Linux** as firewall target

---

## Key Firewall Concepts Covered

### Firewall Fundamentals
- Network traffic filtering
- Default deny principle
- Least privilege networking

### Stateful vs Stateless Firewalls
- Packet inspection
- Connection tracking
- Session awareness

### Inbound and Outbound Rules
- Incoming traffic control
- Outgoing traffic restrictions
- Malware communication prevention

### Firewall Logging
- Visibility into blocked and allowed traffic
- Incident detection
- Audit and troubleshooting support

### IP Blocking
- Temporary containment strategy
- Response to suspicious activity
- Limitations of IP-based filtering

---

## Practical Activities Performed

- Verified baseline connectivity before firewall rules
- Enabled UFW with default deny inbound policy
- Allowed SSH access securely
- Allowed and denied specific ports
- Tested connectivity from Kali Linux
- Enabled and analyzed firewall logs
- Blocked Kali IP to simulate malicious behavior
- Restored access by removing rules
- Analyzed firewall impact and limitations

Each step includes **commands, observations, and security reasoning**.

---

## Learning Outcomes

By completing this task, the following skills were developed:

- Practical firewall configuration
- Understanding of network access control
- Safe use of Kali Linux for defensive testing
- Firewall log analysis
- Risk and impact assessment
- Real-world SOC and system administration mindset

---

## Deliverables

- Firewall rules documentation
- Practical VM-based testing results
- Impact and security analysis
- Interview-ready understanding of firewall operations

---

## Disclaimer

All testing in this repository was performed:

- On self-owned virtual machines
- In an isolated lab environment
- For educational and internship purposes only

Unauthorized testing of real-world systems is illegal and unethical.

---

## Conclusion

Firewalls are a critical security control for reducing network-based attacks.
This task demonstrates how firewalls are **configured, tested, monitored,
and analyzed in real environments** using Kali Linux and Linux firewalls.

Firewalls do not stop all attacks, but when correctly configured and tested,
they significantly reduce an organization’s attack surface.
