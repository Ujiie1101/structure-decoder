---
type: meta-pattern-registry
version: v1.0
date: 2026-03-05
meta_pattern_count: 13
core_grammar: ['emergence', 'substitution', 'erosion', 'collapse', 'fragmentation', 'inversion']
archetype_ids: ['A01', 'A02', 'A03', 'A04', 'A05', 'A06', 'A07', 'A08']
---

# Meta-Pattern Registry v1.0

Higher-order structural patterns derived from archetype and pattern compositions.

---

## Schema

Each meta-pattern defines:
- **meta_id**: Unique ID (M01-M99)
- **name**: Short kebab-case identifier
- **definition**: 2-4 lines, mechanism-focused
- **composition**: archetypes + pattern_signature
- **decision_rules**: Detection conditions
- **canonical_instances**: Example entities (5-12)
- **cross_domain_candidates**: Expected domains
- **overlaps**: Near-duplicates with rationale

---

## Registry

### M01 | Paradigm Displacement

| Field | Value |
|-------|-------|
| meta_id | M01 |
| name | paradigm-displacement |
| definition | Novel structure emerges and systematically replaces incumbent framework through gradual adoption and eventual institutionalization. |
| composition | archetypes: [A01], signature: {emergence=1, substitution=1} |
| decision_rules | emergence IN patterns AND substitution IN patterns; archetype == A01 |
| canonical_instances | keynesian-economics, classical-economics, shock-therapy, financial-deregulation, ftx-collapse, hayek, rational-expectations, creative-destruction |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M02 | Crisis Driven Transformation

| Field | Value |
|-------|-------|
| meta_id | M02 |
| name | crisis-driven-transformation |
| definition | Systemic crisis forces structural reorganization, replacing failed components with new institutional arrangements. |
| composition | archetypes: [A03, A05], signature: {collapse=1, substitution=1} |
| decision_rules | collapse IN patterns AND substitution IN patterns; archetype IN [A03, A05] |
| canonical_instances | zimbabwe-hyperinflation, enron-scandal, joseph-schumpeter, iranian-revolution, nationalism, crispr, fukushima-disaster, fall-of-berlin-wall |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M03 | Cascade Failure

| Field | Value |
|-------|-------|
| meta_id | M03 |
| name | cascade-failure |
| definition | Localized failure propagates through interconnected systems, triggering widespread collapse without replacement. |
| composition | archetypes: [A08, A02], signature: {collapse=1} |
| decision_rules | collapse IN patterns AND substitution NOT IN patterns; archetype IN [A08, A02] |
| canonical_instances | japan-bubble-burst, black-monday-1987, tulip-mania, minsky-moment, university-rankings-competition, european-debt-crisis, asian-financial-crisis, dot-com-bubble |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M04 | Value Inversion

| Field | Value |
|-------|-------|
| meta_id | M04 |
| name | value-inversion |
| definition | Established value hierarchies or conceptual frameworks reverse without structural collapse, creating new evaluative paradigms. |
| composition | archetypes: [A07], signature: {inversion=1} |
| decision_rules | inversion IN patterns AND collapse NOT IN patterns; archetype == A07 |
| canonical_instances | prospect-theory, david-ricardo, karl-marx, stiglitz, friedrich-hayek, zeno-of-elea, hannah-arendt, edmund-husserl |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M05 | Revolutionary Dissolution

| Field | Value |
|-------|-------|
| meta_id | M05 |
| name | revolutionary-dissolution |
| definition | Unified structure fragments into competing components while hierarchies invert, producing new power configurations. |
| composition | archetypes: [A06], signature: {fragmentation=1, inversion=1} |
| decision_rules | fragmentation IN patterns AND inversion IN patterns; archetype == A06 |
| canonical_instances | immanuel-kant, kant, montesquieu, four-thirty-three |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M06 | Gradual Decay Cycle

| Field | Value |
|-------|-------|
| meta_id | M06 |
| name | gradual-decay-cycle |
| definition | Slow erosion of capacity or legitimacy eventually crosses threshold into systemic collapse. |
| composition | archetypes: [A05], signature: {erosion=1, collapse=1} |
| decision_rules | erosion IN patterns AND collapse IN patterns; archetype == A05 |
| canonical_instances | ltcm-collapse, global-financial-crisis-2008, south-sea-bubble, great-depression-1929, theodor-w-adorno, french-revolution, therac-25, chernobyl-disaster |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M07 | Shock Emergence

| Field | Value |
|-------|-------|
| meta_id | M07 |
| name | shock-emergence |
| definition | Novel structure triggers immediate systemic instability before stabilization or rejection. |
| composition | archetypes: [A02], signature: {emergence=1, collapse=1} |
| decision_rules | emergence IN patterns AND collapse IN patterns; archetype == A02 |
| canonical_instances |  |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M08 | Institutional Lock In

| Field | Value |
|-------|-------|
| meta_id | M08 |
| name | institutional-lock-in |
| definition | Replacement structure becomes embedded as dominant norm, creating path dependency and resistance to change. |
| composition | archetypes: [A04], signature: {substitution=1} |
| decision_rules | substitution IN patterns AND len(patterns) == 1; archetype == A04 |
| canonical_instances | john-maynard-keynes, milton-friedman, daniel-kahneman, amartya-sen, democritus, bertrand-russell, epictetus, diogenes-of-sinope |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M09 | Creative Destruction Cycle

| Field | Value |
|-------|-------|
| meta_id | M09 |
| name | creative-destruction-cycle |
| definition | Continuous cycle where emergence and collapse alternate, driving evolutionary adaptation. |
| composition | archetypes: [A01, A02, A03], signature: {emergence=1, collapse=1, substitution=1} |
| decision_rules | emergence IN patterns AND collapse IN patterns AND substitution IN patterns; archetype IN [A01, A02, A03] |
| canonical_instances |  |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M10 | Fragmentation Without Recovery

| Field | Value |
|-------|-------|
| meta_id | M10 |
| name | fragmentation-without-recovery |
| definition | Structure splinters into components without subsequent reintegration or replacement. |
| composition | archetypes: [A06], signature: {fragmentation=1} |
| decision_rules | fragmentation IN patterns AND substitution NOT IN patterns |
| canonical_instances | anaxagoras, picasso, dharma |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M11 | Emergence Proliferation

| Field | Value |
|-------|-------|
| meta_id | M11 |
| name | emergence-proliferation |
| definition | Novel structures multiply across domains through imitation and adaptation. |
| composition | archetypes: [A01], signature: {emergence=1} |
| decision_rules | emergence IN patterns AND len(patterns) == 1 OR (emergence IN patterns AND substitution NOT IN patterns) |
| canonical_instances | descartes, american-revolution, karma |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M12 | Erosion To Substitution

| Field | Value |
|-------|-------|
| meta_id | M12 |
| name | erosion-to-substitution |
| definition | Gradual decay enables replacement rather than collapse, producing managed transition. |
| composition | archetypes: [A04, A05], signature: {erosion=1, substitution=1} |
| decision_rules | erosion IN patterns AND substitution IN patterns |
| canonical_instances |  |
| cross_domain_candidates | philosophy, economics, politics, history, technology |
| overlaps | — |

---

### M13 | Butterfly Effect

| Field | Value |
|-------|-------|
| meta_id | M13 |
| name | butterfly-effect |
| definition | 微小な初期条件の変化が、増幅・連鎖・閾値超過を経て予測不可能な巨視的結果を創発する。カオス理論における初期条件敏感性（Sensitivity to Initial Conditions）の構造的顕現。 |
| composition | archetypes: [A02, A03, A08], signature: {emergence=1, cascade=1, threshold=1} |
| decision_rules | (cascade IN patterns OR amplification IN patterns) AND (emergence IN patterns) AND (threshold IN patterns OR unintended-consequences IN patterns) |
| canonical_instances | wwi-assassination, 2008-financial-crisis, arab-spring, covid-19, apple-jobs-return, chernobyl-disaster, www-invention |
| cross_domain_candidates | history, economics, politics, technology, science |
| overlaps | M03 (cascade-failure): M03は失敗の連鎖、M13は微小起点からの予測不可能な創発を強調。M06 (gradual-decay-cycle): M06は漸進的侵食、M13は時間遅延を伴う非線形増幅を強調。 |
| unique_elements | 初期微小性, 時間遅延（数日〜数十年）, 分岐点（Bifurcation）, 因果の不可視性 |
| diagnostic_framework | 130_Structure/patterns/butterfly-effect.md |
| prediction_framework | 130_Structure/patterns/butterfly-effect.md |

---

## Summary Table

| ID | Name | Signature | Archetypes | Count |
|----|------|-----------|------------|-------|
| M01 | paradigm-displacement | emergence+substitution | A01 | 106 |
| M02 | crisis-driven-transformation | collapse+substitution | A03,A05 | 11 |
| M03 | cascade-failure | collapse | A08,A02 | 20 |
| M04 | value-inversion | inversion | A07 | 58 |
| M05 | revolutionary-dissolution | fragmentation+inversion | A06 | 4 |
| M06 | gradual-decay-cycle | erosion+collapse | A05 | 11 |
| M07 | shock-emergence | emergence+collapse | A02 | 0 |
| M08 | institutional-lock-in | substitution | A04 | 14 |
| M09 | creative-destruction-cycle | emergence+collapse+substitution | A01,A02,A03 | 0 |
| M10 | fragmentation-without-recovery | fragmentation | A06 | 3 |
| M11 | emergence-proliferation | emergence | A01 | 3 |
| M12 | erosion-to-substitution | erosion+substitution | A04,A05 | 0 |
| M13 | butterfly-effect | emergence+cascade+threshold | A02,A03,A08 | 7 |

---

## Validation Rules

1. `pattern_signature` must use only core grammar: emergence, substitution, erosion, collapse, fragmentation, inversion
2. `archetypes` must use only known IDs: A01, A02, A03, A04, A05, A06, A07, A08
3. Maximum meta-pattern count: 16
4. Minimum canonical instances: 5
5. Coverage target: >= 60%

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-05 | Initial registry; 12 meta-patterns |
