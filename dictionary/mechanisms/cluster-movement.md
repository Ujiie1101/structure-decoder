---
type: canonical-cluster
version: v1.0
date: 2026-03-11
cluster_id: CLUSTER-MOVEMENT
domain: history, politics
source: structural-analysis-671-entities
---

# Movement Cluster

## Definition

The **Movement Cluster** characterizes sustained collective action by non-state actors seeking social, political, or cultural change through mobilization rather than armed conflict.

---

## Loop Signature

```
[F-01] Grievance Crystallization
         |
    Shared injustice articulated
         |
[C-02] Mobilization Cascade
         |
    Participation spreads
         |
[MP-01] Reflexive Amplification
         |
    Movement grows through response
         |
[MP-02] Threshold Transition
         |
    Demands become unavoidable
         |
[T-01] Institutional Response
         |
    Reform or co-optation
```

---

## Classification Formula

```
IF (F-01 OR C-02) AND (MP-01 OR MP-02)
   AND domain IN [history, politics]
   AND type = "movement" OR "event"
   AND involves collective mobilization
   AND primarily non-violent
THEN cluster = CLUSTER-MOVEMENT
```

---

## Evidence Proxies (Max 5)

| Proxy | Measurement | Threshold |
|-------|-------------|-----------|
| **Participation** | Active members | >10,000 |
| **Duration** | Sustained activity | >1 year |
| **Organization** | Leadership/structure | Identifiable |
| **Demands** | Articulated goals | Clear |
| **Impact** | Policy/cultural change | Observable |

---

## Registered Members

| Entity | Period | Primary Mechanism | Key Achievement |
|--------|--------|-------------------|-----------------|
| civil-rights-movement | 1954-1968 | C-02 + T-01 | Legal equality |
| arab-spring | 2010-2012 | C-02 + MP-02 | Regional upheaval |
| solidarity-poland | 1980-1989 | F-01 + C-02 | Communist erosion |

---

## Cluster Validation

| Check | Criterion | Status |
|-------|-----------|--------|
| CC-01 | Loop signature documented | PASS |
| CC-02 | Mechanism chain specified | PASS |
| CC-03 | ≤5 evidence proxies | PASS |
| CC-04 | Classification formula provided | PASS |
| CC-05 | ≥3 registered members | PASS |
| CC-06 | All mechanisms use canonical IDs | PASS |

**Overall**: PASS

---

## Cross-Cluster Relationships

| Related Cluster | Relationship |
|-----------------|--------------|
| CLUSTER-REVOLUTION | Movements can escalate to revolution |
| CLUSTER-TRANSFORMATION | Successful movements drive transformation |
| CLUSTER-JUSTICE | Movements demand justice |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-11 | Initial cluster registration |
