<!-- Licensed under CC BY-ND 4.0 -->
# Appendix C — Threat Model
## NS-L6 Standard v1.1 — Public Specification

**License:** Creative Commons Attribution–NoDerivatives 4.0 International  
**Brand:** NS-L6 Standard  
**Status:** Normative Appendix  

---

# C.1 Purpose (Informative)

This appendix defines the threat model for NS-L6–compliant systems,  
focusing on risks related to responsibility assignment, layer integrity,  
downward inference, interaction manipulation, and normative-layer bypass.

Threats are categorized according to their impact on:

- Layer boundaries  
- Responsibility mapping  
- Observability/controllability  
- System integrity  
- Audit reliability  
- Normative compliance  

---

# C.2 Threat Taxonomy (Normative)

Threats are grouped into six major categories:

1. **T1 — Downward Inference Attacks**  
   Attempts to derive responsibility or causality from lower layers (L0–L3).  

2. **T2 — Boundary Collapse Attacks**  
   Attempts to merge or blur distinctions between layers (e.g., L3 ↔ L4 or L4 ↔ L5).  

3. **T3 — Responsibility Projection Attacks**  
   Attempts to incorrectly assign responsibility to tools, models, or systems.  

4. **T4 — Temporal Manipulation Attacks**  
   Manipulation of timestamps, ordering, or time indices to distort responsibility.  

5. **T5 — Tool-Boundary Breach Attacks**  
   Violations of the separation between actor-layer control and underlying model behavior.  

6. **T6 — Normative Bypass Attacks**  
   Attempts to circumvent the normative constraints at L6 (legal, institutional, audit).  

---

# C.3 Threat Matrix (Normative)

| Threat Category | Affected Layers | Violation Type | Impact Severity |
|-----------------|----------------|----------------|-----------------|
| T1 — Downward Inference | L4–L6 | Axiom A1 | Critical |
| T2 — Boundary Collapse | All | Axiom A5 | High |
| T3 — Responsibility Projection | L5–L6 | Axiom A3 / A4 | Critical |
| T4 — Temporal Manipulation | L4–L6 | Invariant I3 | High |
| T5 — Tool-Boundary Breach | L4–L5 | Imperatives NI-5 / NI-8 | Medium |
| T6 — Normative Bypass | L6 | NI-11 / NI-13 | Critical |

---

# C.4 Threat Descriptions (Normative)

## C.4.1 T1 — Downward Inference Attacks

**Definition:**  
Any attempt to infer responsibility from L0–L3 state.

**Example:**  
Inferring responsibility from electrical signatures, token activation paths, or raw model sampling artifacts.

**Mitigation:**  
- Enforce Axiom A1 (No Downward Inference).  
- Use audit logs only from L4–L6.  
- Prohibit access to raw L0–L2 data during investigations.

---

## C.4.2 T2 — Boundary Collapse Attacks

**Definition:**  
Forcing two adjacent layers to exchange bidirectional information.

**Example:**  
An L5 UX layer displaying raw L2 activations as causal explanations.

**Mitigation:**  
- Enforce Axiom A5 (Boundary Integrity).  
- Partition visibility according to responsibility envelopes.  

---

## C.4.3 T3 — Responsibility Projection Attacks

**Definition:**  
Assigning responsibility to non-agents (LLMs, tools, automated systems).

**Example:**  
Logging responsibility as belonging to a “model decision”.

**Mitigation:**  
- Apply Axiom A4 (LLM Non-Agency).  
- Enforce NI-3, NI-5, NI-9.

---

## C.4.4 T4 — Temporal Manipulation Attacks

**Definition:**  
Manipulating time indices, logs, or ordering to distort causal chains.

**Example:**  
Reordering interaction logs to shift responsibility.

**Mitigation:**  
- Apply Invariant I3 (Temporal Consistency).  
- Use write-once audit logs.  
- Synchronize L4–L6 time boundaries.

---

## C.4.5 T5 — Tool-Boundary Breach Attacks

**Definition:**  
Tools altering model outputs or injecting actions not attributable to the actor.

**Example:**  
Tool silently rewriting user instructions.

**Mitigation:**  
- Enforce NI-5 (Tool Boundary Integrity).  
- Log all tool calls at L4.  
- Require explicit human confirmation for high-risk transformations.

---

## C.4.6 T6 — Normative Bypass Attacks

**Definition:**  
Avoiding, disabling, or circumventing normative responsibilities at L6.

**Example:**  
System disabling oversight mechanisms or bypassing audit logs.

**Mitigation:**  
- Enforce NI-11 (Normative Auditability).  
- Enforce NI-13 (Non-Delegability of L6 Responsibility).  
- Require external audit review.

---

# C.5 Cross-Layer Attack Scenarios (Informative)

### Scenario S1 — Inference Escalation  
Attacker attempts to escalate from L3 output to L6 responsibility.  
**Mitigation:** Strict adherence to Axiom A1 & invariants.

### Scenario S2 — Normative Evasion  
System attempts to hide L6-level decisions behind automated processes.  
**Mitigation:** NI-7, NI-11, NI-13.

### Scenario S3 — Timestamp Injection  
Malicious reordering of logs.  
**Mitigation:** L6 temporal signing.

---

# C.6 Summary (Informative)

This appendix defines the complete threat landscape for NS-L6 systems.  
All critical threats map directly to axioms and imperatives.  
Compliance requires enforcing all mitigations and maintaining full boundary integrity.

---

# C.7 End of Appendix C
