<!-- Licensed under CC BY-ND 4.0 -->
# NS-L6 Standard: Human–LLM Responsibility Framework  
## Version 1.1 — Public Specification

**License:** Creative Commons Attribution–NoDerivatives 4.0 International  
**Brand:** NS-L6 Standard  
**Status:** Public Specification Release  

---

# 1. Purpose and Scope (Normative)

The NS-L6 Standard defines a unified, formal, layer-based responsibility model for human–LLM interaction systems.  
This specification establishes a normative reference for responsibility assignment, system boundaries, and governance processes across layered socio-technical architectures.

This document is the sole authoritative specification of the NS-L6 Responsibility Model.

---

# 2. Terminology (Normative)

- **LLM** — Large Language Model without internal persistent state or agency.  
- **Actor** — A human or institutional decision-maker interacting with a system.  
- **Layer (L0–L6)** — A structural component of the responsibility model.  
- **State** — The complete configuration of all relevant variables at a given time.  
- **Time Index** — The ordered sequence of transitions at any layer.  
- **Responsibility** — A property emerging only where controllability and observability jointly hold.  
- **Axiom** — A formally defined, non-negotiable statement within the NS-L6 theory.  
- **Normative Imperative** — A requirement that must be followed for compliant systems.

---

# 3. Architectural Overview (Normative)

NS-L6 defines seven invariant system layers:

- **L0 – Physical Layer**  
- **L1 – Computation Layer**  
- **L2 – Model Execution Layer**  
- **L3 – Model Output Layer**  
- **L4 – System Integration Layer**  
- **L5 – Interaction Layer**  
- **L6 – Normative Responsibility Layer**

Each layer has:
- layer-specific state variables  
- its own time index  
- transition rules  
- invariants prohibiting reverse inference  
- a defined responsibility envelope  

Cross-layer interactions are strictly non-invertible.

---

# 4. State Taxonomy (Normative)

States are categorized as follows:

1. **Physical State (L0)** — electrical, quantum, hardware-level configuration.  
2. **Computational State (L1)** — machine instructions, memory representations.  
3. **Model State (L2)** — transient activation and token-level transitions.  
4. **Output State (L3)** — probability distributions, decoded text.  
5. **System State (L4)** — orchestration, routing, tools, interfaces.  
6. **Interaction State (L5)** — human interaction context.  
7. **Normative State (L6)** — responsibility and decision structures.

State transitions follow layer-specific rules and cannot be meaningfully projected downward or inferred upward.

---

# 5. Time Taxonomy (Normative)

Time is defined per-layer:

- **L0 Time** — physical propagation and clock drift.  
- **L1 Time** — instruction cycle and computational clocks.  
- **L2 Time** — model-internal token transition time.  
- **L3 Time** — output emission sequence.  
- **L4 Time** — system orchestration timeline.  
- **L5 Time** — interaction cycles.  
- **L6 Time** — decision time and audit time.

There is **no single universal time**, only layer-local time indices.

---

# 6. Layered Responsibility Model (Normative)

Responsibility is assigned according to two global invariants:

### **Invariant R1 — Observability**
Actor cannot be responsible for any layer whose state is not observable.

### **Invariant R2 — Controllability**
Actor cannot be responsible for any layer whose transitions they cannot control.

### **Joint Necessity Principle**
Responsibility exists **only when both observability and controllability are present**.

Application:

- L0–L3 → No human responsibility.  
- L4 → System engineering responsibility.  
- L5 → Human operational responsibility.  
- L6 → Legal, institutional, and normative responsibility.

---

# 7. Axiom Set — Responsibility Boundary (Normative)

**Axiom A1 — No Downward Inference**  
Responsibility cannot be assigned based on any lower-layer state.

**Axiom A2 — No Hidden Responsibility**  
Layers invisible to the actor cannot carry responsibility.

**Axiom A3 — Tool-Responsibility Separation**  
Tools cannot hold responsibility; only actors do.

**Axiom A4 — Frozen Model Constraint**  
Model internals (L2) are not modifiable at runtime; no responsibility attaches.

**Axiom A5 — Non-Agency of LLMs**  
LLMs lack persistent internal state and therefore cannot hold responsibility.

**Axiom A6 — Boundary Completeness**  
Responsibility must map to the highest applicable layer consistent with invariants.

---

# 8. Normative Imperatives (Normative)

1. **NI-1 — Context Integrity**  
2. **NI-2 — Decision Traceability**  
3. **NI-3 — Input Provenance**  
4. **NI-4 — Configuration Accountability**  
5. **NI-5 — Tool Boundary Integrity**  
6. **NI-6 — Disclosure of System Capabilities**  
7. **NI-7 — Human Oversight**  
8. **NI-8 — Causality Preservation**  
9. **NI-9 — No Responsibility Projection**  
10. **NI-10 — Layer-Consistent Logging**  
11. **NI-11 — Normative Auditability**  
12. **NI-12 — Hazard Mitigation**  
13. **NI-13 — Non-Delegability of L6 Responsibility**  
14. **NI-14 — Normative Transparency**

All imperatives are mandatory for NS-L6 compliance.

---

# 9. Formal Responsibility Mapping (Normative)

Responsibility assignment is a function:

```
R : (Actor, Layer, State, Time) → ResponsibilitySet
```

with constraints:

- R = ∅ for layers L0–L3  
- R = Limited for L4  
- R = Full operational for L5  
- R = Normative/legal for L6  

No responsibility may be inferred across layer boundaries.

---

# 10. Compliance Requirements (Normative)

A system is NS-L6 compliant if:

1. No responsibility is assigned contrary to invariants.  
2. All normative imperatives are enforced.  
3. Layer boundaries are preserved.  
4. Audit traces contain L4–L6 visibility.  
5. No downward inference is used for accountability.  
6. Tooling is isolated from responsibility-bearing layers.  

---

# 11. Non-Normative Notes (Informative)

This section provides optional clarifications and examples.

- NS-L6 does not assert or assume LLM agency.  
- NS-L6 does not mandate a specific architecture.  
- NS-L6 does not modify legal frameworks, but structures their application.  

---

# 12. Versioning Rules (Normative)

Version numbers follow the structure:

```
Major.Minor.Patch
```

v1.1 introduces:

- formal semantics  
- responsibility invariants  
- unified architecture  
- normative imperatives  
- compliance rules  

---

# 13. References

Normative and informative references will be added after appendices are finalized.

---

# 14. Appendix References

Appendix A — Formal Proofs  
Appendix B — Formal Semantics  
Appendix C — Threat Model  

(This document does not embed appendices.)

---

# END OF SPECIFICATION
