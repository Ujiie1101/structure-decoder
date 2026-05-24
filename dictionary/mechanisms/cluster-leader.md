---
type: canonical-cluster
version: v1.0
date: 2026-03-11
cluster_id: CLUSTER-LEADER
domain: history, politics
source: structural-analysis-671-entities
---

# Leader Cluster

## Definition

The **Leader Cluster** characterizes transformative historical figures who reshape institutions, nations, or civilizations through personal agency combined with structural opportunity.

---

## Loop Signature

```
[MP-02] Threshold Transition (Crisis/Opportunity)
         |
    Structural opening for leadership
         |
[F-01] Vision Lock-in
         |
    Leader articulates new direction
         |
[C-02] Confidence Contagion
         |
    Followers cascade to new vision
         |
[T-01] Institutional Substitution
         |
    Old order replaced by leader's framework
         |
[F-02] Path Dependency
         |
    Leader's decisions shape long-term trajectory
```

---

## Classification Formula

```
IF (MP-02 OR F-01) AND (C-02 OR T-01)
   AND domain IN [history, politics]
   AND type = "figure"
   AND historical_impact = "transformative"
THEN cluster = CLUSTER-LEADER
```

---

## Evidence Proxies (Max 5)

| Proxy | Measurement | Threshold |
|-------|-------------|-----------|
| **Territorial Change** | Land acquired/unified | Significant |
| **Institutional Creation** | New systems established | ≥1 major |
| **Historical Longevity** | Influence duration | >50 years |
| **Follower Mobilization** | Population engaged | >5% |
| **Paradigm Shift** | New era named after | Binary |

---

## Registered Members

| Entity | Period | Primary Mechanism | Key Achievement |
|--------|--------|-------------------|-----------------|
| napoleon-bonaparte | 1799-1815 | T-01 + V-01 | European transformation |
| alexander-the-great | 336-323 BCE | F-01 + C-02 | Hellenistic world |
| genghis-khan | 1206-1227 | T-01 + V-01 | Mongol Empire |
| julius-caesar | 49-44 BCE | MP-02 + T-01 | Roman transformation |
| abraham-lincoln | 1861-1865 | F-01 + T-01 | Union preservation |
| winston-churchill | 1940-1945 | F-01 + C-02 | WWII leadership |
| mahatma-gandhi | 1915-1948 | C-02 + T-01 | Nonviolent revolution |
| charlemagne | 768-814 | T-01 + F-02 | Medieval Europe |

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
| CLUSTER-REVOLUTION | Leaders emerge from revolutionary contexts |
| CLUSTER-EMPIRE | Leaders build/destroy empires |
| CLUSTER-WAR | Military leaders in conflict |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-11 | Initial cluster registration |
