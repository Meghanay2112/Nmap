# 🔐 Task 1: Local Network Port Scanning using Nmap

## 📌 Cyber Security Internship – Task 1

---

## 🎯 Objective
The objective of this task is to identify active devices and discover open ports within my local network using Nmap. This helps in understanding network exposure and basic reconnaissance techniques used in cybersecurity.

---

## 🛠 Tools Used
- Nmap (Network Scanning Tool)
- Npcap (Packet Capture Driver)
- Windows Command Prompt

---

## 🌐 Network Details
- IPv4 Address: 10.126.199.184
- Network Range Scanned: 10.126.199.0/24
- Scan Type: TCP SYN Scan (-sS)

---

## 🔍 Methodology

1. Installed Nmap and Npcap.
2. Identified the local IPv4 address using:
   ipconfig
3. Determined the network range as:
   10.126.199.0/24
4. Performed TCP SYN scan using:
   nmap -sS 10.126.199.0/24
5. Saved the scan results using:
   nmap -sS 10.126.199.0/24 -oN scan_results.txt

---

## 📊 Scan Results

- Total IP addresses scanned: 256
- Active hosts detected: 2
- Open ports identified on host 10.126.199.184:

| Port | Service       | Description |
|------|--------------|-------------|
| 80   | HTTP         | Web service |
| 135  | MSRPC        | Microsoft Remote Procedure Call |
| 139  | NetBIOS-SSN  | Windows File Sharing |
| 445  | Microsoft-DS | SMB File Sharing |

---

## ⚠️ Security Analysis

- Port 80 (HTTP) may expose web services without encryption.
- Port 445 (SMB) can be vulnerable to ransomware and SMB-based attacks if not properly secured.
- Ports 135 and 139 are related to Windows networking services and may allow unauthorized access if misconfigured.

Open ports increase network exposure and should be secured using firewalls, strong authentication, and proper service configuration.

---

## 🧠 Key Concepts Learned

- Port Scanning
- TCP SYN Scan
- Network Reconnaissance
- Open Port Identification
- Basic Security Risk Analysis

---

## ✅ Conclusion

This task helped me understand how to perform network reconnaissance using Nmap, identify open ports, and analyze potential security risks associated with exposed services. It strengthened my foundational knowledge of network security and port scanning techniques.

---

## 📁 Files Included
- scan_results.txt


