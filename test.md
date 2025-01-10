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
DNS Enumeration:
Query records:
bash
Copy code
dig example.com ANY
Zone transfer (if misconfigured):
bash
Copy code
dig axfr @ns1.example.com example.com
Port Scanning:
Full TCP/UDP scan:
bash
Copy code
nmap -sS -sU -p- -T4 example.com
Web Application Enumeration:
Identify directories:
bash
Copy code
gobuster dir -u https://example.com -w /path/to/wordlist.txt
