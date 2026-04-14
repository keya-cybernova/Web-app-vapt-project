# Web Application VAPT – Vulnerability Assessment & Penetration Testing

## Objective

Performed vulnerability assessment and penetration testing on a simulated vulnerable web application to identify security weaknesses and demonstrate real-world attack scenarios.

---

## Tools Used

* Kali Linux
* Nmap
* Burp Suite
* VirtualBox

---

## Lab Setup

* Attacker: Kali Linux
* Target: Simulated vulnerable web application
* Network: Isolated lab setup

---

## What I Did

### Reconnaissance & Scanning

* Performed aggressive scanning using Nmap (`nmap -A`)
* Identified open ports and running services

### Exploitation

* Discovered FTP service allowing anonymous login
* Extracted sensitive files using FTP and wget

### Web Application Testing

* Analyzed website content and source code
* Identified sensitive data exposed in HTML
* Accessed hidden endpoints like `/robots.txt` and `/admin`

### Traffic Interception

* Used Burp Suite to intercept HTTP requests
* Extracted hidden data from intercepted traffic

---

## Key Findings

* FTP misconfiguration allowing anonymous access
* Sensitive data exposed in website source code
* Weak access control on admin panel
* Exposure of sensitive endpoints

---

## Impact

These vulnerabilities could allow attackers to:

* Gain unauthorized access to sensitive data
* Discover hidden application components
* Exploit weak authentication mechanisms

---

## Recommendations

* Disable anonymous FTP access
* Avoid exposing sensitive data in source code
* Implement strong authentication and access control
* Secure sensitive endpoints and directories

---

## Screenshots

(Add your screenshots below)
