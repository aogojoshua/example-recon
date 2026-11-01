# Reconnaissance & Vulnerability Assessment: example.com

## Project Objective
This repository contains the findings of a comprehensive passive and active reconnaissance engagement conducted against `example.com`. The primary objective is to map the target's external attack surface, enumerate public-facing infrastructure, and provide actionable security-hardening recommendations.

## Tools & Methodology
The assessment was executed from a Kali Linux environment, utilizing the following intelligence-gathering utilities:
* **Passive Reconnaissance:** `whois`, `theHarvester`, and DNS Enumeration (nslookup) to gather administrative metadata, DNS architecture, and exposed corporate emails without alerting the target.
* **Active Reconnaissance:** `nmap` and `whatweb` to transmit direct network probes, identify live hosts, footprint running web technologies, and uncover exposed TCP services.

## Repository Structure
* **Raw Tool Outputs:**
  * `/DNS Enumeration (nslookup)` - Authoritative nameserver and DNS record resolutions.
  * `/Domain Registration and Information` - WHOIS registry data and domain status locks.
  * `/Emails and Subdomains` - OSINT harvesting results from search engines and certificate logs.
  * `/nmap` - Active port scanning, service versioning, and host discovery logs.
  * `/Web Identification/whatweb` - Web server fingerprinting and HTTP header analysis.
* **Project Deliverables:**
  * `Capstone FInal.pdf` - The master report containing the discovered asset table and aggregated findings.
  * `Active v Passive.pdf` - An analytical comparison of non-intrusive versus direct scanning methodologies.
  * `Attack-surface map.jpeg` - A visual network topology diagram mapping the attacker's view of the Cloudflare edge proxy and exposed ports.
  * `Remediation and Security Hardening .pdf` - An executive checklist addressing unencrypted services and security misconfigurations.

## Disclaimer
This project was conducted strictly for educational purposes, academic evaluation, and professional development. All active scanning was constrained to the designated target scope.
