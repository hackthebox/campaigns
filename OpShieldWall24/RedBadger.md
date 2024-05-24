# Threat Intelligence Report - RedBadger

### Produced by: Global Alliance for Security Cooperation (GASC)
### Report Date: 2024-05-24

---

## Executive Summary

RedBadger is a cyber threat group known for its sophisticated and multi-faceted attack techniques. This report highlights the key techniques employed by RedBadger, specifically focusing on their use of off-the-shelf tooling, ransomware deployment, user account creation, living off the land, and the use of remote monitoring and management (RMM) tooling.

---

## Techniques and Tactics

### 1. Use of Off-the-Shelf Tooling

**Description:**  
RedBadger leverages commercially available tools to facilitate their operations. These tools, designed for legitimate purposes, are repurposed for malicious activities, allowing RedBadger to blend in with normal network traffic and avoid detection.

**Technique ID:** T1072

**Details:**
- RedBadger uses software such as Cobalt Strike, Metasploit, and Mimikatz.
- These tools provide capabilities for network reconnaissance, exploitation, and credential harvesting.
- The utilization of these tools complicates attribution and detection efforts.

### 2. Ransomware Deployment

**Description:**  
RedBadger employs ransomware to encrypt critical data and systems within target networks, demanding ransom payments for decryption keys.

**Technique ID:** T1486

**Details:**
- The group uses various ransomware strains, often customizing them to evade antivirus detection.
- Deployment typically follows initial compromise and lateral movement within the network.
- They demand payment in cryptocurrencies to further obscure their identity.

### 3. User Account Creation

**Description:**  
RedBadger creates new user accounts on compromised systems to maintain persistence and facilitate ongoing access.

**Technique ID:** T1136

**Details:**
- Accounts are often created with administrative privileges.
- These accounts are used to perform further malicious activities, including data exfiltration and system manipulation.
- Account creation is often hidden by using names similar to legitimate accounts.

### 4. Living Off the Land

**Description:**  
RedBadger uses built-in system tools and scripts to perform malicious activities, reducing the need for downloading additional malware and thus lowering the chance of detection.

**Technique ID:** T1562

**Details:**
- Tools like PowerShell, Windows Management Instrumentation (WMI), and Task Scheduler are commonly used.
- These techniques enable RedBadger to execute commands, move laterally, and gather information without raising alarms.
- Living off the land minimizes the forensic footprint of their activities.

### 5. Use of RMM Tooling

**Description:**  
RedBadger uses remote monitoring and management (RMM) tools, which are typically used by IT administrators for legitimate purposes, to control compromised systems remotely.

**Technique ID:** T1021.001

**Details:**
- Tools such as TeamViewer, AnyDesk, and LogMeIn are repurposed for malicious control.
- These tools provide remote access to victim machines, allowing for data exfiltration and further system compromise.
- Using legitimate RMM tools helps RedBadger avoid detection by security solutions that trust these applications.

---

## Conclusion

RedBadger demonstrates a high level of sophistication and adaptability in their attack techniques. By leveraging off-the-shelf and built-in tools, creating new user accounts, and deploying ransomware, they effectively balance efficiency and stealth. The use of RMM tools further aids in maintaining control over compromised environments, highlighting the need for vigilant monitoring and robust security measures to counter such threats.

---

## Recommendations

- Implement robust monitoring for the use of off-the-shelf and built-in tools within your network.
- Ensure up-to-date backups and incident response plans to mitigate ransomware impacts.
- Regularly audit user accounts and privileges to detect unauthorized account creation.
- Employ advanced endpoint detection and response (EDR) solutions to identify and stop living off the land techniques.
- Monitor and restrict the use of RMM tools to prevent unauthorized remote access.

---

_For any inquiries or further details, please contact the GASC Threat Intelligence Team._

**Document Classification:** Confidential  
**Document Version:** 1.0
