# Web App VAPT Project

## 🔍 Project Overview

This project demonstrates a hands-on Vulnerability Assessment and Penetration Testing (VAPT) lab performed on a simulated web application.

The objective was to identify security vulnerabilities, exploit them, and extract sensitive information using industry-relevant tools and techniques.

---

## 🛠️ Tools Used

* Kali Linux
* Nmap
* FTP
* Gobuster

---

## ⚙️ Lab Setup

* Attacker Machine: Kali Linux
* Target Machine: Vulnerable Web App (10.0.2.8)
* Environment: Virtual Lab

---

## 🚀 Steps Performed

### 1. Network Scanning

Performed Nmap scan to identify open ports and services.

* Found open ports: 21 (FTP), 22 (SSH), 80 (HTTP)

---

### 2. FTP Exploitation (Flag 1)

* Discovered anonymous FTP login
* Accessed FTP server
* Downloaded sensitive file (`flag1.txt`)
* Extracted Flag 1 from the file

---

### 3. Directory Enumeration (Flag 2)

* Used Gobuster to discover hidden directories
* Identified `/robots.txt` endpoint
* Found Flag 2 exposed in robots.txt

---

### 4. Source Code Analysis (Flag 3)

* Inspected web page source using browser
* Found hidden flag inside HTML comments
* Identified information disclosure vulnerability

---

## 🔐 Key Findings

### 🔴 Flag 1 – FTP Misconfiguration

* Anonymous FTP access allowed
* Sensitive file accessible without authentication
  👉 **Risk:** Unauthorized data access

---

### 🔴 Flag 2 – Sensitive Data Exposure (robots.txt)

* Sensitive information exposed in `/robots.txt`
  👉 **Risk:** Attackers can discover hidden endpoints

---

### 🔴 Flag 3 – Information Disclosure

* Flag found in HTML source code comments
  👉 **Risk:** Developers exposing sensitive data in frontend

---

## 📸 Screenshots

### Nmap Scan

![Nmap](screenshots/nmap-scan.png)

### FTP Access & Download

![FTP](screenshots/ftp-download.png)

### Flag Verification

![Flag](screenshots/flag-verification.png)

### Source Code (Hidden Flag)

![Source](screenshots/source-code-flag.png)

### Web Application

![Web App](screenshots/web-application.png)

### Directory Enumeration (Gobuster)

![Gobuster](screenshots/directory-enumeration.png)

---

## 📌 Conclusion

This project demonstrates practical skills in reconnaissance, enumeration, exploitation, and vulnerability analysis in a controlled environment. It highlights common real-world misconfigurations such as insecure FTP access, exposed endpoints, and improper handling of sensitive data.
