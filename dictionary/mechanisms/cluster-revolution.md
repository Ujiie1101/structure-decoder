---
type: canonical-cluster
version: v1.0
date: 2026-03-04
cluster_id: CLUSTER-REVOLUTION
domain: politics, history
source: structural-analysis-183-entities
---

# Revolution Cluster

## Definition

The **Revolution Cluster** is a canonical structural cluster characterizing political revolution dynamics. It exhibits a distinct loop signature combining regime erosion, threshold breach, and institutional substitution.

---

## Loop Signature

```
[V-01] Overextension / [V-02] Policy Lock-in
         |
    Regime capacity decline / rigidity
         |
[C-02] Confidence Contagion
         |
    Belief cascade: "if they can resist, so can we"
         |
[MP-02] Threshold Transition
         |
    Regime collapse (coercive capacity exhausted)
         |
[T-01] Institutional Substitution
         |
    New order established (republic, new regime)
         |
[MP-09] Vacuum-Authoritarian Cycle (optional)
         |
    Revolutionary chaos creates centralization demand
```

---

## Typical Mechanism Chain

| Phase | Mechanism | Observable Behavior |
|-------|-----------|---------------------|
| 1. Erosion | V-01/V-02 | Fiscal crisis, legitimacy decline, policy rigidity |
| 2. Mobilization | C-02 | Protest contagion, defection cascades |
| 3. Threshold | MP-02 | Coercive apparatus fails or defects |
| 4. Collapse | C-03 | Old regime disintegrates |
| 5. Substitution | T-01 | New institutions replace old |
| 6. Consolidation | MP-09 | (Optional) Authoritarian rebound |

---

## Classification Formula

```
IF (V-01 OR V-02) AND (C-02 OR C-03) AND (MP-02) AND (T-01)
   AND domain IN [politics, history]
   AND patterns INCLUDE [collapse OR substitution]
THEN cluster = CLUSTER-REVOLUTION
```

---

## Evidence Proxies (Max 5)

| Proxy | Measurement | Threshold |
|-------|-------------|-----------|
| **Coercive Defection** | Military/police refusal rate | >30% |
| **Protest Scale** | Participants as % of population | >1% |
| **Regime Legitimacy** | Public approval collapse | >40pt drop |
| **Elite Defection** | Officials abandoning regime | Key figures |
| **Institutional Replacement** | New constitution/government | Binary |

---

## Registered Members

| Entity | Year | Primary Mechanism | Key Trigger |
|--------|------|-------------------|-------------|
| french-revolution | 1789 | C-03 + T-01 | Fiscal crisis |
| russian-revolution | 1917 | V-01 + C-02 + MP-09 | WWI exhaustion |
| american-revolution | 1776 | V-02 + T-01 | Taxation conflict |
| iranian-revolution | 1979 | V-02 + C-02 | Modernization backlash |
| soviet-collapse | 1991 | V-01 + V-03 + C-02 | Overextension |

---

## Cluster Validation

| Check | Criterion | Status |
|-------|-----------|--------|
| CC-01 | Loop signature documented | PASS |
| CC-02 | Mechanism chain specified | PASS |
| CC-03 | ≤5 evidence proxies | PASS |
| CC-04 | Classification formula provided | PASS |
| CC-05 | ≥5 registered members | PASS |
| CC-06 | All mechanisms use canonical IDs | PASS |

**Overall**: PASS

---

## Cross-Cluster Relationships

| Related Cluster | Relationship |
|-----------------|--------------|
| CLUSTER-CRISIS | Economic crisis can trigger revolution |
| CLUSTER-EMPIRE | Empire decline follows similar erosion pattern |
| CANON-03 | Paradigm transformation shares MP-02, T-02 |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-04 | Initial cluster registration |
