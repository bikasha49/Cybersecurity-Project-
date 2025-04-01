### <h1>Hyper-V Internal Network Lab – Windows Server Hyper-V Configuration

### <h2>Introduction
This documentation walks through a hands-on lab configuring an Internal Virtual Network in Windows Server Hyper-V. We will create an isolated internal virtual switch, connect a VM and host to it, assign static IPs, adjust network adapter settings, and enable necessary firewall rules via PowerShell. The goal is to establish secure VM-to-host communication over an internal network (no external access). This showcases virtualization and cybersecurity skills like VLAN tagging, secure network practices, and Windows Firewall configuration. Below, 25 sequential screenshots (Screenshot 1 to Screenshot 25) illustrate each step.

Practical Value: This project demonstrates the ability to set up and manage virtual networks, configure VLANs, use PowerShell for firewall settings, and verify connectivity (ping and SMB). It’s a great addition to a GitHub or freelance portfolio for system administration or cybersecurity roles, highlighting hands-on skills in Hyper-V and Windows Server networking.

## Prerequisites and Lab Setup
•	Operating System: Windows Server 2019 (host name: PLABDM01 – a domain member server acting as a Hyper-V host).

•	Hyper-V Role: Installed and enabled on the host (with Hyper-V Manager available).

•	Virtual Machine: A Windows Server 2019 VM (name: PLABDC02) to act as the internal network peer. This VM will be connected to the new internal switch.

•	Privileges: Administrator access on the host and VM to modify Hyper-V settings, network configurations, and firewall rules.

# Tools Used:

o	Hyper-V Manager (for virtual switch and VM settings)

o	Windows Server GUI (Network Connections for IP settings)

o	Windows PowerShell (Admin) (for firewall configuration)

o	Command Prompt/PowerShell in VM (for connectivity testing with ping and net use)

# Configuring the Hyper-V Internal Virtual Switch

1.	Open Hyper-V Manager on the Host Server: On PLABDM01, launch Hyper-V Manager via Server Manager’s Tools menu. This console allows managing VMs and virtual switches on the host. In our lab domain (PRATICELABS.COM), PLABDM01 is the Hyper-V host for the new internal switch.
   1.png
 <p align=:center">
 creating user <br/>
 <img src="https://imgur.com/a/0Eroa0s" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />





---

## Table of Contents

- [About](#about)
- [Projects](#projects)
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
