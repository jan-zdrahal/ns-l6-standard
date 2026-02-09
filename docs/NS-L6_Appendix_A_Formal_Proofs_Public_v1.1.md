# NS-L6 Appendix A — Formal Proofs (Public Extract)

## Status
Informative Annex  
(Not Normative)

This appendix provides selected formal definitions and proofs necessary for understanding 
the logical foundations of NS-L6. Full internal derivations are maintained in a private 
research document.

---

# 1. Non-invertibility (Axiom B1)

Let fᵢ : Lᵢ → Lᵢ₊₁ denote the transformation between layers.

Axiom:

    fᵢ is not invertible
    ¬∃ g : Lᵢ₊₁ → Lᵢ

Implication:
Higher layers cannot reconstruct lower-layer states.

---

# 2. Observability and Responsibility

Responsibility requires:

    Obs_H(Lᵢ) ≠ ∅
    Ctrl_H(Lᵢ) ≠ ∅

For layers below L5:

    Obs_H(Lᵢ) = ∅
    Ctrl_H(Lᵢ) = ∅

Thus:

    Resp_H(Lᵢ) = ∅    for i < 5

---

# 3. Minimal Definition of State (Public)

A minimal public definition (subset of internal theory):

    σ : I → S

A state σ is a function of an index I (time, cycle, or step).

This definition is sufficient for understanding:

- layer structure,
- non-invertibility,
- responsibility allocation.

---

END OF PUBLIC APPENDIX A.
