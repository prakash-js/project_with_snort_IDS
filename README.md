# 🛡️ Securing DVWA using Snort IDS

A self-initiated project that demonstrates how **Snort IDS** can be used to monitor and detect attacks against the **Damn Vulnerable Web Application (DVWA)** using custom detection rules.

## 🚀 Project Overview

This project focuses on writing and tuning Snort rules to detect real-world attack patterns in a controlled lab setup. The environment was deployed on Ubuntu with Apache, running DVWA and Snort on the same machine configured with dual interfaces.

## 🧪 Attack Scenarios Simulated
Using a Kali Linux attacker machine, the following attacks were simulated and detected by custom Snort rules:
- ✅ Port Scanning (TCP/UDP)
- ✅ SQL Injection
- ✅ Cross-Site Scripting (XSS)
- ✅ Command Injection
- ✅ Path Traversal
- ✅ Reverse Shell Attempts
- ✅ Denial of Service (DoS) Attacks
- ✅ Brute Force Login Attempts

## 🛠️ Tools Used
- DVWA: [https://github.com/digininja/DVWA](https://github.com/digininja/DVWA)
- Snort IDS: [https://www.snort.org/](https://www.snort.org/)
- Kali Linux for attack simulation
- Apache Web Server (Ubuntu)
- Custom Snort Rules

## 📖 Key Concepts Implemented
- Writing and testing Snort rules using `content`, `flow`, `flags`, and `detection_filter`.
- Rate-based detection for DoS and Brute Force.
- Payload-based detection for SQLi, XSS, Command Injection.
- Reverse shell detection using TCP flags and content match.
- Dual-interface configuration for improved traffic separation.
- IP whitelisting using `threshold.conf`.



