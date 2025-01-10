# Authentication and Session Management
- Weak or Default Credentials
- Insufficient Password Complexity Policies
- Credential Stuffing
- Missing or Insecure Multi-Factor Authentication (MFA)
- Session Fixation
- Improper Session Expiry or Timeout
- Use of Hardcoded Credentials
- Token Hijacking (e.g., JWT tampering)
- Insufficient Token Expiration or Revocation
- Broken Authentication
- Password Guessing
- Weak Password Recovery Mechanisms
- Brute Force Attacks
- Exposed Session Tokens
- Predictable Login Endpoints
- Token or Session Expiration Flaws
- Insecure Password Storage
- Multi-Factor Authentication Bypass
- Insecure OAuth-OpenID Configuration
- Unprotected API Authentication
- Mobile App Authentication Weaknesses
- Cross-Protocol Session Hijacking
- JWT Attacks

# Access Control and Authorization
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

# Input Validation and Injection
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

# File and Resource Handling
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

# Cryptographic and Data Protection Issues
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

# Security Misconfigurations
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

# Mobile Application-Specific Vulnerabilities
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

# API-Specific Vulnerabilities
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

# System Application-Specific Vulnerabilities
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

# Data and Privacy Vulnerabilities
- Sensitive Data Exposure in Logs
- Data Leakage via Cache or Temporary Files
- Improper Data Anonymization Techniques
- Unencrypted Backups or Offline Storage

# Logging and Monitoring
- Insufficient Logging for Security Events
- Missing Alerting Mechanisms for Anomalous Activities
- Insecure Log Storage (e.g., plaintext logs)
- Failure to Detect Anomalous Requests
- Lack of Audit Trails for Critical Actions
- API Request-Response Log Tampering

# Client-Side Vulnerabilities
- DOM-based XSS
- Clickjacking
- Insecure Client-Side Storage (e.g., localStorage, IndexedDB)
- Weak JavaScript or DOM Manipulation Protections
- CSRF Tokens Stored Insecurely

# Network and Protocol Vulnerabilities
- Insecure Use of Protocols (e.g., HTTP instead of HTTPS)
- Weak Wi-Fi Protections (e.g., WPA2 vulnerabilities)
- Insecure DNS (e.g., DNS Cache Poisoning)
- Man-in-the-Middle (MITM) Vulnerabilities
- Insecure Communication in Microservices
- Unencrypted Data in Transit

# Business Logic and Design Flaws
- Inconsistent Workflow Logic
- Lack of Account Lockout After Failed Attempts
- Improper Validation of Critical Operations (e.g., fund transfers)
- Design Assumptions That Bypass Security Controls
- Unauthorized API Endpoints
- Unintended Mobile App Behavior
- Misconfiguration of Mobile App Logic Flows
- Logic Flaws Leading to Privilege Escalation
- Unintended Operations

# Architecture-Related Vulnerabilities
- Architectural Design Flaws
  - Lack of Defense-in-Depth: Failure to apply multiple layers of security across the system.
  - Overly Complex Architecture: Complex and convoluted designs make the system harder to secure.
  - Improper Separation of Duties: Failure to enforce strict role-based separation, allowing for too much privilege in one entity.
  - Single Point of Failure: A critical component failure leads to full system compromise.
  - Lack of Redundancy and Scalability: Lack of failover mechanisms or scalability compromises availability.
  - Insecure Microservices Communication: Unsecured communication between microservices or containers, enabling unauthorized access.
  - Hardcoding Sensitive Data in Architecture: Sensitive data hardcoded in configuration files, scripts, or code.
- Insufficient Threat Modeling
  - Failure to Identify Potential Threats: Missing or incomplete threat models, leading to unforeseen risks.
  - Improper Handling of External Dependencies: Failure to evaluate security risks from third-party services or components.
- Insecure Cloud Architecture
  - Misconfigured Cloud Permissions: Inappropriate access control policies leading to data exposure or unauthorized access.
  - Improper Segmentation in Cloud Environments: Insufficient isolation between cloud services, exposing critical data.
  - Exposed API Endpoints in Cloud Architecture: Insecure or unmonitored API endpoints exposed in the cloud.
  - Insecure Cloud Storage and Data Leakage: Cloud storage services misconfigured to allow data leakage.
- Insufficient Secure Communication Design
  - Unencrypted Data in Transit: Data transmitted without proper encryption mechanisms (e.g., HTTP instead of HTTPS).
  - Weak Transport Layer Security: Use of deprecated or weak SSL/TLS configurations.
- Lack of Secure Software Development Lifecycle (SDLC)
  - Failure to Integrate Security from the Beginning: Ignoring security during the design and development phases.
  - Lack of Regular Security Audits and Penetration Testing: Absence of continuous or periodic security testing within the lifecycle.
