# NS-L6 Standard — Canonical Manifest
## Version: v1.1  
**Status:** Normative Provenance Record  
**License:** CC BY-ND 4.0  

This document defines the canonical provenance, cryptographic anchoring,
and archival lineage of the **NS-L6 Standard v1.1**.  
It represents the authoritative manifest for all compliant distributions,
derivative bundles, and reproducible builds.

---

# 1. Canonical Scope (Normative)

This manifest applies to the following normative artifacts:

- `docs/NS-L6_Framework_v1.1.md`
- `docs/NS-L6_RFC_v1.1.md`
- `docs/NS-L6_Appendix_A_Formal_Proofs_Public_v1.1.md`
- `docs/NS-L6_Appendix_B_Formal_Semantics_v1.1.md`
- `docs/NS-L6_Appendix_C_Threat_Model_v1.1.md`
- `meta/NS-L6_BRANDING.md`
- `meta/release_notes_v1.1.md`
- `LICENSE`
- `NOTICE`
- `TRADEMARKS.md`
- This `MANIFEST.md`

The manifest defines the authoritative provenance for **the standard**,  
not for any implementation or external ecosystem.

---

# 2. Canonical Provenance Root (Normative)

## 2.1 Cryptographic Root Hash (SHA3-256)

This is the canonical, immutable hash of the internal archival package
of NS-L6 v1.1, created *before* the public release:  
1580bdbfff85d9c564765c36456b6dbf0bff1435dd4ba16f08d8518ef264543b

This value is the *Provenance Root* and must match:

- the hash published on `ns-l6.org`,
- the TSA-anchored timestamp,
- any derivative distribution archive.

Any deviation invalidates the canonical lineage.

---

## 2.2 TSA Anchoring

The Provenance Root is bound by a third-party  
**Time-Stamping Authority (TSA)**.

The TSA record provides:

- immutable timestamp of authorship priority,  
- anchoring for reproducible builds,  
- legal-grade archival integrity (tamper-evident).

The TSA token is preserved in the internal provenance archive and is **not**
distributed publicly. Only the hash above is normative.

---

# 3. Derivation Tree (Normative)

```
NS-L6 Standard v1.1 (Provenance Root)
│
├── Framework v1.1
│   ├── Axioms A1–A6
│   ├── Normative Imperatives NI-1 … NI-14
│   └── Layer Model L0–L6
│
├── RFC v1.1
│   └── Normative condensation of Framework
│
├── Appendix A — Formal Proofs (Public Extract)
│
├── Appendix B — Formal Semantics (BNF/EBNF)
│
└── Appendix C — Threat Model
```

All downstream artifacts must derive from the Provenance Root  
and preserve the canonical constraints.

No reverse or upward derivation is permitted.

---

# 4. Integrity Invariants (Normative)

The following cryptographic and epistemic invariants define the conditions
for valid canonical distributions:

1. **Invariant I1 — Immutable Hash Root**  
   The SHA3-256 provenance root MUST match exactly.

2. **Invariant I2 — TSA Consistency**  
   The TSA timestamp MUST correspond to the same provenance root.

3. **Invariant I3 — Non-Editable Normative Content**  
   Normative artifacts MUST NOT be modified except by a new version  
   of the standard.

4. **Invariant I4 — Deterministic Packaging**  
   Reproducible builds MUST yield the same root hash.

5. **Invariant I5 — Separation of Normative vs. Informative**  
   Informative files MUST NOT alter the semantics of normative ones.

6. **Invariant I6 — Canonical Lineage Preservation**  
   All published bundles MUST trace lineage to this manifest.

---

# 5. Distribution Requirements (Normative)

Any public or private redistribution of the standard:

- MUST include this canonical manifest,  
- MUST preserve file structure under `/docs` and `/meta`,  
- MUST retain the provenance root unchanged,  
- MAY add non-normative materials as long as they do not alter semantics,  
- MUST NOT imply modifications are canonical.

---

# 6. Release History (Informative)

**v1.1**  
Initial public release of the NS-L6 Responsibility Standard including:

- completed layer model,  
- full axiom set,  
- formal semantics (Appendix B),  
- public proof extract (Appendix A),  
- threat model (Appendix C),  
- branding and governance meta-documents.

Previous internal iterations are archived under the provenance root  
and are not publicly distributed.

---

# 7. End of Manifest
This canonical manifest completes the provenance requirements  
for NS-L6 Standard v1.1.
