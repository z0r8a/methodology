# methodology

1. Injection Vulnerabilities
- SQL Injection (SQLi)
- XML Injection
- LDAP Injection
- Command Injection
- NoSQL Injection
- CRLF Injection
- HTML Injection
- XPath Injection
2. Authentication Vulnerabilities
- Broken Authentication
- Session Fixation
- Credential Stuffing
- Password Guessing
- Weak Password Recovery Mechanisms
- Brute Force Attacks
- Exposed Session Tokens
- Predictable Login Endpoints
- Token or Session Expiration Flaws
- Insecure Password Storage (Weak Hashing)
3. Access Control Vulnerabilities
Broken Access Control
Insecure Direct Object References (IDOR)
Privilege Escalation
Mass Assignment Vulnerabilities
Insecure Function-Level Access Control
Path Traversal
Horizontal Privilege Escalation
Vertical Privilege Escalation
Access Control to User-Inputted Data
4. Cross-Site Scripting (XSS)
Reflected XSS
Stored XSS
DOM-Based XSS
Self-XSS
Blind XSS
5. Cross-Site Request Forgery (CSRF)
Classic CSRF
CSRF with SameSite Cookies
Malicious Link/Script Injection for CSRF
Token Mismanagement in CSRF
6. Insecure Deserialization
Object Injection (PHP/Java Deserialization)
Remote Code Execution (RCE) via Insecure Deserialization
Insecure Deserialization Leading to Privilege Escalation
7. Security Misconfiguration
Default Configuration Vulnerabilities
Misconfigured Security Headers (e.g., CORS, X-Frame-Options)
Open Ports and Services
Verbose Error Messages
Lack of Secure Configuration in Web Servers
Default Accounts or Unchanged Credentials
Improper Caching Configuration
8. Sensitive Data Exposure
Insecure Transmission (e.g., HTTP instead of HTTPS)
Weak Encryption Algorithms
Sensitive Data in URLs, Logs, or Cookies
Improper Key Management
Insecure Storage of Sensitive Data (Unhashed Passwords)
Exposed Secrets in Source Code
9. Insufficient Logging & Monitoring
Lack of Proper Logging
Failure to Log Failed Authentication Attempts
Absence of Alerts on Suspicious Activities
Log Tampering
Sensitive Data in Logs
Lack of Audit Trails for Critical Actions
10. Cross-Origin Resource Sharing (CORS) Issues
CORS Misconfiguration
CORS with Open or Misconfigured Origins
CORS with Insecure Cookies
CORS with Malicious Request Forging
11. Security Headers Issues
Missing or Misconfigured HTTP Security Headers
Missing Content Security Policy (CSP)
Lack of Strict Transport Security (HSTS)
Missing X-Content-Type-Options
X-XSS-Protection Misconfigurations
X-Frame-Options Misconfiguration
Referrer-Policy Misconfiguration
12. File Upload Vulnerabilities
Malicious File Upload (Web Shells, Scripts, etc.)
Insecure File Handling (No Antivirus Scanning)
Unrestricted File Type Upload
Insecure File Storage Locations
File Name Injection
13. XML External Entity (XXE) Injection
Classic XXE
Blind XXE
XXE Leading to SSRF
XML Injection
14. Business Logic Vulnerabilities
Race Conditions
Improper Workflow Implementation
Inconsistent Application States
Insecure Workflow Transitions
Sensitive Data Exposure via Business Logic
15. Server-Side Request Forgery (SSRF)
Classic SSRF
SSRF with Internal Network Access
SSRF to Cloud Metadata API
SSRF to Access Private Resources
SSRF Leading to RCE
16. Clickjacking
Frame Injection Attacks
UI Redressing
Clickjacking with Transparent Layers
Manipulation of Web Interfaces with Hidden Frames
17. Improper Input Validation
Untrusted Data Accepted as Input
Improper Input Sanitization
Input Validation Bypasses
Regular Expression Flaws (ReDoS)
Buffer Overflow via Malicious Input
18. Broken Cryptography
Weak or Deprecated Encryption Algorithms
Improper Key Management
Weak Hashing Algorithms
Insecure Data Decryption
Exposed Encryption Keys or Secrets
19. Denial of Service (DoS)
Resource Exhaustion (CPU, Memory)
Distributed Denial of Service (DDoS)
Large Payload DoS
Excessive Resource Consumption
Server Crash Due to Unexpected Input
20. Out-of-Bounds Access
Buffer Overflow (Stack Overflow)
Out-of-Bounds Read/Write
Heap Overflow
21. Application Logic Flaws
Logic Flaws Leading to Privilege Escalation
Unintended Operations
Bypassing Security Policies
Authorization Bypass Using Business Logic
22. Misconfigured APIs
Insecure API Endpoints
No Authentication on APIs
Unencrypted API Endpoints
Overexposed API Data
API Rate Limiting Issues
23. Insufficient Session Management
Session Fixation
Predictable Session IDs
Session Hijacking
Session Timeout Misconfigurations
Cross-Site Script Inclusion via Cookies (CSRF)
Cookies Not Set with Secure or HttpOnly Flags
24. Remote Code Execution (RCE)
Command Injection Vulnerabilities
Remote Code Execution via File Upload
RCE via XML External Entities
RCE via Insecure Deserialization
25. Insufficient Protection Against Bot Attacks
Captcha Bypassing
Automated Attack Prevention Failure
Lack of Rate Limiting
Bot Abuse of Authentication/Forms
26. API Security Issues
Unsecured API Endpoints
Exposed API Keys or Tokens
Lack of API Authentication
Unprotected API Data
Unvalidated API Inputs
27. Third-Party Library Vulnerabilities
Outdated Libraries
Vulnerable Dependencies
Insecure Packages/Plugins
Use of Vulnerable SDKs/APIs
28. Content Injection Vulnerabilities
Cross-Site Script Inclusion (XSSI)
HTML Injection
JSON Injection
JavaScript Injection
29. Insufficient File Permissions
File Permissions in Web Root
Incorrect Access Control for Files
Sensitive Files Exposed to Public
Writable Folders Accessible by Unauthorized Users
30. Path Traversal
Directory Traversal (../)
Path Injection Vulnerabilities
Access to Arbitrary Files Outside of Web Root
