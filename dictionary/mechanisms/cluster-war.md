---
type: canonical-cluster
version: v1.0
date: 2026-03-11
cluster_id: CLUSTER-WAR
domain: history, politics
source: structural-analysis-671-entities
---

# War Cluster

## Definition

The **War Cluster** characterizes armed conflict dynamics across civilizations. It exhibits escalation cascades, resource exhaustion, and post-conflict transformation patterns.

---

## Loop Signature

```
[V-01] Imperial Overextension / [C-02] Alliance Cascade
         |
    Mutual threat perception escalates
         |
[MP-01] Reflexive Spiral
         |
    Arms race / mobilization feedback
         |
[MP-02] Threshold Transition
         |
    War declaration / hostilities begin
         |
[V-01] Resource Exhaustion
         |
    Attrition / collapse of weaker party
         |
[T-01] Institutional Substitution
         |
    Post-war order established
```

---

## Classification Formula

```
IF (V-01 OR C-02) AND (MP-01 OR MP-02)
   AND domain IN [history, politics]
   AND type = "event" OR "conflict"
   AND involves armed hostilities
THEN cluster = CLUSTER-WAR
```

---

## Evidence Proxies (Max 5)

| Proxy | Measurement | Threshold |
|-------|-------------|-----------|
| **Casualty Scale** | Deaths as % of combatants | >5% |
| **Duration** | Conflict length | >1 year |
| **Geographic Scope** | Nations involved | >2 |
| **Resource Mobilization** | GDP % to military | >10% |
| **Institutional Change** | Post-war order shift | Binary |

---

## Registered Members

| Entity | Period | Primary Mechanism | Key Outcome |
|--------|--------|-------------------|-------------|
| crusades | 1095-1291 | C-02 + V-01 | Religious/cultural clash |
| napoleonic-wars | 1803-1815 | V-01 + MP-02 | European order reshaped |
| peloponnesian-war | 431-404 BCE | V-01 + C-02 | Greek hegemony shift |
| vietnam-war | 1955-1975 | V-01 + MP-01 | US credibility crisis |
| korean-war | 1950-1953 | C-02 + MP-02 | Cold War proxy |
| cuban-missile-crisis | 1962 | MP-01 + MP-02 | Nuclear threshold |
| cold-war | 1947-1991 | MP-01 + V-01 | Superpower exhaustion |

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
| CLUSTER-CRISIS | Economic crisis can trigger war |
| CLUSTER-REVOLUTION | War exhaustion triggers revolution |
| CLUSTER-EMPIRE | Imperial expansion drives conflict |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-11 | Initial cluster registration |
