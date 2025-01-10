# 1. Pre-Engagement Phase (تفاهم نامه)
### Scope Definition
- Identify in-scope assets: List all domains, subdomains, IP ranges, web apps, APIs, networks.
- Confirm out-of-scope assets: Explicitly document systems/services to avoid.
### Rules of Engagement (ROE)
- Timing:
  - Specify testing hours (e.g., weekdays 9 AM–5 PM).
  - Include blackout periods (e.g., during major deployments).
- Test Type:
  - Black-box: No prior knowledge.
  - Gray-box: Limited credentials or architecture knowledge.
  - White-box: Full access to source code and architecture diagrams.
- Critical Findings Process:
  - Define how findings like RCE or privilege escalation will be escalated immediately.
### Legal Documentation
- Authorization to Test: Signed letter from stakeholders confirming consent.
- NDA: Ensure non-disclosure agreements are in place.


# 2. Information Gathering (جلسه شناخت)
### Passive Reconnaissance
- OSINT Tools:
  - theHarvester: Gather emails, subdomains, and metadata.
    - `theHarvester -d example.com -b all`
  - Shodan: Search for exposed services
    - `shodan search "org:Example Company"`
  - Google Dorks:
    - `site:example.com filetype:pdf`
    - `site:example.com intitle:"index of"`
- Public Repositories: Search for leaked credentials or sensitive files
  - `git clone https://github.com/example/repo.git`
  - `grep -ri "password" repo/`
### Active Reconnaissance
- DNS Enumeration:
  - Query records: `dig example.com ANY`
  - Zone transfer (if misconfigured): `dig axfr @ns1.example.com example.com`
- Port Scanning:
  - Full TCP/UDP scan: `nmap -sS -sU -p- -T4 example.com`
- Web Application Enumeration:
  - Identify directories: `gobuster dir -u https://example.com -w /path/to/wordlist.txt`

### Architecture-Related Vulnerabilities
- [Architectural Design Flaws](/resources/Architectural_Design_Flaws.md)
- [Insufficient Threat Modeling](/resources/Insufficient_Threat_Modeling.md)
- [Insecure Cloud Architecture](/resources/Insecure_Cloud_Architecture.md)
- [Insufficient Secure Communication Design](/resources/Insufficient_Secure_Communication_Design.md)
- [Lack of Secure Software Development Lifecycle (SDLC)](/resources/Lack_of_Secure_Software_Development_Lifecycle.md)

# 3. Threat Modeling and Target Prioritization (طراحی تست)
### Attack Surface Analysis:
- Create a diagram of all services, endpoints, and applications.
- Use tools like OWASP Threat Dragon to visualize threats.
### Prioritization Criteria:
- Business-critical systems: Databases, payment gateways, sensitive APIs.
- Historical vulnerabilities: Legacy software and outdated libraries.

# 4. Vulnerability Assessment
### Authentication and Session Management
- [Weak or Default Credentials](/resources/Weak_or_Default_Credentials.md)
- [Insufficient Password Complexity Policies](/resources/Insufficient_Password_Complexity_Policies.md)
- [Credential Stuffing](/resources/Credential_Stuffing.md)
- [Missing or Insecure Multi-Factor Authentication (MFA)](/resources/Missing_or_Insecure_Multi-Factor_Authentication.md)
- [Session Fixation](/resources/Session_Fixation.md)
- [Improper Session Expiry or Timeout](/resources/Improper_Session_Expiry_or_Timeout.md)
- [Use of Hardcoded Credentials](/resources/Use_of_Hardcoded_Credentials.md)
- [Token Hijacking (e.g., JWT tampering)](/resources/Token_Hijacking.md)
- [Insufficient Token Expiration or Revocation](/resources/Insufficient_Token_Expiration_or_Revocation.md)
- [Broken Authentication](/resources/Broken_Authentication.md)
- [Password Guessing](/resources/Password_Guessing.md)
- [Weak Password Recovery Mechanisms](/resources/Weak_Password_Recovery_Mechanisms.md)
- [Brute Force Attacks](/resources/Brute_Force_Attacks.md)
- [Exposed Session Tokens](/resources/Exposed_Session_Tokens.md)
- [Predictable Login Endpoints](/resources/Predictable_Login_Endpoints.md)
- [Token or Session Expiration Flaws](/resources/Token_or_Session_Expiration_Flaws.md)
- [Insecure Password Storage](/resources/Insecure_Password_Storage.md)
- [Multi-Factor Authentication Bypass](/resources/Multi-Factor_Authentication_Bypass.md)
- [Insecure OAuth-OpenID Configuration](/resources/Insecure_OAuth-OpenID_Configuration.md)
- [Unprotected API Authentication](/resources/Unprotected_API_Authentication.md)
- [Mobile App Authentication Weaknesses](/resources/Mobile_App_Authentication_Weaknesses.md)
- [Cross-Protocol Session Hijacking](/resources/Cross-Protocol_Session_Hijacking.md)
- [JWT Attacks](/resources/JWT_Attacks.md)

### Access Control and Authorization
- Broken Access Control
- Privilege Escalation
- Insecure Direct Object References (IDOR)
- Overly Permissive API Permissions
- Role-Based Access Control (RBAC) Misconfigurations
- Insecure File and Directory Permissions
- Excessive Data Exposure in APIs
- Unrestricted Access to Critical Functions or Endpoints
- Mass Assignment Vulnerabilities
- Insecure Function-Level Access Control
- Horizontal Privilege Escalation
- Vertical Privilege Escalation
- Access Control to User-Inputted Data
- Improper API Access Control
- Authorization Bypass via Business Logic
- Improper API Access Control
- Uncontrolled Access to Mobile App Resources

### Input Validation and Injection
- SQL Injection
- NoSQL Injection
- Command Injection
- LDAP Injection
- Cross-Site Scripting (XSS)
  - Stored XSS
  - Reflected XSS
  - DOM-based XSS
- HTML Injection
- XML External Entity (XXE) Injection
- CRLF Injection
- HTTP Header Injection
- Cross-Site Request Forgery (CSRF)
- Template Injection
- Business Logic Injection
- XPath Injection
- Script Injection
- Entity Injection
- Blind Injection Attacks
- File and Resource Handling

### File and Resource Handling
- Unrestricted File Upload
- Directory Traversal
- Insecure File Parsing
- File Inclusion (Local/Remote)
- Unsafe Use of Temporary Files
- Server-Side Request Forgery (SSRF)
- Open Redirects
- Uncontrolled Zip Bombs or Archive Extraction
- Malicious File Upload
- Insecure File Handling
- Unrestricted File Type Upload
- Insecure File Storage Locations
- File Name Injection
- File Upload Vulnerabilities in Mobile Apps
- Path Traversal in Uploaded Files
- Server-Side File Processing Vulnerabilities
- Path Traversal via User Input

### Cryptographic and Data Protection Issues
- Weak Encryption Algorithms
- Missing Encryption for Sensitive Data (at rest/in transit)
- Hardcoded Cryptographic Keys
- Improper Key Management (e.g., key exposure)
- Insecure Random Number Generation
- Padding Oracle Attacks
- Plaintext Storage of Sensitive Data
- Improper Certificate Validation
- Token Replay Attacks (e.g., in JWT or OAuth)
- Sensitive Data in URLs, Logs, or Cookies
- Exposed Secrets in Source Code
- Weak Hashing Algorithms
- Insecure Data Decryption
- Exposed Encryption Keys or Secrets
- Mobile App Cryptography Flaws
- Insecure SSL-TLS Implementation

### Security Misconfigurations
- Unpatched or Outdated Software
- Misconfigured Security Headers (e.g., CSP, HSTS)
- Debug Information Exposed in Production
- Excessive Permissions in Cloud Storage (e.g., S3 buckets)
- Default Configurations Left Enabled
- Unnecessary Features or Services Running (e.g., Telnet)
- Default Accounts or Unchanged Credentials
- Improper Caching Configuration
- Misconfigured API Endpoints
- Misconfigured Firewall Rules
- Misconfigured Load Balancer
- Cloud Security Misconfigurations
- Exposed API Keys or Tokens in Source Code
- API Rate Limiting Issues
- Mobile App Sensitive Data Leakage
- Insecure Transmission

### Mobile Application-Specific Vulnerabilities
- Insecure Data Storage (e.g., SQLite, Shared Preferences)
- Insecure Use of Platform APIs (e.g., Keychain, Keystore)
- Lack of Binary Protection (e.g., reverse engineering, tampering)
- Insecure Inter-Process Communication (IPC)
- Sensitive Data Exposure via Logs or Backups
- Unprotected Sensitive Activities (e.g., screenshot leaks)
- Insufficient Root/Jailbreak Detection
- Improper Use of WebViews (e.g., JavaScript-enabled WebView)
- Mobile App Insecure Configurations
- Mobile App Session Management Weaknesses
- Mobile App Cryptography Flaws
- Mobile App API Misconfigurations
- Mobile App UI Manipulation via Clickjacking
- Mobile App Path Traversal

### API-Specific Vulnerabilities
- Lack of Rate Limiting (e.g., brute force attacks)
- Mass Assignment Vulnerabilities
- Insecure Deserialization
- Misconfigured CORS Policies
- Overly Verbose Error Messages (revealing backend details)
- GraphQL-Specific Issues (e.g., excessive introspection, data exposure)
- API Key Exposure (e.g., in client-side code or logs)
- Improper API Versioning (leading to untested, outdated endpoints)
- Improper API Authorization
- Unencrypted API Endpoints
- Overexposed API Data
- API Information Disclosure
- Improperly Scoped API Permissions
- API Logic Flaws

### System Application-Specific Vulnerabilities
- Buffer Overflows (Heap/Stack)
- Use After Free
- Out-of-Bounds Read/Write
- Integer Overflow or Underflow
- NULL Pointer Dereference
- Race Conditions (TOCTOU issues)
- Privilege Escalation via Misconfigured Services
- DLL Hijacking or Insecure Library Loading
- Lack of ASLR (Address Space Layout Randomization)
- Weak Kernel Hardening

### Data and Privacy Vulnerabilities
- Sensitive Data Exposure in Logs
- Data Leakage via Cache or Temporary Files
- Improper Data Anonymization Techniques
- Unencrypted Backups or Offline Storage

### Logging and Monitoring
- Insufficient Logging for Security Events
- Missing Alerting Mechanisms for Anomalous Activities
- Insecure Log Storage (e.g., plaintext logs)
- Failure to Detect Anomalous Requests
- Lack of Audit Trails for Critical Actions
- API Request-Response Log Tampering

### Client-Side Vulnerabilities
- DOM-based XSS
- Clickjacking
- Insecure Client-Side Storage (e.g., localStorage, IndexedDB)
- Weak JavaScript or DOM Manipulation Protections
- CSRF Tokens Stored Insecurely

### Network and Protocol Vulnerabilities
- Insecure Use of Protocols (e.g., HTTP instead of HTTPS)
- Weak Wi-Fi Protections (e.g., WPA2 vulnerabilities)
- Insecure DNS (e.g., DNS Cache Poisoning)
- Man-in-the-Middle (MITM) Vulnerabilities
- Insecure Communication in Microservices
- Unencrypted Data in Transit

### Business Logic and Design Flaws
- Inconsistent Workflow Logic
- Lack of Account Lockout After Failed Attempts
- Improper Validation of Critical Operations (e.g., fund transfers)
- Design Assumptions That Bypass Security Controls
- Unauthorized API Endpoints
- Unintended Mobile App Behavior
- Misconfiguration of Mobile App Logic Flows
- Logic Flaws Leading to Privilege Escalation
- Unintended Operations

# 5. Exploitation & Post-Exploitation

# 6. Reporting
- **Vulnerability Details:** Vulnerability name, description, impact, and proof of concept (PoC).
- **Screenshots:** Show exploitation steps for clarity.
- **Risk Assessment:** Use CVSS scores for prioritization.
