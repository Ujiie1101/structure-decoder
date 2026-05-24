---
type: archetype-registry
version: v1.0
date: 2026-03-05
archetype_count: 8
core_grammar: [emergence, substitution, erosion, collapse, fragmentation, inversion]
spec: 040_OS/structural-archetype-engine.md
output: 135_Meta/archetype-report.json
---

# Archetype Registry v1.0

Canonical registry of structural archetypes for Knowledge OS.

---

## Schema

Each archetype defines:
- **archetype_id**: Unique ID (A01-A99)
- **name**: Short identifier
- **definition**: Mechanism-focused description
- **signature_patterns**: Required grammar types from entity `patterns[]`
- **decision_rules**: Scoring conditions for assignment
- **first_instances**: Known entities that exemplify this archetype
- **cross_domain_candidates**: Domains where this archetype is expected

---

## Registry

### A01 | Innovation Displacement

| Field | Value |
|-------|-------|
| archetype_id | A01 |
| name | innovation-displacement |
| definition | Novel structure emerges and replaces incumbent framework through gradual adoption |
| signature_patterns | `[emergence, substitution]` |
| decision_rules | `emergence IN patterns AND substitution IN patterns` → score 1.0; `emergence IN patterns AND len(patterns)==1` → score 0.6 |
| first_instances | thales, anaximander, tcp-ip, printing-press, transistor |
| cross_domain_candidates | philosophy, technology, economics |
| overlay_affinity | CANON-01, CANON-04, STACK-01 |

---

### A02 | System Shock

| Field | Value |
|-------|-------|
| archetype_id | A02 |
| name | system-shock |
| definition | Novel structure triggers systemic instability before stabilization |
| signature_patterns | `[emergence, collapse]` |
| decision_rules | `emergence IN patterns AND collapse IN patterns` → score 1.0; `emergence IN patterns AND CLUSTER-CRISIS IN overlays` → score 0.8 |
| first_instances | dot-com-bubble, ltcm-collapse |
| cross_domain_candidates | economics, technology, politics |
| overlay_affinity | CLUSTER-CRISIS, STACK-02 |

---

### A03 | Crisis Reordering

| Field | Value |
|-------|-------|
| archetype_id | A03 |
| name | crisis-reordering |
| definition | System crisis enables new institutional order through forced restructuring |
| signature_patterns | `[collapse, substitution]` |
| decision_rules | `collapse IN patterns AND substitution IN patterns` → score 1.0; `collapse IN patterns AND CLUSTER-REVOLUTION IN overlays` → score 0.8 |
| first_instances | french-revolution, russian-revolution, bretton-woods |
| cross_domain_candidates | history, politics, economics |
| overlay_affinity | CLUSTER-CRISIS, CLUSTER-REVOLUTION, CANON-02 |

---

### A04 | Paradigm Lock

| Field | Value |
|-------|-------|
| archetype_id | A04 |
| name | paradigm-lock |
| definition | Replacement structure becomes embedded as dominant norm, resisting further change |
| signature_patterns | `[substitution]` |
| decision_rules | `substitution IN patterns AND len(patterns)==1` → score 0.9; `substitution IN patterns AND CANON-03 IN overlays` → score 0.8 |
| first_instances | john-maynard-keynes, adam-smith, john-locke |
| cross_domain_candidates | economics, politics, philosophy |
| overlay_affinity | STACK-01, CANON-01, CANON-03 |

---

### A05 | Terminal Decline

| Field | Value |
|-------|-------|
| archetype_id | A05 |
| name | terminal-decline |
| definition | Gradual decay culminates in systemic failure without recovery |
| signature_patterns | `[erosion, collapse]` |
| decision_rules | `erosion IN patterns AND collapse IN patterns` → score 1.0; `erosion IN patterns AND CLUSTER-EMPIRE IN overlays` → score 0.8 |
| first_instances | fall-of-roman-empire, fall-of-constantinople, soviet-collapse |
| cross_domain_candidates | history, politics |
| overlay_affinity | CANON-05, CLUSTER-EMPIRE |

---

### A06 | Revolutionary Dissolution

| Field | Value |
|-------|-------|
| archetype_id | A06 |
| name | revolutionary-dissolution |
| definition | Unity fragments and hierarchy inverts through disruptive reconfiguration |
| signature_patterns | `[fragmentation, inversion]` |
| decision_rules | `fragmentation IN patterns AND inversion IN patterns` → score 1.0; `inversion IN patterns AND CLUSTER-REVOLUTION IN overlays` → score 0.7 |
| first_instances | french-revolution, cultural-revolution |
| cross_domain_candidates | history, politics |
| overlay_affinity | CLUSTER-REVOLUTION, CLUSTER-EMPIRE |

---

### A07 | Conceptual Inversion

| Field | Value |
|-------|-------|
| archetype_id | A07 |
| name | conceptual-inversion |
| definition | Value hierarchy or established framework reverses without structural collapse |
| signature_patterns | `[inversion]` |
| decision_rules | `inversion IN patterns AND collapse NOT IN patterns` → score 0.9; `inversion IN patterns AND emergence IN patterns` → score 0.8 |
| first_instances | friedrich-nietzsche, jean-jacques-rousseau, arthur-schopenhauer |
| cross_domain_candidates | philosophy, economics |
| overlay_affinity | none |

---

### A08 | Cascade Collapse

| Field | Value |
|-------|-------|
| archetype_id | A08 |
| name | cascade-collapse |
| definition | Single-mode systemic failure without preceding erosion or following substitution |
| signature_patterns | `[collapse]` |
| decision_rules | `collapse IN patterns AND len(patterns)==1` → score 1.0; `collapse IN patterns AND CLUSTER-CRISIS IN overlays` → score 0.9 |
| first_instances | black-monday-1987, japan-bubble-burst, asian-financial-crisis |
| cross_domain_candidates | economics |
| overlay_affinity | STACK-02, CLUSTER-CRISIS |

---

## Summary Table

| ID | Name | Signature | Primary Domain |
|----|------|-----------|----------------|
| A01 | innovation-displacement | emergence+substitution | philosophy, technology |
| A02 | system-shock | emergence+collapse | economics, technology |
| A03 | crisis-reordering | collapse+substitution | history, politics |
| A04 | paradigm-lock | substitution | economics, philosophy |
| A05 | terminal-decline | erosion+collapse | history |
| A06 | revolutionary-dissolution | fragmentation+inversion | politics |
| A07 | conceptual-inversion | inversion | philosophy |
| A08 | cascade-collapse | collapse | economics |

---

## Validation Rules

1. `signature_patterns` must contain only core grammar (6 types)
2. `archetype_id` must be unique (A01-A99)
3. `decision_rules` must be deterministic and computable
4. `first_instances` must reference entities in structure-index.json
5. Score thresholds: ≥0.75 auto-assign, 0.50-0.74 review, <0.50 reject

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-05 | Complete registry; 8 archetypes; decision_rules added |
| v0.1 | 2026-03-05 | Initial draft; 6 archetypes |
