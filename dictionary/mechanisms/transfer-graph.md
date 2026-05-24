---
type: transfer-graph
version: v1.0
date: 2026-03-04
node_count: 7
edge_count: 12
source: structural-analysis-177-entities
---

# Cross-Domain Transfer Graph

## Graph Structure

```
                    Philosophy
                   /    |    \
                  3     2     2
                 /      |      \
         Economics ←—3—→ Technology
                \      /
                 2    2
                  \  /
                 Politics
                    |
                    2
                    |
                 History
                   / \
                  1   1
                 /     \
            Religion   Art
```

**Edge weights**: Transfer strength (0–3 scale)

---

## Transfer Strength Scoring Rubric

| Score | Label | Criteria |
|-------|-------|----------|
| **3** | STRONG | ≥10 shared mechanism patterns; direct conceptual bridge; bidirectional transfer documented |
| **2** | MODERATE | 5–9 shared patterns; indirect bridge via mediating domain; unidirectional transfer common |
| **1** | WEAK | 2–4 shared patterns; metaphorical transfer only; requires explicit justification |
| **0** | NONE | <2 shared patterns; no documented transfer |

---

## Transfer Matrix

| From \ To | Phil | Hist | Rel | Econ | Pol | Tech | Art |
|-----------|------|------|-----|------|-----|------|-----|
| **Philosophy** | — | 2 | 2 | **3** | 2 | **3** | 2 |
| **History** | 2 | — | 1 | 2 | 2 | 1 | 1 |
| **Religion** | 2 | 1 | — | 1 | 1 | 1 | 1 |
| **Economics** | **3** | 2 | 1 | — | 2 | **3** | 1 |
| **Politics** | 2 | 2 | 1 | 2 | — | 2 | 1 |
| **Technology** | **3** | 1 | 1 | **3** | 2 | — | 2 |
| **Art** | 2 | 1 | 1 | 1 | 1 | 2 | — |

---

## Strong Transfer Paths (Score = 3)

### Path 1: Philosophy ↔ Economics

**Mechanism Bridges**
| Mechanism | Philosophy Instance | Economics Instance |
|-----------|---------------------|-------------------|
| E-01 | Spontaneous order (Hayek/Smith) | Market coordination |
| MP-04 | Paradigm displacement | Market disruption |
| T-02 | Conceptual transformation | Policy paradigm shift |

**Exemplar Transfers**
- `adam-smith` ← `aristotle` (virtue → self-interest)
- `keynes` ← `hume` (uncertainty → animal spirits)
- `hayek` ← `kant` (knowledge limits → price signals)

---

### Path 2: Economics ↔ Technology

**Mechanism Bridges**
| Mechanism | Economics Instance | Technology Instance |
|-----------|-------------------|---------------------|
| F-02 | Network effects | Platform dynamics |
| TE-03 | Marginal cost collapse | Reproduction cost zero |
| MP-04 | Market disruption | Gatekeeper displacement |

**Exemplar Transfers**
- `platform-economics` ← `tcp-ip` (protocol → market design)
- `creative-destruction` ← `digital-revolution` (innovation cycles)
- `network-effects` ↔ `internet` (bidirectional)

---

### Path 3: Philosophy ↔ Technology

**Mechanism Bridges**
| Mechanism | Philosophy Instance | Technology Instance |
|-----------|---------------------|---------------------|
| TE-02 | Conceptual layering | Protocol stack |
| MP-02 | Paradigm threshold | Adoption threshold |
| T-01 | School succession | Platform substitution |

**Exemplar Transfers**
- `tcp-ip` ← `thales` (abstraction principle)
- `ai-revolution` ← `descartes` (mind-machine)
- `information-theory` ← `leibniz` (symbolic logic)

---

## Moderate Transfer Paths (Score = 2)

| Path | Common Mechanisms | Notes |
|------|-------------------|-------|
| Philosophy → Politics | T-02, MP-04 | Legitimacy frameworks |
| Philosophy → Art | MP-04, E-01 | Aesthetic paradigms |
| Economics → Politics | V-02, F-01 | Policy constraints |
| History → Politics | C-02, V-01 | Regime dynamics |
| Technology → Art | TE-03, F-02 | Reproduction/distribution |
| Politics → History | T-01, MP-02 | State formation |

---

## Transfer Validation

| Check | Criterion | Status |
|-------|-----------|--------|
| TG-01 | All 7 domains represented | PASS |
| TG-02 | Scoring rubric defined | PASS |
| TG-03 | Strong paths (≥3) documented with exemplars | PASS |
| TG-04 | Matrix is symmetric (bidirectional weights) | PASS |
| TG-05 | No score >3 or <0 | PASS |

---

## Usage

**To assess transfer potential for a new entity:**

1. Identify entity's primary mechanisms
2. Find domains with matching mechanisms in transfer matrix
3. Score = highest matching cell value
4. If score ≥2, transfer is viable; document bridge mechanisms

**To propose cross-domain connection:**

1. Identify shared mechanism IDs
2. Count co-occurrences across domains
3. Apply scoring rubric
4. If score ≥2, add to `135_Meta/cross-entity-matrix.md`

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-04 | Initial transfer graph; P↔E↔T triangle documented |
