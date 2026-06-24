# Host Header Injection Leading to Open Redirect Behavior

## Overview

A Host header manipulation issue was identified in a web application, where user-controlled input influenced URL generation logic.

This resulted in an open redirect behavior affecting trusted application flows.

---

## 🧠 Attack Surface Discovery

During testing of application routing and request handling, it was observed that the system dynamically constructed URLs using request metadata.

This indicated a potential trust boundary issue between:

- user-controlled headers
- server-side URL generation logic

---

## ⚙️ Root Cause

The vulnerability was caused by:

- unsafe usage of Host header in application logic
- lack of validation of trusted origin
- dynamic URL construction based on untrusted input

This leads to **trust boundary violation in request processing**.

---

## 💥 Security Impact

This issue can lead to:

- open redirect behavior
- phishing vector amplification
- bypass of trusted domain assumptions
- manipulation of user navigation flows

In some cases, it can be chained with authentication flows.

---

## 🧠 Why This Happens

This is commonly caused by:

- incorrect assumptions about HTTP headers
- missing validation of origin metadata
- insecure URL construction patterns

---

## 🛡️ Mitigation

- validate Host header against allowlist
- avoid using headers for security decisions
- implement strict URL generation rules
- enforce canonical domain configuration

---

## 🔗 Classification

- OWASP: A01 Injection
- CWE: CWE-20 Improper Input Validation
