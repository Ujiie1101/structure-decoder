---
type: pattern-canon
version: v1.0
date: 2026-03-04
pattern_count: 5
source: structural-analysis-177-entities
---

# Pattern Canon v1.0

Canonical structural patterns extracted from co-occurrence analysis of 177 Core entities.

---

## Canon Registry

### CANON-01 | Innovation-Displacement

| Field | Value |
|-------|-------|
| **name** | Innovation-Displacement |
| **formula** | `E-01 → MP-04 → T-01` |
| **loop_type** | emergence → substitution |
| **dominant_grammar** | emergence, substitution |
| **mechanisms** | E-01 (Invisible Hand), MP-04 (Gatekeeper Displacement), T-01 (Institutional Substitution) |
| **coverage** | 48 co-occurrences (E-01 × MP-04) |
| **example_entities** | thales, tcp-ip, john-calvin, monet, dharma, anaximander |
| **transfer_potential** | HIGH (Philosophy ↔ Technology ↔ Economics ↔ Art) |

**Description**: Emergent self-organization produces novel structures that displace incumbent gatekeepers, leading to gradual institutional substitution.

---

### CANON-02 | Reflexive-Crisis

| Field | Value |
|-------|-------|
| **name** | Reflexive-Crisis |
| **formula** | `V-02 → MP-01 → C-01/C-02 → MP-03` |
| **loop_type** | lock-in → reflexive → cascade → collapse |
| **dominant_grammar** | collapse |
| **mechanisms** | V-02 (Policy Lock-in), MP-01 (Reflexive Spiral), C-01 (Leverage Cascade), C-02 (Confidence Contagion), MP-03 (Self-Undermining Success) |
| **coverage** | 29 co-occurrences (MP-03 × V-02) |
| **example_entities** | ltcm-collapse, gfc-2008, great-depression, japan-bubble, minsky-moment |
| **transfer_potential** | MEDIUM (Economics dominant; some Politics/History) |

**Description**: Policy orthodoxy creates lock-in; reflexive dynamics build pressure; threshold breach triggers cascade; success itself creates failure conditions.

---

### CANON-03 | Paradigm-Transformation

| Field | Value |
|-------|-------|
| **name** | Paradigm-Transformation |
| **formula** | `MP-02 → T-02 → MP-04` |
| **loop_type** | threshold → transformation |
| **dominant_grammar** | substitution, emergence |
| **mechanisms** | MP-02 (Threshold Transition), T-02 (Procedural Transformation), MP-04 (Gatekeeper Displacement) |
| **coverage** | 35 co-occurrences (MP-02 × T-02) |
| **example_entities** | adam-smith, keynes, friedman, protagoras, kant, kuhn |
| **transfer_potential** | HIGH (Philosophy ↔ Economics ↔ Politics) |

**Description**: Critical threshold crossed enables procedural/conceptual transformation, displacing prior paradigm's gatekeepers.

---

### CANON-04 | Technology-Stack

| Field | Value |
|-------|-------|
| **name** | Technology-Stack |
| **formula** | `TE-02 → F-02 → TE-03 → T-01` |
| **loop_type** | accumulation → network → displacement |
| **dominant_grammar** | emergence |
| **mechanisms** | TE-02 (Protocol Layering), F-02 (Network Effect), TE-03 (Reproduction Cost Collapse), T-01 (Institutional Substitution) |
| **coverage** | 32 co-occurrences (T-01 × TE-02) |
| **example_entities** | transistor, internet, tcp-ip, digital-revolution, telegraph, printing-press |
| **transfer_potential** | MEDIUM (Technology dominant; transfers to Economics) |

**Description**: Protocol layering enables network effects; reproduction cost collapse disrupts incumbents; institutional substitution follows.

---

### CANON-05 | Empire-Decline

| Field | Value |
|-------|-------|
| **name** | Empire-Decline |
| **formula** | `V-01 → T-01 → C-03` |
| **loop_type** | erosion → fragmentation → collapse |
| **dominant_grammar** | erosion, collapse |
| **mechanisms** | V-01 (Overextension-Fragmentation), T-01 (Institutional Substitution), C-03 (Institutional Sclerosis/Retaliation Cascade) |
| **coverage** | 25 co-occurrences (T-01 × V-01) |
| **example_entities** | fall-of-roman-empire, fall-of-constantinople, habsburg-decline, ottoman-decline |
| **transfer_potential** | MEDIUM (History ↔ Politics) |

**Description**: Administrative overextension enables peripheral autonomy; functions transfer outward; institutional sclerosis prevents adaptation; gradual-then-sudden collapse.

---

## Canon Validation Matrix

| Canon | Formula Valid | Coverage ≥20 | Grammar Aligned | Transfer Scored | Status |
|-------|---------------|--------------|-----------------|-----------------|--------|
| CANON-01 | ✓ | ✓ (48) | ✓ | ✓ | PASS |
| CANON-02 | ✓ | ✓ (29) | ✓ | ✓ | PASS |
| CANON-03 | ✓ | ✓ (35) | ✓ | ✓ | PASS |
| CANON-04 | ✓ | ✓ (32) | ✓ | ✓ | PASS |
| CANON-05 | ✓ | ✓ (25) | ✓ | ✓ | PASS |

---

## Canon-to-Grammar Mapping

| Canon | emergence | substitution | inversion | collapse | erosion | fragmentation |
|-------|-----------|--------------|-----------|----------|---------|---------------|
| CANON-01 | ● | ● | | | | |
| CANON-02 | | | | ● | | |
| CANON-03 | ● | ● | | | | |
| CANON-04 | ● | | | | | |
| CANON-05 | | | | ● | ● | ● |

---

## Canon-to-Stack Relationship

| Canon | STACK-01 Overlap | Notes |
|-------|------------------|-------|
| CANON-01 | Partial (MP-04, T-01) | Adds E-01 |
| CANON-02 | Low | Different mechanism set |
| CANON-03 | High (MP-02, MP-04, T-01 core overlap) | Alternative entry via T-02 |
| CANON-04 | Partial (T-01) | Domain-specific (Tech) |
| CANON-05 | Partial (T-01) | Decline variant |

---

## Usage

**To classify an entity under a canon:**

1. Extract entity's mechanism mappings
2. Match against canon formulas (≥3 mechanism match)
3. Verify grammar alignment
4. Tag in frontmatter: `canon: CANON-XX`

**To propose a new canon:**

1. Identify recurring mechanism combination (coverage ≥20)
2. Document formula and loop type
3. Provide ≥5 example entities
4. Submit for validation against canon criteria

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-04 | Initial canon registration (5 patterns) |
