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
- [Broken Access Control](/resources/Broken_Access_Control.md)
- [Insecure Direct Object References (IDOR)](/resources/Insecure_Direct_Object_References.md)
- [Privilege Escalation](/resources/Privilege_Escalation.md)
- [Mass Assignment Vulnerabilities](/resources/Mass_Assignment_Vulnerabilities.md)
- [Insecure Function-Level Access Control](/resources/Insecure_Function-Level_Access_Control.md)
- [Path Traversal](/resources/Path_Traversal.md)
- [Horizontal Privilege Escalation](/resources/Horizontal_Privilege_Escalation.md)
- [Vertical Privilege Escalation](/resources/Vertical_Privilege_Escalation.md)
- [Access Control to User-Inputted Data](/resources/Access_Control_to_User-Inputted_Data.md)
- [Uncontrolled Access to Mobile App Resources](/resources/Uncontrolled_Access_to_Mobile_App_Resources.md)
- [Improper API Access Control](/resources/Improper_API_Access_Control.md)
- [API Rate Limiting Issues](/resources/API_Rate_Limiting_Issues.md)

### 4. Cross-Site Scripting (XSS)
- [Reflected XSS](/resources/Reflected_XSS.md)
- [Stored XSS](/resources/Stored_XSS.md)
- [DOM-Based XSS](/resources/DOM-Based_XSS.md)
- [Self-XSS](/resources/Self-XSS.md)
- [Blind XSS](/resources/Blind_XSS.md)
- [Cross-Site Script Inclusion (XSSI)](/resources/Cross-Site_Script_Inclusion.md)
- [Mobile App XSS (via WebViews)](/resources/Mobile_App_XSS.md)
- [Cross-Site Script Execution via APIs](/resources/Cross-Site_Script_Execution_via_APIs.md)

### 5. Cross-Site Request Forgery (CSRF)
- [Classic CSRF](/resources/Classic_CSRF.md)
- [CSRF with SameSite Cookies](/resources/CSRF_with_SameSite_Cookies.md)
- [Malicious Link/Script Injection for CSRF](/resources/Malicious_Link-Script_Injection_for_CSRF.md)
- [Token Mismanagement in CSRF](/resources/Token_Mismanagement_in_CSRF.md)
- [Mobile App CSRF Vulnerabilities](/resources/Mobile_App_CSRF_Vulnerabilities.md)
- [CSRF via Unauthenticated API Endpoints](/resources/CSRF_via_Unauthenticated_API_Endpoints.md)

### 6. Insecure Deserialization
- [Object Injection (PHP/Java Deserialization)](/resources/Object_Injection.md)
- [Remote Code Execution (RCE) via Insecure Deserialization](/resources/RCE_via_Insecure_Deserialization.md)
- [Insecure Deserialization Leading to Privilege Escalation](/resources/Insecure_Deserialization_Leading_to_Privilege_Escalation.md)
- [Mobile App Insecure Deserialization (e.g., for Local Storage)](/resources/Mobile_App_Insecure_Deserialization.md)

### 7. Security Misconfiguration
- [Default Configuration Vulnerabilities](/resources/Default_Configuration_Vulnerabilities.md)
- [Misconfigured Security Headers (e.g., CORS, X-Frame-Options)](/resources/Misconfigured_Security_Headers.md)
- [Open Ports and Services](/resources/Open_Ports_and_Services.md)
- [Verbose Error Messages](/resources/Verbose_Error_Messages.md)
- [Lack of Secure Configuration in Web Servers](/resources/Lack_of_Secure_Configuration_in_Web_Servers.md)
- [Default Accounts or Unchanged Credentials](/resources/Default_Accounts_or_Unchanged_Credentials.md)
- [Improper Caching Configuration](/resources/Improper_Caching_Configuration.md)
- [Mobile App Insecure Configurations (e.g., Debugging Enabled)](/resources/Mobile_App_Insecure_Configurations.md)
- [Misconfigured API Endpoints](/resources/Misconfigured_API_Endpoints.md)
- [Misconfigured Firewall Rules](/resources/Misconfigured_Firewall_Rules.md)
- [Misconfigured Load Balancer](/resources/Misconfigured_Load_Balancer.md)

### 8. Sensitive Data Exposure
- [Insecure Transmission (HTTP instead of HTTPS)](/resources/Insecure_Transmission.md)
- [Weak Encryption Algorithms](/resources/Weak_Encryption_Algorithms.md)
- [Sensitive Data in URLs, Logs, or Cookies](/resources/Sensitive_Data_in_URLs_Logs_Cookies.md)
- [Improper Key Management](/resources/Improper_Key_Management.md)
- [Insecure Storage of Sensitive Data (Unhashed Passwords)](/resources/Insecure_Storage_of_Sensitive_Data.md)
- [Exposed Secrets in Source Code](/resources/Exposed_Secrets_in_Source_Code.md)
- [Mobile App Sensitive Data Leakage (e.g., in logs or backups)](/resources/Mobile_App_Sensitive_Data_Leakage.md)
- [Exposed API Keys or Tokens in Source Code](/resources/Exposed_API_Keys_or_Tokens_in_Source_Code.md)

### 9. Insufficient Logging & Monitoring
- [Lack of Proper Logging](/resources/Lack_of_Proper_Logging.md)
- [Failure to Log Failed Authentication Attempts](/resources/Failure_to_Log_Failed_Authentication_Attempts.md)
- [Absence of Alerts on Suspicious Activities](/resources/Absence_of_Alerts_on_Suspicious_Activities.md)
- [Log Tampering](/resources/Log_Tampering.md)
- [Sensitive Data in Logs](/resources/Sensitive_Data_in_Logs.md)
- [Lack of Audit Trails for Critical Actions](/resources/Lack_of_Audit_Trails_for_Critical_Actions.md)
- [Mobile App Insufficient Logging for Security Events](/resources/Mobile_App_Insufficient_Logging_for_Security_Events.md)
- [API Request/Response Log Tampering](/resources/API_Request-Response_Log_Tampering.md)

### 10. Cross-Origin Resource Sharing (CORS) Issues
- [CORS Misconfiguration](/resources/CORS_Misconfiguration.md)
- [CORS with Open or Misconfigured Origins](/resources/CORS_with_Open_or_Misconfigured_Origins.md)
- [CORS with Insecure Cookies](/resources/CORS_with_Insecure_Cookies.md)
- [CORS with Malicious Request Forging](/resources/CORS_with_Malicious_Request_Forging.md)
- [Insecure CORS Configuration in Mobile Apps with Webviews](/resources/Insecure_CORS_Configuration_in_Mobile_Apps_with_Webviews.md)

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
