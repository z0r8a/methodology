# methodology

### 1. Injection Vulnerabilities
- [SQL Injection](/resources/SQL_Injection.md)
- [XML Injection](/resources/XML_Injection.md)
- [LDAP Injection](/resources/LDAP_Injection.md)
- [Command Injection](/resources/Command_Injection.md)
- [NoSQL Injection](/resources/NoSQL_Injection.md)
- [CRLF Injection](/resources/CRLF_Injection.md)
- [HTML Injection](/resources/HTML_Injection.md)
- [XPath Injection](/resources/XPath_Injection.md)
- [Script Injection (JavaScript Injection, HTML Injection)](/resources/Script_Injection.md)
- [XML External Entity (XXE) Injection](/resources/XXE_Injection.md)
- [Entity Injection](/resources/Entity_Injection.md)
- [Code Injection via API (e.g., SOAP or JSON APIs)](/resources/Code_Injection_via_API.md)

### 2. Authentication Vulnerabilities
- [Broken Authentication](/resources/Broken_Authentication.md)
- [Session Fixation](/resources/Session_Fixation.md)
- [Credential Stuffing](/resources/Credential_Stuffing.md)
- [Password Guessing](/resources/Password_Guessing.md)
- [Weak Password Recovery Mechanisms](/resources/Weak_Password_Recovery_Mechanisms.md)
- [Brute Force Attacks](/resources/Brute_Force_Attacks.md)
- [Exposed Session Tokens](/resources/Exposed_Session_Tokens.md)
- [Predictable Login Endpoints](/resources/Predictable_Login_Endpoints.md)
- [Token or Session Expiration Flaws](/resources/Token_or_Session_Expiration_Flaws.md)
- [Insecure Password Storage (Weak Hashing or Plaintext Passwords)](/resources/Insecure_Password_Storage.md)
- [Multi-Factor Authentication Bypass](/resources/Multi-Factor_Authentication_Bypass.md)
- [Insecure OAuth / OpenID Configuration](/resources/Insecure_OAuth-OpenID_Configuration.md)
- [Unprotected API Authentication](/resources/Unprotected_API_Authentication.md)
- [Mobile App Authentication Weaknesses (e.g., weak PIN storage)](/resources/Mobile_App_Authentication_Weaknesses.md)

### 3. Access Control Vulnerabilities
- Broken Access Control
- Insecure Direct Object References (IDOR)
- Privilege Escalation
- Mass Assignment Vulnerabilities
- Insecure Function-Level Access Control
- Path Traversal
- Horizontal Privilege Escalation
- Vertical Privilege Escalation
- Access Control to User-Inputted Data
- Uncontrolled Access to Mobile App Resources
- Improper API Access Control
- API Rate Limiting Issues

### 4. Cross-Site Scripting (XSS)
- Reflected XSS
- Stored XSS
- DOM-Based XSS
- Self-XSS
- Blind XSS
- Cross-Site Script Inclusion (XSSI)
- Mobile App XSS (via WebViews)
- Cross-Site Script Execution via APIs

### 5. Cross-Site Request Forgery (CSRF)
- Classic CSRF
- CSRF with SameSite Cookies
- Malicious Link/Script Injection for CSRF
- Token Mismanagement in CSRF
- Mobile App CSRF Vulnerabilities
- CSRF via Unauthenticated API Endpoints

### 6. Insecure Deserialization
- Object Injection (PHP/Java Deserialization)
- Remote Code Execution (RCE) via Insecure Deserialization
- Insecure Deserialization Leading to Privilege Escalation
- Mobile App Insecure Deserialization (e.g., for Local Storage)

### 7. Security Misconfiguration
- Default Configuration Vulnerabilities
- Misconfigured Security Headers (e.g., CORS, X-Frame-Options)
- Open Ports and Services
- Verbose Error Messages
- Lack of Secure Configuration in Web Servers
- Default Accounts or Unchanged Credentials
- Improper Caching Configuration
- Mobile App Insecure Configurations (e.g., Debugging Enabled)
- Misconfigured API Endpoints
- Misconfigured Firewall Rules
- Misconfigured Load Balancer

### 8. Sensitive Data Exposure
- Insecure Transmission (HTTP instead of HTTPS)
- Weak Encryption Algorithms
- Sensitive Data in URLs, Logs, or Cookies
- Improper Key Management
- Insecure Storage of Sensitive Data (Unhashed Passwords)
- Exposed Secrets in Source Code
- Mobile App Sensitive Data Leakage (e.g., in logs or backups)
- Exposed API Keys or Tokens in Source Code

### 9. Insufficient Logging & Monitoring
- Lack of Proper Logging
- Failure to Log Failed Authentication Attempts
- Absence of Alerts on Suspicious Activities
- Log Tampering
- Sensitive Data in Logs
- Lack of Audit Trails for Critical Actions
- Mobile App Insufficient Logging for Security Events
- API Request/Response Log Tampering

### 10. Cross-Origin Resource Sharing (CORS) Issues
- CORS Misconfiguration
- CORS with Open or Misconfigured Origins
- CORS with Insecure Cookies
- CORS with Malicious Request Forging
- Insecure CORS Configuration in Mobile Apps with Webviews

### 11. Security Headers Issues
- Missing or Misconfigured HTTP Security Headers
- Missing Content Security Policy (CSP)
- Lack of Strict Transport Security (HSTS)
- Missing X-Content-Type-Options
- X-XSS-Protection Misconfigurations
- X-Frame-Options Misconfiguration
- Referrer-Policy Misconfiguration

### 12. File Upload Vulnerabilities
- Malicious File Upload (Web Shells, Scripts, etc.)
- Insecure File Handling (No Antivirus Scanning)
- Unrestricted File Type Upload
- Insecure File Storage Locations
- File Name Injection
- File Upload Vulnerabilities in Mobile Apps

### 13. XML External Entity (XXE) Injection
- Classic XXE
- Blind XXE
- XXE Leading to SSRF
- XML Injection
- XXE in API Payloads

### 14. Business Logic Vulnerabilities
- Race Conditions
- Improper Workflow Implementation
- Inconsistent Application States
- Insecure Workflow Transitions
- Sensitive Data Exposure via Business Logic
- Unintended Mobile App Behavior
- API Logic Flaws

### 15. Server-Side Request Forgery (SSRF)
- Classic SSRF
- SSRF with Internal Network Access
- SSRF to Cloud Metadata API
- SSRF to Access Private Resources
- SSRF Leading to RCE
- Mobile App SSRF via Webviews

### 16. Clickjacking
- Frame Injection Attacks
- UI Redressing
- Clickjacking with Transparent Layers
- Manipulation of Web Interfaces with Hidden Frames
- Mobile App UI Manipulation via Clickjacking

### 17. Improper Input Validation
- Untrusted Data Accepted as Input
- Improper Input Sanitization
- Input Validation Bypasses
- Regular Expression Flaws (ReDoS)
- Buffer Overflow via Malicious Input
- Mobile App Input Validation Bypass
- API Input Validation Flaws

### 18. Broken Cryptography
- Weak or Deprecated Encryption Algorithms
- Improper Key Management
- Weak Hashing Algorithms
- Insecure Data Decryption
- Exposed Encryption Keys or Secrets
- Mobile App Cryptography Flaws (e.g., weak PIN encryption)

### 19. Denial of Service (DoS)
- Resource Exhaustion (CPU, Memory)
- Distributed Denial of Service (DDoS)
- Large Payload DoS
- Excessive Resource Consumption
- Server Crash Due to Unexpected Input
- Mobile App DoS via Insecure Network Requests

### 20. Out-of-Bounds Access
- Buffer Overflow (Stack Overflow)
- Out-of-Bounds Read/Write
- Heap Overflow
- Memory Corruption in Mobile Apps
- Out-of-Bounds API Access

### 21. Application Logic Flaws
- Logic Flaws Leading to Privilege Escalation
- Unintended Operations
- Bypassing Security Policies
- Authorization Bypass Using Business Logic
- Misconfiguration of Mobile App Logic Flows

### 22. Misconfigured APIs
- Insecure API Endpoints
- No Authentication on APIs
- Unencrypted API Endpoints
- Overexposed API Data
- API Rate Limiting Issues
- Mobile App API Misconfigurations

### 23. Insufficient Session Management
- Session Fixation
- Predictable Session IDs
- Session Hijacking
- Session Timeout Misconfigurations
- Cross-Site Script Inclusion via Cookies (CSRF)
- Cookies Not Set with Secure or HttpOnly Flags
- Mobile App Session Management Weaknesses

### 24. Remote Code Execution (RCE)
- Command Injection Vulnerabilities
- Remote Code Execution via File Upload
- RCE via XML External Entities
- RCE via Insecure Deserialization
- RCE via API Vulnerabilities

### 25. Insufficient Protection Against Bot Attacks
- Captcha Bypassing
- Automated Attack Prevention Failure
- Lack of Rate Limiting
- Bot Abuse of Authentication/Forms
- Mobile App Bot Mitigation Flaws

### 26. API Security Issues
- Unsecured API Endpoints
- Exposed API Keys or Tokens
- Lack of API Authentication
- Unprotected API Data
- Unvalidated API Inputs

### 27. Third-Party Library Vulnerabilities
- Outdated Libraries
- Vulnerable Dependencies
- Insecure Packages/Plugins
- Use of Vulnerable SDKs/APIs
- Mobile App Third-Party Library Vulnerabilities

### 28. Content Injection Vulnerabilities
- Cross-Site Script Inclusion (XSSI)
- HTML Injection
- JSON Injection
- JavaScript Injection
- Mobile App Content Injection via WebViews

### 29. Insufficient File Permissions
- File Permissions in Web Root
- Incorrect Access Control for Files
- Sensitive Files Exposed to Public
- Writable Folders Accessible by Unauthorized Users
- Improper File Permission in System/Network Apps

### 30. Path Traversal
- Directory Traversal (../)
- Path Injection Vulnerabilities
- Access to Arbitrary Files Outside of Web Root
- Mobile App Path Traversal
