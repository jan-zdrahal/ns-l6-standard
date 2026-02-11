# NS-L6 Standard — Governance Policy

## 1. Purpose
This document defines the governance model for the NS-L6 Standard.  
It ensures deterministic evolution, custodial oversight, and provenance integrity.

---

## 2. Governance Model

NS-L6 uses a **custodial governance model**, not a community or multi-stakeholder model.

**Custodian:**  
**Jan Zdráhal** — the sole authority responsible for:

- maintaining normative documents,
- issuing new versions,
- approving or rejecting proposals,
- preserving provenance, hash lineage, and TSA anchoring.

No other entity may publish normative updates.

---

## 3. What Governance Covers

This policy controls:

- versioning  
- publication of new releases  
- acceptance or rejection of proposals  
- amendment of normative content  
- appendices restructuring  
- release notes  
- canonical repo structure  
- hash & TSA updates (major versions only)  

---

## 4. Versioning Process

### Minor or Patch Release (e.g., 1.1 → 1.2 or 1.1.0 → 1.1.1)

Permitted when:

- clarifying language  
- adding non-normative explanation  
- correcting typographical issues  
- updating appendices without changing core model  

Requires:

- updated VERSION file  
- updated release notes  
- updated MANIFEST if provenance boundary changes  

### Major Release (e.g., 1.x → 2.x)

Requires:

- formal custodial decision  
- updated provenance root  
- new TSA anchoring  
- regenerated MANIFEST  
- public announcement  

Major releases redefine conceptual scope or introduce new invariants.

---

## 5. Proposal Intake

Anyone may open Issues, but:

- proposals are advisory  
- custodian is the only decision-maker  
- PRs are not accepted  

---

## 6. Non-Changeable Foundations

The following are permanently fixed unless superseded by a major 
custodial redesign:

- Axioms A1–A6  
- Responsibility invariants (R1, R2 + joint principle)  
- Seven-layer model (L0–L6)  
- Non-invertibility  
- Local time indices  
- Non-agency of LLMs  
- Responsibility mapping rules  
- NI-1 … NI-14  

---

## 7. Release Announcement Rules

Each release MUST include:

- updated HTML publication  
- updated canonical spec in `/docs`  
- updated release notes  
- updated MANIFEST (only if provenance boundary changes)

---

## 8. End of Governance Policy
