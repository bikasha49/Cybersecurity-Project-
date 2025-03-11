# Hi, I'm Bikasha

Welcome to the Cybersecurity Analyst project! This showcases projects, tools, and resources developed or curated by cybersecurity analysts. It serves as a portfolio and knowledge base to demonstrate expertise and share insights in the field of cybersecurity.

---

## Table of Contents

- [About](#about)
- [Projects](#projects)
- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IT Projects Diagram</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 100%;
            margin: 0 auto;
        }
        .project-diagram {
            display: flex;
            flex-direction: column;
            gap: 30px;
            margin-top: 20px;
        }
        .project {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            padding: 20px;
            position: relative;
        }
        .project-title {
            background-color: #2c3e50;
            color: white;
            padding: 10px 15px;
            border-radius: 5px;
            margin-bottom: 20px;
            font-size: 18px;
            font-weight: bold;
            text-align: center;
        }
        .diagram-area {
            position: relative;
            height: 280px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background-color: #f9f9f9;
            overflow: hidden;
        }
        .component {
            position: absolute;
            padding: 10px;
            border-radius: 5px;
            background-color: #3498db;
            color: white;
            font-size: 14px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0,0,0,0.2);
            transition: all 0.3s ease;
            cursor: pointer;
        }
        .component:hover {
            transform: scale(1.05);
            z-index: 10;
        }
        .connection {
            position: absolute;
            background-color: #7f8c8d;
            z-index: 0;
        }
        .description {
            margin-top: 20px;
            font-size: 16px;
            color: #333;
        }
        .legend {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 10px;
        }
        .legend-item {
            display: flex;
            align-items: center;
            font-size: 14px;
        }
        .legend-color {
            width: 15px;
            height: 15px;
            border-radius: 3px;
            margin-right: 5px;
        }
        .tooltip {
            position: absolute;
            background-color: rgba(0,0,0,0.8);
            color: white;
            padding: 8px 12px;
            border-radius: 4px;
            font-size: 14px;
            z-index: 100;
            max-width: 200px;
            display: none;
        }
        #networkServer { background-color: #3498db; }
        #adServer { background-color: #9b59b6; }
        #dnsServer { background-color: #2ecc71; }
        #dhcpServer { background-color: #e74c3c; }
        #client { background-color: #f39c12; }
        #repairStation { background-color: #3498db; }
        #securityTraining { background-color: #9b59b6; }
        #userSupport { background-color: #2ecc71; }
        #community { background-color: #e74c3c; }
        
        @media (max-width: 768px) {
            .diagram-area {
                height: 400px;
            }
            .component {
                font-size: 12px;
                padding: 8px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>IT Projects Visualization</h1>
        
        <div class="project-diagram">
            <!-- Enterprise Network Lab Project -->
            <div class="project">
                <div class="project-title">Enterprise Network Lab</div>
                <div class="diagram-area" id="network-diagram">
                    <!-- Network Components -->
                    <div class="component" id="networkServer" style="top: 20px; left: 50%; transform: translateX(-50%); width: 140px;">
                        Virtual Environment
                    </div>
                    
                    <div class="component" id="adServer" style="top: 100px; left: 20%; width: 120px;">
                        Active Directory
                    </div>
                    
                    <div class="component" id="dnsServer" style="top: 100px; left: 50%; transform: translateX(-50%); width: 120px;">
                        DNS Server
                    </div>
                    
                    <div class="component" id="dhcpServer" style="top: 100px; left: 80%; width: 120px; transform: translateX(-100%);">
                        DHCP Server
                    </div>
                    
                    <div class="component" id="client" style="top: 200px; left: 50%; transform: translateX(-50%); width: 160px;">
                        Simulated Corporate Environment
                    </div>
                    
                    <!-- Connections as divs -->
                    <div class="connection" style="top: 65px; left: 50%; width: 2px; height: 35px; transform: translateX(-50%);"></div>
                    
                    <div class="connection" style="top: 65px; left: 26%; width: 2px; height: 35px;"></div>
                    <div class="connection" style="top: 65px; left: 50%; width: 2px; height: 35px; transform: translateX(-50%);"></div>
                    <div class="connection" style="top: 65px; left: 74%; width: 2px; height: 35px;"></div>
                    
                    <div class="connection" style="top: 145px; left: 26%; width: 2px; height: 55px;"></div>
                    <div class="connection" style="top: 145px; left: 50%; width: 2px; height: 55px; transform: translateX(-50%);"></div>
                    <div class="connection" style="top: 145px; left: 74%; width: 2px; height: 55px;"></div>
                    
                    <div class="connection" style="top: 145px; left: 26%; width: 48%; height: 2px;"></div>
                </div>
                
                <div class="description">
                    <p>This virtual lab environment simulates a corporate IT infrastructure with core network services:</p>
                    <div class="legend">
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #3498db;"></div>
                            <span>Virtual Environment: Hypervisor platform hosting all services</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #9b59b6;"></div>
                            <span>Active Directory: User accounts, group policies, and authentication</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #2ecc71;"></div>
                            <span>DNS Server: Domain name resolution and service records</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #e74c3c;"></div>
                            <span>DHCP Server: IP address assignment and network configuration</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #f39c12;"></div>
                            <span>Simulated Corporate Network: Clients, servers, and network devices</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Community Tech Support Initiative -->
            <div class="project">
                <div class="project-title">Community Tech Support Initiative</div>
                <div class="diagram-area" id="support-diagram">
                    <!-- Support Components -->
                    <div class="component" id="repairStation" style="top: 30px; left: 30%; width: 120px;">
                        PC/Printer Repair
                        <br>20+ Devices
                    </div>
                    
                    <div class="component" id="securityTraining" style="top: 30px; left: 70%; width: 120px; transform: translateX(-100%);">
                        Security Training
                    </div>
                    
                    <div class="component" id="userSupport" style="top: 120px; left: 50%; transform: translateX(-50%); width: 160px;">
                        Technical Support Services
                    </div>
                    
                    <div class="component" id="community" style="top: 210px; left: 50%; transform: translateX(-50%); width: 160px;">
                        Community Members
                    </div>
                    
                    <!-- Connections -->
                    <div class="connection" style="top: 75px; left: 35%; width: 2px; height: 45px;"></div>
                    <div class="connection" style="top: 75px; left: 65%; width: 2px; height: 45px;"></div>
                    
                    <div class="connection" style="top: 75px; left: 35%; width: 30%; height: 2px;"></div>
                    
                    <div class="connection" style="top: 165px; left: 50%; width: 2px; height: 45px; transform: translateX(-50%);"></div>
                </div>
                
                <div class="description">
                    <p>This community initiative provided technical support and education to local residents:</p>
                    <div class="legend">
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #3498db;"></div>
                            <span>PC/Printer Repair: Troubleshooting and fixing 20+ devices</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #9b59b6;"></div>
                            <span>Security Training: Teaching best practices for online safety</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #2ecc71;"></div>
                            <span>Technical Support: Central coordination of all services</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background-color: #e74c3c;"></div>
                            <span>Community Members: Recipients of technical assistance</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="tooltip" id="tooltip"></div>

    <script>
        // Add interactivity to components
        const components = document.querySelectorAll('.component');
        const tooltip = document.getElementById('tooltip');
        
        const tooltipContent = {
            'networkServer': 'Virtual environment using technologies like VMware or VirtualBox to create isolated network sandbox.',
            'adServer': 'Active Directory services for centralized authentication, user management, and group policies.',
            'dnsServer': 'Domain Name System for hostname resolution and service discovery.',
            'dhcpServer': 'Dynamic Host Configuration Protocol for automatic IP address assignment and network configuration.',
            'client': 'Simulated workstations and servers representing an enterprise network topology.',
            'repairStation': 'Workbench with diagnostic tools for hardware and software repair of community devices.',
            'securityTraining': 'Educational sessions on password management, phishing awareness, and safe browsing habits.',
            'userSupport': 'Central hub for coordinating technical assistance and educational resources.',
            'community': 'Local residents and organizations benefiting from free technical support and training.'
        };
        
        components.forEach(component => {
            component.addEventListener('mouseover', function(e) {
                const id = this.id;
                if (tooltipContent[id]) {
                    tooltip.textContent = tooltipContent[id];
                    tooltip.style.display = 'block';
                    tooltip.style.left = e.pageX + 10 + 'px';
                    tooltip.style.top = e.pageY + 10 + 'px';
                }
            });
            
            component.addEventListener('mouseout', function() {
                tooltip.style.display = 'none';
            });
            
            component.addEventListener('mousemove', function(e) {
                tooltip.style.left = e.pageX + 10 + 'px';
                tooltip.style.top = e.pageY + 10 + 'px';
            });
            
            component.addEventListener('click', function() {
                this.style.backgroundColor = this.style.backgroundColor === 'yellow' ? 
                    document.getElementById(this.id).style.backgroundColor : 'yellow';
            });
        });
    </script>
</body>
</html>
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
