# 🛡️ Intrusion Detection Setup with Snort for DVWA

A self-initiated project demonstrating how **Snort IDS** can be used to monitor and detect attacks against the **Damn Vulnerable Web Application (DVWA)** through a combination of **custom detection rules**, **protocol anomaly detection**, and **traffic normalization**.

## 🚀 Project Overview

This project focuses on building a practical intrusion detection lab using Snort and DVWA. The environment was deployed on Ubuntu with Apache, running DVWA and Snort on the same machine using a dual-interface configuration. Detection capabilities were explored through both custom Snort rules and built-in preprocessors such as **Frag3**, **Stream5**, and **HTTP Inspect**.

## 🧪 Attack Scenarios Simulated

Using a Kali Linux attacker machine, the following attacks were simulated and detected:

### Custom Rule Detection

* ✅ Port Scanning (TCP/UDP)
* ✅ SQL Injection (SQLi)
* ✅ Cross-Site Scripting (XSS)
* ✅ Command Injection
* ✅ Path Traversal
* ✅ Reverse Shell Activity
* ✅ Denial of Service (DoS) Attacks
* ✅ Brute Force Login Attempts
* ✅ Malicious File Upload Attempts
* ✅ Automated Scanner Detection 

### Preprocessor-Based Detection

* ✅ Slowloris Attack Detection
* ✅ Fragmentation Evasion Detection
* ✅ TCP FIN Scan Detection
* ✅ Oversized HTTP Header Detection
* ✅ URL-Encoded Payload Detection

## 🛠️ Tools Used

* DVWA: https://github.com/digininja/DVWA
* Snort IDS: https://www.snort.org/
* Kali Linux
* Apache Web Server (Ubuntu)
* Nmap
* Custom Snort Rules

## 📖 Key Concepts Implemented

* Writing and testing Snort rules using `content`, `flow`, `flags`, and `detection_filter`
* Payload-based detection for SQLi, XSS, Command Injection, and Path Traversal
* Rate-based detection for DoS and Brute Force attacks
* Reverse shell detection techniques
* HTTP Header, URI, and Request Body inspection
* Traffic normalization using Frag3, Stream5, and HTTP Inspect
* Protocol anomaly detection and evasion detection
* Dual-interface configuration for traffic separation
* IP whitelisting using `threshold.conf`
* Security monitoring and alert analysis

Preprocessor Rules Reference: [Snort 2.x Preprocessor Rule Definitions](https://github.com/chenkc/snort2.9/blob/master/snort-2.9.11.1/preproc_rules/preprocessor.rules)
