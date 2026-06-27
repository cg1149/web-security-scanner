# Web Security Scanner

A browser-based website security auditing tool that performs real security checks using public APIs and AI-powered analysis.

**[Live Demo →](https://cg1149.github.io/web-security-scanner)**

## Preview

![Web Security Scanner](screenshot.png)

## What it does

Paste any URL and get a full security audit in seconds:

| Check | What's tested |
|---|---|
| HTTP headers | Page source, tech stack fingerprinting, sensitive path detection |
| SSL/TLS | Official grade (A–F) via SSL Labs, cert expiry, HSTS, Forward Secrecy |
| DNS records | SPF, DMARC, IPv6, A/MX records — email spoofing detection |
| robots.txt | Sensitive paths exposed, sitemap declaration |
| CVE lookup | Detects tech stack → queries NIST NVD for known vulnerabilities |
| OWASP Top 10 | Every threat mapped to A01–A10 with official references |
| Security score | Overall 0–100 score with radar chart across 6 categories |
| PDF export | Download full audit as a professional PDF report |

## Tech stack

- Vanilla JS + HTML/CSS — no frameworks, no build step, no install
- Claude API (claude-sonnet-4-6) — AI-powered threat analysis & OWASP mapping
- SSL Labs API — real TLS grading (free, no key)
- NIST NVD API — CVE database (free, no key)
- Google DNS API — SPF/DMARC record lookup (free, no key)
- Chart.js — radar chart for category scores
- jsPDF — client-side PDF report generation

## How to use

1. Visit the [live demo](https://cg1149.github.io/web-security-scanner)
2. Enter your Anthropic API key in the bar at the top
3. Type any URL and click **Full scan**
4. View threats, SSL grade, DNS records, CVEs, and OWASP mapping
5. Download a PDF report

## Run locally

```bash
git clone https://github.com/cg1149/web-security-scanner
cd web-security-scanner
open index.html
```

## Project structure
