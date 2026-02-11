# NS-L6 Standard — Security Policy

## 1. Scope
This document defines the security disclosure and handling policy for the 
NS-L6 Standard repository.  
It covers vulnerabilities affecting:

- normative correctness,
- boundary integrity (L0–L6),
- provenance or timestamp anchoring,
- compliance statements,
- documentation that affects system safety.

The NS-L6 Standard is a **responsibility framework**, not software; however, 
security-related findings may impact normative correctness.

---

## 2. Reporting a Vulnerability

Please report potential issues via GitHub Issues:

**https://github.com/jan-zdrahal/ns-l6-standard/issues**

Use the label:  
`security`

Include:

- description of the issue  
- affected files / sections  
- reasoning why it constitutes a security, boundary, or normative-risk defect  
- proposed correction (optional)

No private channel is required because the NS-L6 Standard contains no 
confidential code.  
All security-related issues are public and transparent.

---

## 3. Out of Scope

The following are **not** treated as vulnerabilities:

- misunderstandings of the theory  
- content requests  
- AI-generated derivative texts  
- implementation errors in third-party systems  
- disagreements with normative content  
- translation inaccuracies

---

## 4. Security Principles

NS-L6 defines the following mandatory properties:

- **Non-invertibility of layers**  
- **No downward inference**  
- **Local time indices**  
- **Responsibility cannot be projected to L0–L3**  
- **No normative authority for automated systems**  

Any defect violating these principles should be reported immediately.

---

## 5. TSA & Hash Integrity

The provenance hash and TSA anchoring MUST NOT be modified except by custodial 
authority and only during major release processes.

---

## 6. Closing Notes

This repository carries no dangerous code; however, it defines formal 
responsibility structures for AI systems.  
Integrity is therefore essential for safety.

Thank you for supporting the NS-L6 Standard.
