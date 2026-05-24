---
type: grammar-distribution
version: v1.0
date: 2026-03-04
entity_base: 177
source: structural-analysis-177-entities
---

# Grammar Distribution

## Current Distribution (n=177)

| Grammar | Count | Percentage | Primary Loop Type |
|---------|-------|------------|-------------------|
| **emergence** | 64 | 36.2% | Positive feedback |
| **substitution** | 52 | 29.4% | Gradual replacement |
| **inversion** | 42 | 23.7% | Reversal |
| **collapse** | 16 | 9.0% | Threshold breach |
| **erosion** | 9 | 5.1% | Gradual decay |
| **fragmentation** | 8 | 4.5% | Unity → parts |

*Note: Entities may have multiple grammar types; percentages reflect primary classification.*

---

## Grammar by Domain

| Domain | emergence | substitution | inversion | collapse | erosion | fragmentation |
|--------|-----------|--------------|-----------|----------|---------|---------------|
| Philosophy (49) | 42% | 28% | 24% | 4% | 2% | 0% |
| History (20) | 25% | 30% | 15% | 15% | 10% | 5% |
| Religion (18) | 33% | 33% | 22% | 6% | 6% | 0% |
| Economics (26) | 27% | 31% | 23% | 15% | 4% | 0% |
| Politics (20) | 30% | 25% | 25% | 10% | 5% | 5% |
| Technology (24) | 50% | 29% | 17% | 0% | 0% | 4% |
| Art (20) | 40% | 30% | 25% | 5% | 0% | 0% |

---

## Phase Estimator

Given a set of entities, estimate the dominant structural phase.

### Input
- Entity set with mechanism mappings
- Grammar type annotations (from frontmatter)

### Computation Rubric

**Step 1: Count grammar occurrences**
```
For each grammar type g in [emergence, substitution, inversion, collapse, erosion, fragmentation]:
    count[g] = number of entities with g as primary pattern
```

**Step 2: Calculate relative weights**
```
total = sum(count)
weight[g] = count[g] / total
```

**Step 3: Determine dominant phase**
```
IF weight[emergence] > 0.35 THEN phase = "GENERATIVE"
ELSE IF weight[substitution] > 0.30 THEN phase = "TRANSITIONAL"
ELSE IF weight[collapse] + weight[erosion] > 0.20 THEN phase = "DECLINING"
ELSE IF weight[inversion] > 0.25 THEN phase = "DIALECTICAL"
ELSE phase = "MIXED"
```

### Phase Definitions

| Phase | Dominant Grammar | Expected Dynamics |
|-------|------------------|-------------------|
| **GENERATIVE** | emergence ≥35% | New structures forming; positive feedback loops |
| **TRANSITIONAL** | substitution ≥30% | Established structures being replaced |
| **DECLINING** | collapse + erosion ≥20% | Structural degradation; threshold risks |
| **DIALECTICAL** | inversion ≥25% | Reversals and counter-movements |
| **MIXED** | No dominant | Multiple dynamics in tension |

### Current System Phase

Based on 177 entities:
- emergence: 36.2% → **exceeds 35% threshold**
- Phase classification: **GENERATIVE**

Interpretation: The Knowledge OS entity base reflects predominantly generative structural dynamics—new orders emerging from component interactions.

---

## Phase Trajectory Tracking

| Date | Entity Count | Phase | Notes |
|------|--------------|-------|-------|
| 2026-03-04 | 177 | GENERATIVE | Initial measurement |

*Update this table as entity count grows to track phase drift.*

---

## Validation Rules

| Check | Criterion | Status |
|-------|-----------|--------|
| G-01 | All 6 canonical grammar types represented | PASS |
| G-02 | Percentages sum to valid total (allowing overlap) | PASS |
| G-03 | Phase estimator produces deterministic output | PASS |
| G-04 | Domain breakdown available | PASS |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-04 | Initial grammar distribution; phase estimator defined |
