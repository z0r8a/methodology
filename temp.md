# 1. Injection Vulnerabilities
- SQL Injection (SQLi)
- XML Injection
- LDAP Injection
- Command Injection
- NoSQL Injection
- CRLF Injection
- XPath Injection
- Script Injection (JavaScript Injection)
- XML External Entity (XXE) Injection
- Entity Injection
- Code Injection via API (e.g., SOAP or JSON APIs)
- Blind Injection Attacks (Out-of-Band)

# 2. Authentication Vulnerabilities
- Broken Authentication
- Session Fixation
- Credential Stuffing
- Password Guessing
- Weak Password Recovery Mechanisms
- Brute Force Attacks
- Exposed Session Tokens
- Predictable Login Endpoints
- Token or Session Expiration Flaws
- Insecure Password Storage (Weak Hashing or Plaintext Passwords)
- Multi-Factor Authentication Bypass
- Insecure OAuth / OpenID Configuration
- Unprotected API Authentication
- Mobile App Authentication Weaknesses (e.g., weak PIN storage)
- Cross-Protocol Session Hijacking
- JWT Attacks (JWT Manipulation, Forging)

# 3. Access Control Vulnerabilities
- Broken Access Control
- Insecure Direct Object References (IDOR)
- Privilege Escalation
- Mass Assignment Vulnerabilities
- Insecure Function-Level Access Control
- Horizontal Privilege Escalation
- Vertical Privilege Escalation
- Access Control to User-Inputted Data
- Improper API Access Control
- Authorization Bypass via Business Logic
- Path Traversal
- Uncontrolled Access to Mobile App Resources
- Improper API Access Control
- API Rate Limiting Issues

# 4. Cross-Site Scripting (XSS)
- Reflected XSS
- Stored XSS
- DOM-Based XSS
- Self-XSS
- Blind XSS
- Cross-Site Script Inclusion (XSSI)
- Mobile App XSS (via WebViews)
- XSS via APIs
- XSS in WebSocket Connections

# 5. Cross-Site Request Forgery (CSRF)
- Classic CSRF
- CSRF with SameSite Cookies
- Malicious Link/Script Injection for CSRF
- Token Mismanagement in CSRF
- Mobile App CSRF Vulnerabilities
- CSRF via Unauthenticated API Endpoints

# 6. Insecure Deserialization
- Object Injection (PHP/Java Deserialization)
- Remote Code Execution (RCE) via Insecure Deserialization
- Insecure Deserialization Leading to Privilege Escalation
- Mobile App Insecure Deserialization (e.g., for Local Storage)

# 7. Security Misconfiguration
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
- Cloud Security Misconfigurations (e.g., AWS S3 buckets, IAM permissions)

# 8. Sensitive Data Exposure
- Insecure Transmission (HTTP instead of HTTPS)
- Weak Encryption Algorithms
- Sensitive Data in URLs, Logs, or Cookies
- Improper Key Management
- Insecure Storage of Sensitive Data (Unhashed Passwords)
- Exposed Secrets in Source Code
- Mobile App Sensitive Data Leakage (e.g., in logs or backups)
- Exposed API Keys or Tokens in Source Code
- Weak Cryptographic Storage (e.g., weak PIN encryption)

# 9. Insufficient Logging & Monitoring
- Lack of Proper Logging
- Failure to Log Failed Authentication Attempts
- Absence of Alerts on Suspicious Activities
- Log Tampering
- Sensitive Data in Logs
- Lack of Audit Trails for Critical Actions
- Mobile App Insufficient Logging for Security Events
- API Request/Response Log Tampering
- Failure to Detect Anomalous Requests (Rate Limiting, Sudden Traffic Spikes)

# 10. Cross-Origin Resource Sharing (CORS) Issues
- CORS Misconfiguration
- CORS with Open or Misconfigured Origins
- CORS with Insecure Cookies
- CORS with Malicious Request Forging
- Insecure CORS Configuration in Mobile Apps with WebViews
- CORS Exploitation via APIs

# 11. Security Headers Issues
- Missing or Misconfigured HTTP Security Headers
- Missing Content Security Policy (CSP)
- Lack of Strict Transport Security (HSTS)
- Missing X-Content-Type-Options
- X-XSS-Protection Misconfigurations
- X-Frame-Options Misconfiguration
- Referrer-Policy Misconfiguration

# 12. File Upload Vulnerabilities
- Malicious File Upload (Web Shells, Scripts, etc.)
- Insecure File Handling (No Antivirus Scanning)
- Unrestricted File Type Upload
- Insecure File Storage Locations
- File Name Injection
- File Upload Vulnerabilities in Mobile Apps
- Path Traversal in Uploaded Files
- Server-Side File Processing Vulnerabilities

# 13. Business Logic Vulnerabilities
- Race Conditions
- Improper Workflow Implementation
- Inconsistent Application States
- Insecure Workflow Transitions
- Sensitive Data Exposure via Business Logic
- Unintended Mobile App Behavior
- API Logic Flaws (Improper Business Flow)

# 14. Server-Side Request Forgery (SSRF)
- Classic SSRF
- SSRF with Internal Network Access
- SSRF to Cloud Metadata API
- SSRF to Access Private Resources
- SSRF Leading to RCE
- Mobile App SSRF via WebViews

# 15. Clickjacking
- Frame Injection Attacks
- UI Redressing
- Clickjacking with Transparent Layers
- Manipulation of Web Interfaces with Hidden Frames
- Mobile App UI Manipulation via Clickjacking

# 16. Improper Input Validation
- Untrusted Data Accepted as Input
- Improper Input Sanitization
- Input Validation Bypasses
- Regular Expression Flaws (ReDoS)
- Buffer Overflow via Malicious Input
- Mobile App Input Validation Bypass
- API Input Validation Flaws
- Path Traversal via User Input

# 17. Broken Cryptography
- Weak or Deprecated Encryption Algorithms
- Improper Key Management
- Weak Hashing Algorithms
- Insecure Data Decryption
- Exposed Encryption Keys or Secrets
- Mobile App Cryptography Flaws (e.g., weak PIN encryption)
- Insecure SSL/TLS Implementation

# 18. Denial of Service (DoS)
- Resource Exhaustion (CPU, Memory)
- Distributed Denial of Service (DDoS)
- Large Payload DoS
- Excessive Resource Consumption
- Server Crash Due to Unexpected Input
- Mobile App DoS via Insecure Network Requests
- Slowloris and Connection Exhaustion
- Application-Level DoS via Complex Calculations

# 19. Out-of-Bounds Access
- Buffer Overflow (Stack Overflow)
- Out-of-Bounds Read/Write
- Heap Overflow
- Memory Corruption in Mobile Apps
- Out-of-Bounds API Access

# 20. Application Logic Flaws
- Logic Flaws Leading to Privilege Escalation
- Unintended Operations
- Bypassing Security Policies
- Authorization Bypass Using Business Logic
- Misconfiguration of Mobile App Logic Flows
- Improper API Logic (e.g., race conditions, flawed state management)

# 21. Misconfigured APIs
- Insecure API Endpoints
- No Authentication on APIs
- Unencrypted API Endpoints
- Overexposed API Data
- API Rate Limiting Issues
- Mobile App API Misconfigurations
- Excessive API Permissions
- Improper API Authorization (e.g., scope violations)

# 22. Insufficient Session Management
- Session Fixation
- Predictable Session IDs
- Session Hijacking
- Session Timeout Misconfigurations
- Cross-Site Script Inclusion via Cookies (CSRF)
- Cookies Not Set with Secure or HttpOnly Flags
- Mobile App Session Management Weaknesses
- Session Reuse and Token Revocation Failure

# 23. Remote Code Execution (RCE)
- Command Injection Vulnerabilities
- Remote Code Execution via File Upload
- RCE via XML External Entities
- RCE via Insecure Deserialization
- RCE via API Vulnerabilities
- RCE via WebSocket Messages

# 24. Insufficient Protection Against Bot Attacks
- Captcha Bypassing
- Automated Attack Prevention Failure
- Lack of Rate Limiting
- Bot Abuse of Authentication/Forms
- Mobile App Bot Mitigation Flaws
- Fingerprinting Bypass for CAPTCHA Systems

# 25. API Security Issues
- Unsecured API Endpoints
- Exposed API Keys or Tokens
- Lack of API Authentication
- Unprotected API Data
- Unvalidated API Inputs
- API Information Disclosure
- Improperly Scoped API Permissions

# 26. Third-Party Library Vulnerabilities
- Outdated Libraries
- Vulnerable Dependencies
- Insecure Packages/Plugins
- Use of Vulnerable SDKs/APIs
- Mobile App Third-Party Library Vulnerabilities
- Supply Chain Attacks via External Libraries

# 27. Content Injection Vulnerabilities
- Cross-Site Script Inclusion (XSSI)
- HTML Injection
- JSON Injection
- JavaScript Injection
- Mobile App Content Injection via WebViews

# 28. Insufficient File Permissions
- File Permissions in Web Root
- Incorrect Access Control for Files
- Sensitive Files Exposed to Public
- Writable Folders Accessible by Unauthorized Users
- Improper File Permission in System/Network Apps

# 29. Path Traversal
- Directory Traversal (../)
- Path Injection Vulnerabilities
- Access to Arbitrary Files Outside of Web Root
- Mobile App Path Traversal
