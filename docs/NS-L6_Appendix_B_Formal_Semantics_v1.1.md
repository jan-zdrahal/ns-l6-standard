<!-- Licensed under CC BY-ND 4.0 -->
# Appendix B — Formal Semantics (BNF/EBNF)
## NS-L6 Standard v1.1 — Public Specification

**License:** Creative Commons Attribution–NoDerivatives 4.0 International  
**Brand:** NS-L6 Standard  
**Status:** Normative Appendix  

---

# B.1 Purpose (Informative)

This appendix defines the formal semantics of the NS-L6 Standard using  
Extended Backus–Naur Form (EBNF).  
The grammar defines the structure of responsibility assignments,  
layer transitions, state declarations, time indices, and compliance constructs.

---

# B.2 Semantic Domains (Normative)

```
Layer        = L0 | L1 | L2 | L3 | L4 | L5 | L6 ;
State        = identifier ;
TimeIndex    = integer ;
Actor        = identifier ;
ResponsibilitySet = "∅" | "{" ResponsibilityItem ("," ResponsibilityItem)* "}" ;
ResponsibilityItem = identifier ;
```

---

# B.3 Core Grammar Definitions (Normative)

## B.3.1 Responsibility Mapping

```
ResponsibilityMapping =
    "R" "(" Actor "," Layer "," State "," TimeIndex ")" "→" ResponsibilitySet ;
```

Constraints:

- For L0–L3: ResponsibilitySet MUST be ∅.  
- For L4: ResponsibilitySet MAY contain technical responsibilities.  
- For L5–L6: ResponsibilitySet MUST NOT be ∅.

---

## B.3.2 Observability and Controllability Rules

```
Observability  = "Obs"  "(" Actor "," Layer ")" "=" ( "True" | "False" ) ;
Controllability = "Ctrl" "(" Actor "," Layer ")" "=" ( "True" | "False" ) ;
```

Mandatory consistency rule:

```
R(a, i, t) ≠ ∅  ⇔  Obs(a, i) = True AND Ctrl(a, i) = True ;
```

---

## B.3.3 Layer Transition Semantics

```
Transition =
    Layer "." "T" "(" State "," TimeIndex ")" "=" State ;
```

Constraints:

- Transition functions MUST be non-invertible for all i < j.
- Bidirectional transitions MUST NOT exist.

---

## B.3.4 State Declarations

```
StateDeclaration =
    Layer "." "State" "(" TimeIndex ")" "=" State ;
```

---

## B.3.5 Imperative Compliance Syntax

```
ComplianceCheck =
    "CHECK" ImperativeName ":" ( "PASS" | "FAIL" ) ;
```

Where ImperativeName ∈ { NI-1, NI-2, ..., NI-14 }.

Compliance requirements:

- All NI-* MUST be PASS for NS-L6 compliance.

---

# B.4 Meta-Constraints (Normative)

## B.4.1 Non-Invertibility

```
NonInvertible =
    "NONINV" "(" Layer "," Layer ")" "=" "True" ;
```

Required for all (i, j) such that i < j.

---

## B.4.2 Time Locality

```
TimeLocality =
    Layer "." "Time" "=" "LocalIndex" ;
```

No global time index is permitted.

---

# B.5 Extended Grammar (Informative)

## B.5.1 Responsibility Logic Expressions

```
LogicExpr =
      "NOT" LogicExpr
    | LogicExpr "AND" LogicExpr
    | LogicExpr "OR"  LogicExpr
    | "(" LogicExpr ")"
    | Predicate ;

Predicate =
      Observability
    | Controllability
    | ResponsibilityMapping ;
```

---

# B.6 Validation Rules (Normative)

A system is semantically valid if:

1. All syntactic rules in B.2–B.5 are satisfied.  
2. No ResponsibilityMapping violates invariants.  
3. NonInvertible(i, j) = True holds for all i < j.  
4. All NI-* rules evaluate to PASS.  

---

# B.7 End of Appendix B
