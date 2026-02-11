# NS-L6 Standard — Formal Objection Process
## Version: 1.1

This document defines the formal mechanism for submitting objections,
comments, and revision proposals to the NS-L6 Standard.

This process is normative.

---

# 1. Scope

This objection mechanism applies to:

- NS-L6 Framework
- NS-L6 RFC
- Appendix A, B, C
- Canonical MANIFEST and Provenance Root
- Governance and Security processes

Other repositories (e.g., implementations) are out of scope.

---

# 2. What Constitutes a Formal Objection

A Formal Objection is a documented statement asserting that:

- A normative requirement is inconsistent,
- A definition is incomplete or contradictory,
- A security or responsibility issue is present,
- A term or axiom conflicts with observed constraints,
- A revision is required for correctness or integrity.

General feedback is handled through Issues, not objections.

---

# 3. How to Submit an Objection

A Formal Objection MUST be submitted through:

https://github.com/jan-zdrahal/ns-l6-standard/issues

and MUST contain:

1. **Objecting Party** — name or institution  
2. **Document + Section** — precise reference  
3. **Type** — { Normative, Security, Semantic, Logical }  
4. **Argumentation** — technical reasoning  
5. **Proposed Resolution** — optional  
6. **Evidence** — proofs, logs, examples, citations  

Submissions lacking these fields may be rejected.

---

# 4. Review Process

The Custodian of the NS-L6 Standard will:

1. Acknowledge the objection within **7 days**.  
2. Classify severity and scope.  
3. Publish a public resolution within **30 days**, unless complexity requires extension.  
4. If the objection is valid, schedule revision for the next version (v1.2 or later).  

No automated system may issue or resolve objections.

---

# 5. Resolution Outcomes

A resolution may be:

- **Accepted** — incorporated in next normative revision  
- **Accepted with modification**  
- **Deferred** — valid but requires broader architectural changes  
- **Rejected** — with documented reasoning  
- **Out of scope**  

All outcomes are fully documented in the Issue tracker.

---

# 6. Binding Authority

Only the Custodian listed in MANIFEST.md  
holds authority to approve or reject Formal Objections.

No derivative, fork, or external platform has normative authority.

---

# END OF DOCUMENT
