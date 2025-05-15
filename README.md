# NESSUS-VUL-SCANNING-from_Zero_to_Hero
# scan vulnerability in you environment as a Pro



# Nessus Vulnerability Scanning - From Zero to Pro

Welcome to the ultimate guide on mastering **Nessus**, one of the most powerful vulnerability scanners available. This GitHub page will walk you through installation, configuration, different scan types, their advantages, use cases, and provide a step-by-step guide to become a pro in vulnerability assessment using Nessus.

---

## Table of Contents

- [What is Nessus?](#what-is-nessus)
- [Why Use Nessus?](#why-use-nessus)
- [Types of Nessus Scans](#types-of-nessus-scans)
- [Installation Guide](#installation-guide)
- [Initial Setup & Configuration](#initial-setup--configuration)
- [Creating and Running a Scan](#creating-and-running-a-scan)
- [Analyzing Results](#analyzing-results)
- [Advanced Tips & Pro Techniques](#advanced-tips--pro-techniques)
- [Best Practices](#best-practices)
- [Resources](#resources)

---

## What is Nessus?

[Nessus](https://www.tenable.com/products/nessus) is a widely-used vulnerability scanner developed by Tenable. It helps identify security issues like missing patches, configuration weaknesses, and known vulnerabilities across systems, networks, and applications.

---

## Why Use Nessus?

-l-setup--configuration)
- [Creat- Over 70,000 plugins covering various vulnerabilities
- Compliance auditing (CIS, PCI-DSS, HIPAA, etc.)
- Easy to use UI and rich reporting options
- Integration with other Tenable products and SIEM tools

---

## Types of Nessus Scans

### 1. Basic Network Scan
- Purpose: Identify common vulnerabilities on IPs or ranges
- Advantages: Fast and easy
- Use Case: Regular security checks on servers

### 2. Advanced Scan
- Purpose: Custom, detailed scan with full control
- Advantages: Highly configurable
- Use Case: Penetration testing, compliance scanning

### 3. Web Application Scan
- Purpose: Test web apps for XSS, SQLi, etc.
- Advantages: Detect OWASP Top 10 vulnerabilities
- Use Case: Secure web-based platforms

### 4. Credentialed Scan
- Purpose: Authenticated scanning with system credentials
- Advantages: Deeper insight, less false positives
- Use Case: Internal audits, patch verification

### 5. Compliance Scan
- Purpose: Check adherence to standards like PCI, HIPAA
- Advantages: Readymade templates
- Use Case: Regulatory and legal compliance

---

## Installation Guide

### On Kali Linux / Ubuntu:
```bash
wget https://www.tenable.com/downloads/api/v1/public/pages/nessus/downloads/NESSUS_VERSION.deb
sudo dpkg -i NESSUS_VERSION.deb
sudo systemctl start nessusd

On Windows / macOS:
 • Download the installer from: https://www.tenable.com/downloads/nessus
 • Follow the setup wizard

Then access Nessus at:

https://localhost:8834


⸻

Initial Setup & Configuration
 1. Access the web interface (https://localhost:8834)
 2. Create an account
 3. Choose Nessus Essentials (Free) or link your Tenable license
 4. Enter activation code
 5. Download plugins (automatic process)
 6. Log in and start scanning

⸻

Creating and Running a Scan

Step-by-Step:
 1. Login to Nessus Web Interface
 2. Go to Scans > New Scan
 3. Select a scan template (e.g., Basic Network Scan)
 4. Enter:
 • Name
 • Targets (IPs, subnets)
 • Schedule (optional)
 5. Configure credentials if needed (Windows, SSH, etc.)
 6. Click Save and Launch

⸻

Analyzing Results

After a scan:
 1. Go to My Scans
 2. Click on your completed scan
 3. Review:
 • Vulnerabilities tab for severity levels
 • Affected hosts
 • Plugins triggered
 4. Export results as:
 • PDF
 • CSV
 • HTML

⸻

Advanced Tips & Pro Techniques

1. Use Credentialed Scanning
 • Reduces false positives
 • Detects patch levels and local misconfigurations

2. Filter with Tags and Policies
 • Tag assets by department, location
 • Reuse scanning policies for consistency

3. Automate with Schedules
 • Run weekly or monthly scans automatically

4. Integrate with SIEM
• Export results to Splunk, QRadar, etc. for deeper analysis

5. Build Custom Scan Templates
 • Fine-tune plugins and settings
 • Disable noisy checks or irrelevant ones

⸻

Best Practices
 • Always update plugins
 • Use credentialed scans
 • Scan both internal and external assets
 • Perform regular scans (weekly/monthly)
 • Review and remediate critical/high vulnerabilities immediately
 • Document exceptions and compensating controls

⸻

Resources
 • Nessus Documentation (https://docs.tenable.com/nessus/)
 • Plugin Library (https://www.tenable.com/plugins)
 • OWASP Top 10 (https://owasp.org/www-project-top-ten/)
 • Security Standards (https://www.cisecurity.org/cis-benchmarks/)

⸻

Author

Groua7
Certified in AWS Solution Architect-Associate,  CCNA, Security+, CySA+, CSAP and  Splunk Core
Passionate about Network Security and Vulnerability Management

“Scan smart, fix fast, stay secure.”

