# Hi, I'm Bikasha

Welcome to the Cybersecurity Analyst project! This showcases projects, tools, and resources developed or curated by cybersecurity analysts. It serves as a portfolio and knowledge base to demonstrate expertise and share insights in the field of cybersecurity.

---

## Table of Contents

- [About](#about)
- [Projects](#projects)
- Enterprise Network Lab Setup
This lab simulates a corporate IT infrastructure with Active Directory (AD), Domain Name System (DNS), and Dynamic Host Configuration Protocol (DHCP) in a virtualized environment.

Lab Requirements:
Virtualization Software: VMware Workstation, VirtualBox, or Hyper-V
Operating System: Windows Server (2016, 2019, or 2022)
Client OS: Windows 10/11 for testing
Network: Internal or Host-Only network
Step 1: Set Up a Windows Server VM
Install Windows Server on a virtual machine.
Assign a static IP address (e.g., 192.168.1.10).
Rename the server (e.g., DC01).
Step 2: Configure Active Directory (AD DS)
Open Server Manager → Add Roles and Features.
Install Active Directory Domain Services (AD DS).
Promote the server to a Domain Controller (DC).
Create a domain (e.g., corp.local).
Reboot and verify domain setup.
Step 3: Set Up DNS
In Server Manager, go to DNS Manager.
Configure Forward Lookup Zones for the domain (corp.local).
Verify DNS resolution using nslookup.
Step 4: Configure DHCP
Install the DHCP Server role via Server Manager.
Configure a DHCP scope:
Scope Name: Corporate LAN
IP Range: 192.168.1.100 - 192.168.1.200
Subnet Mask: 255.255.255.0
Gateway: 192.168.1.1
DNS: 192.168.1.10 (AD DS Server)
Authorize and activate the DHCP scope.
Step 5: Join a Client Machine to the Domain
Set up a Windows 10/11 VM.
Assign an IP via DHCP.
Join the domain (corp.local).
Verify domain login using Active Directory users.
Community Tech Support Initiative Setup
This project involves repairing PCs/printers and training users on security best practices.

Step 1: Hardware & Software Repair
PC Repair Tasks:

Run hardware diagnostics.
Check disk health (chkdsk /f).
Optimize performance by clearing temporary files (cleanmgr).
Printer Repair Tasks:

Update printer drivers.
Clear print spooler (net stop spooler & net start spooler).
Step 2: Security Training Topics
Strong Passwords: Enforce password complexity.
Phishing Awareness: Identify suspicious emails.
System Updates: Enable auto-updates for OS and antivirus.
Data Backup: Use OneDrive or external drives for backups.
- [Threat Detection](#threat-detection)
- [Incident Response](#incident-response)
 -[Vulnerability Assessment](#vulnerability-assessment)
- [Tools and Scripts](#tools-and-scripts)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

---

## About

Motivated Cybersecurity Graduate | Entry-Level Cybersecurity Analyst | Skilled in Network Security, Threat Detection, & Incident Response | Passionate About Safeguarding Data Integrity & Combating Evolving Threats.

- Threat detection and analysis
- Incident response and mitigation
- Network security and monitoring
- Vulnerability assessments
- Security automation and scripting

It is intended to highlight both practical skills and a strong understanding of cybersecurity concepts.

---

## Skills

### Threat Detection
- **Malware Analysis Toolkit**: A Python-based tool for analyzing malware samples and identifying potential threats. 
  [View Project](./projects/malware-analysis)
- **SIEM Rule Set**: A custom rule set designed for Splunk to identify anomalous behaviors in network traffic.
  [View Project](./projects/siem-rules)

### Incident Response
- **Phishing Email Analysis**: A framework for analyzing and responding to phishing email attacks.
  [View Project](./projects/phishing-response)
- **Forensics Investigation Report**: A detailed investigation of a compromised system using forensic tools.
  [View Project](./projects/forensic-report)

### Vulnerability Assessment
- **Web Application Security Assessment**: A comprehensive report on the vulnerabilities found in a sample web application.
  [View Project](./projects/web-security-assessment)
- **Network Vulnerability Scan**: A scanning project using tools like Nessus and OpenVAS.
  [View Project](./projects/network-scan)

---

## Tools and Scripts

- **Automated Log Parser**: A Python script to parse and analyze log files for suspicious activities.
  [View Script](./tools/log-parser)
- **Firewall Configuration Checker**: A Bash script for validating firewall rules against security policies.
  [View Script](./tools/firewall-checker)

---

## Resources

- **Learning Materials**: Links to recommended books, courses, and articles on cybersecurity.
  [View Resources](./resources/learning-materials.md)
- **Cybersecurity Standards**: Documentation and guidelines on industry standards such as NIST, ISO 27001, and CIS.
  [View Resources](./resources/standards.md)

---

## Contributing

Contributions are welcome! If you have suggestions, bug reports, or would like to add your own projects to this repository, please submit a pull request or open an issue.

---

## License

This repository is licensed under the [MIT License](./LICENSE). Feel free to use and modify the content as needed.
