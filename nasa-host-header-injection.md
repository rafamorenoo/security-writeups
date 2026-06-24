# NASA – Host Header Injection Leading to Open Redirect

## 📌 Overview
A Host header injection issue was identified in a web application that resulted in improper handling of redirect logic.

---

## 🔍 Discovery Method
Identified during security testing of web application request handling and validation of HTTP headers.

---

## 🧨 Vulnerability Details
The application processed user-controlled Host headers without proper validation, allowing manipulation of redirect behavior.

---

## ⚠️ Impact
- Open redirect behavior
- Potential phishing exploitation
- Abuse of trusted domain redirection logic

---

## 🧠 Technical Analysis
- OWASP A01: Broken Access Control
- OWASP A03: Injection (context-dependent)

---

## 🛠️ Remediation
- Validate and sanitize Host headers
- Enforce strict redirect allowlists
- Avoid using user-controlled headers in URL generation

---

## 📬 Disclosure
Reported via bug bounty program and acknowledged by the security team.
