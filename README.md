# NS-L6 Standard: Human–LLM Responsibility Framework  
## Version 1.1 — Public Specification

**Status:** Public Release  
**License:**  
- Documentation: CC BY-ND 4.0  
- Tooling: Apache 2.0  
**Brand:** NS-L6 Standard  
**Maintainer:** Jan Zdráhal

---

## 1. Overview

The **NS-L6 Standard** defines a unified, formally structured responsibility architecture for human–LLM systems.  
It introduces a seven-layer model (L0–L6) with strict non-invertibility, formal axioms, normative imperatives,  
and mathematically grounded responsibility boundaries.

This repository contains the full **NS-L6 v1.1 Public Specification**, suitable for regulatory agencies,  
auditors, enterprise AI governance, and safety engineering.

The NS-L6 Standard provides:

- A complete responsibility model  
- A formal layer architecture  
- Normative imperatives  
- Mathematical proofs  
- Formal semantics (BNF/EBNF)  
- Threat model  
- Hybrid licensing model  
- Trademark-protected terminology  
- Auditability requirements  

---

## 2. Repository Structure

```
/
│ README.md
│ LICENSE
│ TRADEMARKS.md
│ NOTICE
│ docs_LICENSE_CC_BY_ND.md
│
├── docs/
│   ├─ NS-L6_Framework_v1.1.md
│   ├─ NS-L6_RFC_v1.1.md
│   ├─ NS-L6_Appendix_A_Formal_Proofs_Public_v1.1.md
│   ├─ NS-L6_Appendix_B_Formal_Semantics_v1.1.md
│   ├─ NS-L6_Appendix_C_Threat_Model_v1.1.md
│
└── meta/
    ├─ NS-L6_BRANDING.md
    ├─ release_notes_v1.1.md
```

The Framework and RFC are normative. Appendix A, Appendix B, and Appendix C are Informative Annex documents.

---

## 3. Licensing Policy (Hybrid Model)

The NS-L6 Standard uses a **two-part hybrid license**:

### 3.1 Documentation License — CC BY-ND 4.0  
The standard documents must **not** be modified or distributed in altered form.  
This preserves the integrity of the normative core.

### 3.2 Tooling License — Apache 2.0  
Used for any code, schemas, validators, or implementations.  
This enables:

- integration in enterprise systems  
- modification  
- redistribution  
- commercial use  

### 3.3 Trademarks  
Protected names include (but are not limited to):

- “NS-L6”
- “NS-L6 Standard”
- “Human–LLM Responsibility Framework”

See `TRADEMARKS.md`.

---

## 4. Relationship to the NS-L6 Manifest

The **NS-L6 Manifest** provides philosophical background and motivation.  
It is **not normative** and must not be interpreted as part of the standard.

The Standard alone defines:

- axioms  
- layer definitions  
- imperatives  
- formal semantics  
- responsibility mapping  
- compliance requirements  

---

## 5. NS-L6 Layer Model (Summary)

The seven-layer architecture:

- **L0 — Physical Layer**  
- **L1 — Computation Layer**  
- **L2 — Model Execution Layer**  
- **L3 — Output Layer**  
- **L4 — System Integration Layer**  
- **L5 — Interaction Layer**  
- **L6 — Normative Layer**

Responsibility exists only at:

- **L5 (human operational responsibility)**  
- **L6 (normative / legal responsibility)**

Lower layers (L0–L4) **cannot** bear responsibility by definition.

---

## 6. Release Notes (v1.1)

This release includes the full NS-L6 Standard:

- Framework  
- RFC  
- Appendix A  
- Appendix B  
- Appendix C  
- Licensing  
- Branding  

Version 1.1 is the first complete public specification.

---

# End of README
