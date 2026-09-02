# Task 3 - Basic Vulnerability Scan

Target: My Device - Android 10 (End of Life) + Google Chrome < 151
Finding: Device is running outdated OS with no security patches since 2023, 
making it vulnerable to multiple High/Critical CVEs including CVE-2026-82072.
Recommendation: Upgrade device to Android 13+ or use with updated browser and minimal sensitive data.


**Name:** Sukanya
**Tool Used:** CVE Details + CIRCL Lookup (Mobile-based Vulnerability Scanning - Alternative to Nessus/OpenVAS)
**Target:** Google Chrome (Version < 151.0.7922.72) - My Device
**Date:** 01-09-2026

### 1. Scan Summary
Used CVE Details database to perform vulnerability lookup on my system software (Google Chrome). This database is the same source used by Nessus/OpenVAS scanners.

Total Vulnerabilities Found for Chrome: 200+ 
Filtered by CVSS Min 7 (High/Critical): 4 Critical Vulnerabilities found in recent scan.

### 2. Vulnerabilities Found (Proof Attached)

**Vuln 1: CVE-2026-82072 - HIGH - CVSS 8.8**
- Description: Out of bounds read in V8 in Google Chrome prior to 151.0.7922.72 allowed remote attacker to execute arbitrary code via crafted HTML page.
- CWE: CWE-125 Out-of-bounds Read
- Impact: Code Execution inside sandbox
- Fix: Update Chrome to version 151.0.7922.72 or later

**Vuln 2: CVE-2026-79292 - HIGH - CVSS 8.3**
- Description: Integer overflow in Chromecast in Chrome prior to 152.0.7977.65 allowed attacker to execute arbitrary code outside sandbox.
- Fix: Update Chrome

**Vuln 3: CVE-2026-79293 - MEDIUM - CVSS 6.5**
- Description: Information leak in Animation in Chrome allowed remote attacker to obtain sensitive information via crafted HTML page.

### 3. Screenshots
- Screenshot 1: Vulnerability list from cvedetails.com
- Screenshot 2: Detailed CVE-2026-82072 with CVSS Vector and EPSS score

### 4. Mitigation Steps I Took
1. Updated Google Chrome to latest version (Settings > About Chrome)
2. Enabled Enhanced Protection in Chrome Safety
3. Cleared cache and restarted browser

### 5. Conclusion
Learned how vulnerability scanners use CVE database, what is CVSS scoring (0-10), EPSS scoring, and how to fix outdated software vulnerabilities.

