# AenexzInternship

# SecureCorp Security Assessment

## Project Overview

This project presents a controlled security assessment of the SecureCorp customer portal environment.

The assessment was conducted in an isolated laboratory environment to identify security weaknesses, perform controlled attack simulations, investigate security events, and evaluate centralized monitoring using Wazuh.

## Assessment Environment

The assessment environment consisted of:

- Ubuntu Server — target server and DVWA host
- DVWA (Damn Vulnerable Web Application) — vulnerable web application used for security testing
- WSL — attacker and security analyst environment
- Wazuh — centralized security monitoring and event analysis
- Nmap — network and service discovery
- Hydra — controlled brute-force testing
- Wireshark — packet capture and traffic analysis

## Security Assessment Activities

The assessment followed a structured process:

1. Environment and network discovery
2. Asset and service identification
3. Vulnerability and security testing
4. Controlled attack simulation
5. Wazuh-based monitoring and log collection
6. Detection and investigation of security events
7. Risk analysis and security recommendations

## Attack Simulations

The following controlled attacks were performed against the DVWA laboratory environment:

### 1. Brute Force
Repeated authentication attempts were performed to evaluate authentication security and monitoring visibility.

### 2. SQL Injection
SQL Injection testing was performed to determine whether crafted input could manipulate database queries and disclose additional records.

### 3. Reflected XSS
Reflected Cross-Site Scripting testing was performed to determine whether injected JavaScript could be reflected and executed in the browser.

### 4. Command Injection
Command Injection testing was performed to determine whether application input could result in operating-system command execution.

## Security Monitoring

Wazuh was used as the centralized security monitoring platform.

The assessment included monitoring of:

- Linux authentication events
- Web application activity
- Security alerts
- Attack-related events
- Authentication failures
- Wazuh detection rules and event details

Some activities were automatically visible through Wazuh, while certain application-level attacks required additional manual investigation of available web-server/application logs.

## Key Findings

The assessment identified the following major security risks:

- Weak authentication controls can increase the risk of unauthorized access.
- SQL Injection can result in unauthorized database information disclosure or manipulation.
- Reflected XSS can allow malicious JavaScript to execute in a user's browser.
- Command Injection can potentially allow unauthorized operating-system command execution.
- Default monitoring coverage may not automatically identify every application-level attack.

## Recommendations

The main security recommendations include:

- Enforce strong password policies.
- Implement multi-factor authentication.
- Use parameterized SQL queries and prepared statements.
- Apply strict input validation and output encoding.
- Avoid direct operating-system command execution.
- Restrict unnecessary network services.
- Maintain regular patch management.
- Improve Wazuh detection coverage and centralized logging.
- Maintain tested backups.
- Conduct regular security awareness training.

## Project Deliverables

This repository contains supporting materials for the security assessment, including:

- Security Assessment Report
- Network discovery evidence
- Attack simulation evidence
- Wazuh monitoring evidence
- Supporting logs and screenshots

## Disclaimer

This project was conducted only in an authorized and controlled laboratory environment for educational and security assessment purposes.

No public websites, public IP addresses, shared network devices, or systems belonging to other users were targeted.

## Author

**Koshik T**

Security Assessment Project  
16 August 2026
