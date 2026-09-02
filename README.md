# Task 3 - Basic Vulnerability Scan

**Name:** Sukanya  
**Tool Used:** CVE Details + CIRCL CVE Lookup (Alternative to Nessus/OpenVAS for Mobile)  
**Target:** My Device - Google Chrome (< 151.0.7922.72) on Android 10  
**Date:** 01-09-2026

### 1. Objective
To perform a basic vulnerability scan on my own device and understand CVE, CVSS, and EPSS scoring without using paid tools like Nessus.

### 2. Scan Summary
Used CVE Details (cvedetails.com), the same database used by Nessus/OpenVAS.

- Total Vulnerabilities Found for Chrome: 200+
- Filtered (CVSS >= 7.0): 4 High/Critical vulnerabilities found

### 3. Key Vulnerability Found

**CVE-2026-82072 - HIGH - CVSS 8.8**
- **Description:** Out of bounds read in V8 in Google Chrome prior to 151.0.7922.72 allowed a remote attacker to execute arbitrary code via a crafted HTML page.
- **CWE:** CWE-125 (Out-of-bounds Read)
- **Impact:** Remote Code Execution inside sandbox
- **Fix:** Update to Chrome version 151.0.7922.72 or later

Other Findings:
- CVE-2026-79292 (CVSS 8.3) - Integer Overflow in Chromecast
- CVE-2026-79293 (CVSS 6.5) - Information Leak in Animation

### 4. Proof of Scan
- Screenshot 1: Vulnerability list from cvedetails.com
- Screenshot 2: Detailed CVE-2026-82072 with CVSS Vector and EPSS score

*(Upload your screenshots in this folder)*

### 5. Mitigation Steps Taken
1. Updated Google Chrome to latest version (Settings > About Chrome > Update)
2. Enabled Enhanced Protection in Chrome > Safety Check
3. Cleared cache and restarted browser

### 6. Conclusion
Understood how vulnerability scanners work using the CVE database. Learned about CVSS scoring (0-10 severity), EPSS scoring (exploit probability), and importance of regular software updates to prevent exploitation.
