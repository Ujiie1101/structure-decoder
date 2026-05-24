---
type: canonical-cluster
version: v1.0
date: 2026-03-04
cluster_id: CLUSTER-CRISIS
domain: economics
source: structural-analysis-177-entities
---

# Crisis Cascade Cluster

## Definition

The **Crisis Cascade Cluster** is a canonical structural cluster characterizing financial/economic crisis dynamics. It exhibits a distinct loop signature combining reflexive buildup, policy lock-in, and cascade collapse.

---

## Loop Signature

```
[V-02] Policy Lock-in
         ↓
    Orthodoxy prevents adaptive response
         ↓
[MP-01] Reflexive Spiral
         ↓
    Self-reinforcing buildup (leverage, confidence, prices)
         ↓
[Threshold Breach]
         ↓
[C-01] Leverage Cascade  AND/OR  [C-02] Confidence Contagion
         ↓
    Forced liquidation / bank run dynamics
         ↓
[F-03] Debt-Deflation Spiral (optional amplifier)
         ↓
[MP-03] Self-Undermining Success
         ↓
    The very success of the system created its failure conditions
```

---

## Typical Mechanism Chain

| Phase | Mechanism | Observable Behavior |
|-------|-----------|---------------------|
| 1. Stability | V-02 | Policy/model commitment hardens |
| 2. Buildup | MP-01 | Prices → confidence → leverage → prices |
| 3. Peak | MP-02 | Threshold approached (ignored signals) |
| 4. Trigger | C-01/C-02 | Margin call or confidence shock |
| 5. Cascade | F-03 | Asset deflation amplifies debt burden |
| 6. Resolution | T-01 | Institutional substitution (bailout, new regime) |

---

## Evidence Proxies (Max 5)

| Proxy | Measurement | Threshold |
|-------|-------------|-----------|
| **Leverage Ratio** | Debt/Equity across major actors | >3:1 systemic |
| **Volatility Spike** | VIX or equivalent index | >30 sustained |
| **Spread Contagion** | CDS spread correlation across sectors | >0.8 |
| **Liquidity Freeze** | Interbank lending volume decline | >50% drop |
| **Confidence Index** | Consumer/business sentiment | >20pt drop |

---

## Classification Cues

An entity belongs to CLUSTER-CRISIS if:

| Cue | Required | Check |
|-----|----------|-------|
| Contains [C-01] OR [C-02] | YES | Cascade mechanism present |
| Contains [V-02] | YES | Policy lock-in documented |
| Contains [MP-01] OR [MP-03] | YES | Reflexive or self-undermining dynamic |
| Domain = Economics OR History | YES | Appropriate domain |
| Collapse grammar in frontmatter | RECOMMENDED | Structural classification |

**Classification Formula:**
```
IF (C-01 OR C-02) AND V-02 AND (MP-01 OR MP-03)
   AND domain IN [economics, history]
THEN cluster = CLUSTER-CRISIS
```

---

## Registered Members

| Entity | Year | Primary Cascade | Key Lock-in |
|--------|------|-----------------|-------------|
| great-depression-1929 | 1929 | C-01 + C-02 | Gold standard |
| ltcm-collapse | 1998 | C-01 | Model orthodoxy |
| global-financial-crisis-2008 | 2008 | C-01 + C-02 | Rating models |
| european-debt-crisis | 2010 | C-02 | Euro constraints |
| japan-bubble-burst | 1991 | C-01 | Convoy system |
| zimbabwe-hyperinflation | 2008 | C-02 | Political lock-in |
| minsky-moment | (theory) | C-01 | Stability breeds instability |

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

**Overall**: ✅ PASS

---

## Predictive Application

**Early Warning Detection:**

1. Monitor leverage proxy across financial sector
2. Track volatility index trend
3. Identify V-02 indicators (policy rigidity discourse)
4. Watch for MP-01 signals (asset price → confidence feedback)

**If 3+ proxies exceed thresholds:**
- Classify situation as CLUSTER-CRISIS precondition
- Apply crisis response playbook (see `150_Playbook/crisis-response.md` when created)

---

## Cross-Cluster Relationships

| Related Cluster | Relationship |
|-----------------|--------------|
| Empire-Decline | Shares V-01 (overextension); slower dynamics |
| Technology-Disruption | Shares MP-04; constructive vs destructive |
| Paradigm-Shift | Shares MP-02; crisis can trigger paradigm change |
| Butterfly-Effect (M13) | CLUSTER-CRISISはバタフライ効果の経済的顕現。微小な種子（サブプライム延滞等）から閾値超過・連鎖を経て巨視的結果へ。診断・予測フレームワークは `130_Structure/patterns/butterfly-effect.md` |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-04 | Initial crisis cascade cluster registration |
