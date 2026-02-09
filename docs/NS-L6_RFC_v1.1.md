<!-- Licensed under CC BY-ND 4.0 -->
# NS-L6 RFC v1.1 — Strict Final
## Request for Comments — NS-L6-RFC-1.1

**License:** Creative Commons Attribution–NoDerivatives 4.0 International  
**Brand:** NS-L6 Standard  
**Status:** Final – Normative Specification Layer  

---

# Table of Contents
- 1. Abstract
- 2. Status of This Memo
- 3. Terminology
- 4. Normative References
- 5. Informative References
- 6. Introduction
- 7. Architectural Model
- 8. Specification
- 9. Security Considerations
- 10. IANA Considerations
- 11. Appendices (External)
- 12. End of Document

---

# 1. Abstract

This RFC defines the NS-L6 Standard responsibility architecture for human–LLM systems.  
It specifies a non-invertible, seven-layer model establishing responsibility boundaries, axioms, and normative imperatives governing human–LLM interaction systems.  
This document is fully normative except where explicitly declared informative.

---

# 2. Status of This Memo

This document is part of the NS-L6 Standard suite and constitutes the authoritative RFC for version 1.1.  
It is not an IETF publication but follows the RFC formatting conventions for clarity and interoperability.

Distribution of this memo is unlimited.

---

# 3. Terminology (Normative)

All terms are to be interpreted as defined in the NS-L6 Framework v1.1.

Key terms:
- **Actor** — Human or institutional entity capable of responsibility.
- **LLM** — Stateless transformer-based language model.
- **Layer (L0–L6)** — Structural strata of the NS-L6 model.
- **Responsibility** — A property defined by observability and controllability.
- **Axiom** — Formal, non-negotiable rule within the NS-L6 theory.

Terms such as MUST, MUST NOT, REQUIRED, SHALL, SHALL NOT, SHOULD, SHOULD NOT, MAY, and OPTIONAL  
are to be interpreted as specified in RFC 2119.

---

# 4. Normative References

(NR-1) NS-L6 Framework v1.1  
(NR-2) ISO/IEC 42001 Artificial Intelligence Management Systems  
(NR-3) RFC 2119 — Key Words for Use in RFCs to Indicate Requirement Levels  
(NR-4) CC BY-ND 4.0 License Specification  

---

# 5. Informative References

(IR-1) EU AI Act (Final Text)  
(IR-2) NIST AI Risk Management Framework  
(IR-3) OECD AI Principles  

---

# 6. Introduction (Informative)

The NS-L6 Standard establishes a layer-based responsibility system for human–LLM ecosystems.  
The RFC serves as a condensed formalization of the normative requirements from the Framework, suitable for auditors, regulators, and system architects.

---

# 7. Architectural Model (Normative)

NS-L6 specifies the following invariant layers:

- L0 — Physical  
- L1 — Computation  
- L2 — Model  
- L3 — Output  
- L4 — System  
- L5 — Interaction  
- L6 — Normative

Cross-layer inference is prohibited.  
Layers MUST NOT be collapsed or merged in any compliant system.

---

# 8. Specification (Normative)

## 8.1 Axioms

### Axiom A1 — No Downward Inference  
Responsibility MUST NOT be derived from any lower layer state.

### Axiom A2 — Observability  
Actors MUST NOT be held responsible for states they cannot observe.

### Axiom A3 — Controllability  
Actors MUST NOT be held responsible for transitions they cannot control.

### Axiom A4 — LLM Non-Agency  
Models MUST NOT be treated as agents.  
No responsibility SHALL be applied to L0–L3.

### Axiom A5 — Boundary Integrity  
Layer boundaries MUST be preserved.

---

## 8.2 Normative Imperatives (Mandatory)

Systems MUST implement all 14 imperatives defined in the NS-L6 Framework.  
Key requirements include:

- Context integrity  
- Traceability  
- Provenance  
- Configuration accountability  
- Tool isolation  
- Responsibility mapping  
- Transparency  

No deviation is permitted.

---

## 8.3 Responsibility Mapping

Responsibility MUST be assigned only to L5 and L6 entities.  
System-level (L4) responsibility MUST be technical, not normative.  
Model-level (L2) responsibility MUST be zero.

---

# 9. Security Considerations (Normative)

Compliant systems MUST prevent:

- downward inference attacks  
- timestamp manipulation  
- responsibility projection  
- tool-boundary violations  
- normative-bypass attempts  

Security controls MUST align with Appendix C Threat Model.

---

# 10. IANA Considerations

This document requires no IANA actions.

---

# 11. Appendices

Appendix A — Formal Proofs  
Appendix B — Formal Semantics  
Appendix C — Threat Model  

(Appendices are external documents.)

---

# 12. End of Document

