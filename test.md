# 1. Pre-Engagement Phase
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


# 2. Information Gathering (Reconnaissance)
### Passive Reconnaissance (No direct interaction)
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
### Active Reconnaissance (Direct interaction with target)
- DNS Enumeration:
  - Query records: `dig example.com ANY`
  - Zone transfer (if misconfigured): `dig axfr @ns1.example.com example.com`
- Port Scanning:
  - Full TCP/UDP scan: `nmap -sS -sU -p- -T4 example.com`
- Web Application Enumeration:
  - Identify directories: `gobuster dir -u https://example.com -w /path/to/wordlist.txt`

# 3. Threat Modeling and Target Prioritization
### Attack Surface Analysis:
- Create a diagram of all services, endpoints, and applications.
- Use tools like OWASP Threat Dragon to visualize threats.
### Prioritization Criteria:
- Business-critical systems: Databases, payment gateways, sensitive APIs.
- Historical vulnerabilities: Legacy software and outdated libraries.

# 4. Vulnerability Assessment
# 5. Exploitation
# 6. Post-Exploitation
# 7. Reporting
### Vulnerability Details:
- Vulnerability name, description, impact, and proof of concept (PoC).
### Screenshots:
- Show exploitation steps for clarity.
### Risk Assessment:
- Use CVSS scores for prioritization.
# 8. Retesting and Improvement
### Validation:
- Confirm fixed vulnerabilities are no longer exploitable.
### Retrospective:
- Document lessons learned and update workflows.


