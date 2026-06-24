# 🧠 Security Writeups

## Security Research | Bug Bounty | Web & API Security | Attack Surface Analysis

This repository contains structured and sanitized writeups from real-world security research conducted in bug bounty programs and independent security analysis.

The goal of this repository is to demonstrate practical offensive security skills, methodology, and vulnerability understanding without exposing sensitive or exploitable details.

---

## 👋 About Me

I am a Security Researcher focused on identifying and analyzing real-world vulnerabilities in web applications, APIs, and cloud-based systems.

I actively participate in bug bounty programs (HackerOne, Bugcrowd, and private programs), where I perform security testing on production systems under responsible disclosure policies.

My work focuses on:
- Web application security (OWASP Top 10)
- API security & Broken Access Control
- Attack surface discovery & reconnaissance automation
- Security tooling and scripting (Python, Bash)
- Cloud security fundamentals (AWS environments)

---

## 🐞 Real-World Security Research

The following are high-level summaries of validated security findings:

### 🔓 Vodafone DE — Exposed Internal System (Access Control Issue)
- Discovered an exposed internal administrative panel without authentication
- Identified through external attack surface reconnaissance
- Impact: Unauthorized access to internal automation interface
- Reported via HackerOne program

---

### 🌐 NASA — Host Header Injection → Open Redirect
- Identified insecure usage of Host header in URL generation logic
- Exploitable for external redirection manipulation
- Impact: Open redirect behavior affecting trusted NASA subdomain
- Reported through Bugcrowd program

---

### 🔐 DeFi Protocol — Liquidation Logic Vulnerability
- Identified critical flaw in liquidation cooldown mechanism
- Edge case allowed state reset without asset transfer
- Impact: Blocking of liquidation process in undercollateralized positions
- Found through manual smart contract analysis and invariant testing

---

## 🧠 Methodology

My typical security research workflow:

### 1. Attack Surface Enumeration
- Subdomain discovery
- Asset mapping
- Endpoint identification

### 2. Reconnaissance & Analysis
- Technology fingerprinting
- Exposure validation
- Input surface identification

### 3. Manual Security Testing
- Authentication & authorization testing
- API request manipulation
- Business logic validation

### 4. Exploitation Validation (Controlled)
- Proof-of-concept verification
- Impact assessment
- Responsible disclosure preparation

---

## 🛠️ Tools & Technologies

### Recon & Security Testing
- Burp Suite Professional
- Subfinder
- Httpx
- Katana
- LinkFinder

### Development & Automation
- Python
- Bash
- Java (Spring Boot)
- REST APIs

### Cloud & Infrastructure
- AWS (EC2, S3, ECS, IAM)
- Docker
- Terraform

---

## 📁 Repository Structure


security-writeups/
│
├── vodafone-exposed-panel.md
├── nasa-host-header-injection.md
├── defi-liquidation-bypass.md
├── methodology.md
└── README.md


Each writeup follows a structured, sanitized format focused on:
- Technical understanding
- Security impact
- Methodology
- No sensitive or weaponizable details

---

## ⚠️ Disclaimer

All content in this repository is for **educational and portfolio purposes only**.

- No exploits or weaponizable payloads are included
- No sensitive information is disclosed
- All findings were responsibly reported through official bug bounty programs

---

## 🎯 Goals

This repository is part of my professional security portfolio and is intended to demonstrate readiness for roles such as:

- Junior Application Security Engineer
- Penetration Tester (Web / API)
- Security Researcher / Bug Bounty Hunter
- Cloud Security Engineer (AWS-focused roles)

---

## 🔗 Links

- 🌐 Portfolio: https://rafa-moreno.vercel.app
- 💼 LinkedIn: https://www.linkedin.com/in/rafa-moreno-5b44b4307
- 💻 GitHub: https://github.com/rafamorenoo

---

## 🚀 Status

Continuously improving security research skills through:
- Bug bounty programs
- Offensive security labs
- Real-world vulnerability research
- Cloud security exploration
