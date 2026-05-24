---
type: structural-archetype-engine
version: v1.1.0
date: 2026-03-05
archetype_count: 6
core_grammar: [emergence, substitution, erosion, collapse, fragmentation, inversion]
extended_grammar: [crisis, institutionalization]
meta_output: 135_Meta/archetype-index.json
integrates_with: 040_OS/civilization-loop-engine.md
backward_compatible: true
---

# Structural Archetype Engine v1.1

## 1. Purpose

The Structural Archetype Engine classifies entities by **grammar transition sequences** — the dominant pattern of structural change an entity exhibits.

**Primary Functions**:
1. Detect recurring grammar-to-grammar transitions across the entity base
2. Classify entities into archetype families
3. Output archetype assignments with confidence scores
4. Enable cross-domain structural comparison at the grammar level

**Integration Point**: This engine operates downstream of the Civilization Loop Engine. It consumes:
- Grammar type assignments (`patterns:` frontmatter)
- Loop state paths (from civilization-loop-engine analysis)
- Overlay assignments (STACK/CANON/CLUSTER)

**Compatibility**: The canonical 6-state loop in civilization-loop-engine.md remains unchanged. This engine extends classification capability without modifying the core loop.

---

## 2. Grammar Classification

### 2.1 Core Grammar (6 Types)

The **canonical** grammar types used by the Civilization Loop Engine:

| Grammar | Definition | Loop Role |
|---------|------------|-----------|
| `emergence` | Novel properties arising from reconfigured components | Renewal operator |
| `substitution` | Gradual replacement of incumbent structure | Transformation operator |
| `erosion` | Gradual decay of capacity, trust, or legitimacy | Decline operator |
| `collapse` | Sudden systemic failure | Crisis operator |
| `fragmentation` | Unity dissolution into parts | Modifier (any state) |
| `inversion` | Hierarchy or value reversal | Modifier (any state) |

**Rule**: These 6 types are the **only** valid values for entity `patterns:` frontmatter fields.

### 2.2 Extended Grammar (2 Types)

**Transition amplifiers** used exclusively by the Archetype Engine for sequence classification:

| Extended | Definition | Archetype Role |
|----------|------------|----------------|
| `crisis` | Systemic instability / pressure state | Transition amplifier between core states |
| `institutionalization` | Embedding of new structure as norm | Stabilization marker following transformation |

**Rule**: Extended grammar are **annotation-level constructs**. They:
- Do NOT appear in entity `patterns:` frontmatter
- Do NOT modify the 6-state canonical loop
- Are used ONLY in archetype sequence definitions
- Map to core grammar for loop projection (see 2.3)

### 2.3 Extended-to-Core Projection

When archetype sequences include extended grammar, project to core loop as follows:

| Extended | Projects To | Rationale |
|----------|-------------|-----------|
| `crisis` | `collapse` (or `erosion` → `collapse`) | Crisis represents instability phase preceding/during collapse |
| `institutionalization` | `substitution` → `stability` | Institutionalization represents post-substitution locking |

**Projection Function**:
```
project_to_core(grammar):
  IF grammar IN core_grammar:
    RETURN grammar
  ELSE IF grammar == "crisis":
    RETURN "collapse"
  ELSE IF grammar == "institutionalization":
    RETURN "substitution"  # or loop_state "stabilization"
```

**Usage**: When computing entity loop paths for civilization-loop-engine compatibility, apply projection. Archetype assignment uses full sequences (core + extended).

---

## 3. Archetypes vs. Stacks vs. Canons

| Dimension | Stack | Canon | Archetype |
|-----------|-------|-------|-----------|
| **Unit** | Mechanism combination | Mechanism formula | Grammar sequence |
| **Granularity** | Mechanism-level | Mechanism-level | Grammar-level |
| **Format** | `STACK-XX` | `CANON-XX` | `ARCH-XX-YY` |
| **Detection** | All components present | Formula match + path alignment | Grammar sequence match |
| **Scope** | Cross-domain structural scaffold | Loop-path specific | Grammar-transition specific |
| **Question** | "What mechanisms co-occur?" | "What mechanism path defines this?" | "What grammar transition dominates?" |

### Hierarchy

```
[Entity]
   |
   +-- mechanisms: [MP-02, MP-04, T-01, ...]
   |       |
   |       +-- STACK: mechanism co-occurrence
   |       +-- CANON: mechanism formula sequence
   |
   +-- patterns: [emergence, substitution, ...]  (core grammar only)
           |
           +-- ARCHETYPE: grammar transition sequence (core + extended)
```

**Key Distinction**:
- **Stacks** and **Canons** operate at the mechanism level
- **Archetypes** operate at the grammar level
- Archetypes compress mechanism-level detail into higher-order structural signatures

---

## 4. Archetype Registry

### Summary Table

| ID | Sequence | Grammar Types | Meaning |
|----|----------|---------------|---------|
| ARCH-ES-01 | emergence → substitution | core → core | Innovation displacement |
| ARCH-EC-01 | emergence → crisis | core → extended | System shock |
| ARCH-CI-01 | crisis → institutionalization | extended → extended | Reordering |
| ARCH-SI-01 | substitution → institutionalization | core → extended | System stabilization |
| ARCH-ER-01 | erosion → collapse | core → core | Terminal decline |
| ARCH-FI-01 | fragmentation → inversion | core → core | Revolutionary dissolution |

---

### ARCH-ES-01 | Emergence → Substitution

| Field | Value |
|-------|-------|
| **ID** | `ARCH-ES-01` |
| **Sequence** | `emergence → substitution` |
| **Grammar Types** | core → core |
| **Definition** | Novel structure emerges and replaces incumbent framework |
| **Civilization Meaning** | Innovation displacement |
| **Core Projection** | emergence → substitution (no change) |
| **Loop States** | emergence → substitution-* → stabilization |
| **Overlay Affinity** | CANON-01, CANON-04, STACK-01 |
| **Example Entity Types** | Philosophy thinkers, technology inventions, economic paradigms |

---

### ARCH-EC-01 | Emergence → Crisis

| Field | Value |
|-------|-------|
| **ID** | `ARCH-EC-01` |
| **Sequence** | `emergence → crisis` |
| **Grammar Types** | core → extended |
| **Definition** | Novel structure emerges and triggers systemic instability |
| **Civilization Meaning** | System shock |
| **Core Projection** | emergence → collapse |
| **Loop States** | emergence → threshold-breach → collapse-cascade |
| **Overlay Affinity** | CLUSTER-CRISIS, STACK-02 |
| **Example Entity Types** | Disruptive innovations, market shocks, paradigm conflicts |

---

### ARCH-CI-01 | Crisis → Institutionalization

| Field | Value |
|-------|-------|
| **ID** | `ARCH-CI-01` |
| **Sequence** | `crisis → institutionalization` |
| **Grammar Types** | extended → extended |
| **Definition** | System crisis enables new institutional order |
| **Civilization Meaning** | Reordering |
| **Core Projection** | collapse → substitution |
| **Loop States** | collapse-* → substitution-* → stabilization → stability |
| **Overlay Affinity** | CLUSTER-CRISIS, CLUSTER-REVOLUTION, CANON-02 |
| **Example Entity Types** | Post-crisis reforms, revolutionary settlements, reconstruction eras |

---

### ARCH-SI-01 | Substitution → Institutionalization

| Field | Value |
|-------|-------|
| **ID** | `ARCH-SI-01` |
| **Sequence** | `substitution → institutionalization` |
| **Grammar Types** | core → extended |
| **Definition** | Replacement structure becomes embedded as new norm |
| **Civilization Meaning** | System stabilization |
| **Core Projection** | substitution → substitution (stabilization phase) |
| **Loop States** | substitution-* → stabilization → stability |
| **Overlay Affinity** | STACK-01, CANON-01, CANON-03 |
| **Example Entity Types** | Constitutional settlements, standards adoption, paradigm consolidation |

---

### ARCH-ER-01 | Erosion → Collapse

| Field | Value |
|-------|-------|
| **ID** | `ARCH-ER-01` |
| **Sequence** | `erosion → collapse` |
| **Grammar Types** | core → core |
| **Definition** | Gradual decay culminates in systemic failure |
| **Civilization Meaning** | Terminal decline |
| **Core Projection** | erosion → collapse (no change) |
| **Loop States** | stability → erosion → threshold-breach → collapse-* |
| **Overlay Affinity** | CANON-05, CLUSTER-EMPIRE |
| **Example Entity Types** | Empire decline, institutional failure, organizational death |

---

### ARCH-FI-01 | Fragmentation → Inversion

| Field | Value |
|-------|-------|
| **ID** | `ARCH-FI-01` |
| **Sequence** | `fragmentation → inversion` |
| **Grammar Types** | core → core |
| **Definition** | Unity breaks apart; hierarchy reverses |
| **Civilization Meaning** | Revolutionary dissolution |
| **Core Projection** | fragmentation → inversion (no change) |
| **Loop States** | erosion [+fragmentation] → substitution [+inversion] |
| **Overlay Affinity** | CLUSTER-REVOLUTION, CLUSTER-EMPIRE |
| **Example Entity Types** | Decolonization, decentralization movements, regime inversion |

---

## 5. Detection Logic

### 5.1 Input Specification

```json
{
  "entity_slug": "string",
  "patterns": ["emergence", "substitution"],
  "stack_ids": ["STACK-01"],
  "canon_tags": ["CANON-01"],
  "cluster_tags": [],
  "loop_state_path": ["stability", "emergence", "substitution-category", "stabilization"]
}
```

**Note**: `patterns[]` contains only core grammar. Extended grammar are inferred from loop state paths and overlay context.

### 5.2 Processing Pipeline

```
INPUT: entity_data, archetype_registry

PROCESS:

1. VALIDATE
   - patterns[] must be non-empty
   - all values must be core grammar types (6)
   - REJECT if validation fails

2. EXTRACT transition
   primary := patterns[0]
   secondary := patterns[1] if exists, else infer from loop_state_path

   # Infer extended grammar from context
   IF loop_state_path includes collapse-cascade AND patterns lacks "collapse":
     inferred_extended := "crisis"
   IF loop_state_path ends with stability AND patterns includes "substitution":
     inferred_extended := "institutionalization"

3. MATCH archetype
   FOR each ARCH in registry:
     score := 0.0

     # Direct match (core grammar)
     IF (primary, secondary) == ARCH.sequence:
       score := 1.0

     # Projected match (extended grammar)
     ELSE IF (primary, inferred_extended) == ARCH.sequence:
       score := 0.8
     ELSE IF project_to_core(ARCH.sequence) == (primary, secondary):
       score := 0.7

     # Overlay bonus
     IF entity.overlays INTERSECT ARCH.overlay_affinity:
       score += 0.1

     candidates[ARCH.id] := score

4. SELECT best match
   best := max(candidates, key=score)
   IF best.score < 0.5:
     RETURN null

5. CALCULATE confidence
   confidence := weighted_average(
     pattern_match: 0.4,
     overlay_alignment: 0.3,
     frequency_support: 0.3
   )

6. OUTPUT
   RETURN {
     archetype_id: best.id,
     confidence: confidence,
     supporting_entities: query_similar(best.id, limit=10)
   }
```

### 5.3 Confidence Thresholds

| Range | Classification | Action |
|-------|----------------|--------|
| ≥ 0.75 | High | Auto-assign |
| 0.50 – 0.74 | Medium | Manual review recommended |
| < 0.50 | Low | Do not assign |

### 5.4 Output Specification

```json
{
  "archetype_id": "ARCH-ES-01",
  "sequence": ["emergence", "substitution"],
  "sequence_types": ["core", "core"],
  "confidence": 0.82,
  "match_factors": {
    "pattern_match": 1.0,
    "overlay_alignment": 0.6,
    "frequency_support": 0.8
  },
  "core_projection": ["emergence", "substitution"],
  "supporting_entities": ["thales", "anaximander", "tcp-ip", "printing-press"]
}
```

---

## 6. Meta Output Specification: archetype-index.json

### 6.1 Purpose

`135_Meta/archetype-index.json` aggregates archetype assignments across all entities for:
- Coverage analysis
- Cross-domain pattern detection
- Archetype frequency reporting

### 6.2 Schema

```json
{
  "$schema": "archetype-index-v1.0",
  "schema_version": "1.0",
  "generated_at": "2026-03-05T12:00:00Z",
  "generated_by": "kos_meta.py",
  "grammar_model": {
    "core": ["emergence", "substitution", "erosion", "collapse", "fragmentation", "inversion"],
    "extended": ["crisis", "institutionalization"]
  },
  "statistics": {
    "total_archetypes": 6,
    "total_assignments": 0,
    "coverage_rate": 0.0,
    "high_confidence_count": 0,
    "medium_confidence_count": 0
  },
  "archetypes": [
    {
      "archetype": "ARCH-ES-01",
      "name": "Emergence-Substitution",
      "sequence": ["emergence", "substitution"],
      "sequence_types": ["core", "core"],
      "entity_count": 28,
      "avg_confidence": 0.78,
      "supporting_entities": ["thales", "anaximander", "tcp-ip", "printing-press", "adam-smith"],
      "domain_distribution": {
        "philosophy": 12,
        "technology": 8,
        "economics": 5,
        "religion": 3
      },
      "overlay_distribution": {
        "STACK-01": 15,
        "CANON-01": 10,
        "CANON-04": 8
      }
    }
  ],
  "unclassified": {
    "count": 0,
    "entities": []
  }
}
```

### 6.3 Field Definitions

| Field | Type | Description |
|-------|------|-------------|
| `archetype` | string | Archetype ID (ARCH-XX-YY) |
| `name` | string | Human-readable name |
| `sequence` | array[2] | Grammar sequence |
| `sequence_types` | array[2] | "core" or "extended" per element |
| `entity_count` | integer | Assigned entity count |
| `avg_confidence` | float | Mean confidence across assignments |
| `supporting_entities` | array | Sample entities (max 10) |
| `domain_distribution` | object | Per-domain counts |
| `overlay_distribution` | object | Per-overlay counts |

### 6.4 Generation

```bash
# Future implementation
python scripts/kos_meta.py archetype
```

**Note**: File not yet generated. Specification only.

---

## 7. Archetype-Overlay Alignment Matrix

| Archetype | STACK-01 | STACK-02 | CANON-01 | CANON-02 | CANON-04 | CANON-05 | CLUSTER-CRISIS | CLUSTER-REVOLUTION | CLUSTER-EMPIRE |
|-----------|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------------:|:------------------:|:--------------:|
| ARCH-ES-01 | ● | - | ● | - | ● | - | - | ○ | - |
| ARCH-EC-01 | - | ● | - | ● | - | - | ● | ○ | - |
| ARCH-CI-01 | ○ | ● | - | ● | - | - | ● | ● | - |
| ARCH-SI-01 | ● | - | ● | - | - | - | - | ○ | - |
| ARCH-ER-01 | - | ○ | - | - | - | ● | ○ | - | ● |
| ARCH-FI-01 | - | - | - | - | - | ○ | - | ● | ● |

**Legend**: ● strong | ○ weak | - none

---

## 8. Validation Checklist

| Check | Criterion |
|-------|-----------|
| SAE-01 | Entity has ≥1 grammar type in `patterns:` |
| SAE-02 | All `patterns:` values are core grammar (6 types) |
| SAE-03 | Archetype sequence matches entity grammar order |
| SAE-04 | Confidence ≥ 0.50 |
| SAE-05 | Overlay assignments do not conflict with affinity |
| SAE-06 | Loop state path aligns with archetype (if available) |
| SAE-07 | Extended grammar inferred only from context, never stored in `patterns:` |

---

## 9. Compatibility Notes

### 9.1 Civilization Loop Engine Compatibility

- The canonical 6-state loop in `civilization-loop-engine.md` is **unchanged**
- Extended grammar (`crisis`, `institutionalization`) are **archetype-level annotations**
- Loop state computation **ignores** extended grammar; use projection function
- Entity `patterns:` fields contain **only** core grammar

### 9.2 Schema Compatibility

- No changes to `135_Meta/structure-index.json` schema
- Archetype data outputs to **new** file `135_Meta/archetype-index.json`
- Overlay IDs (STACK/CANON/CLUSTER) remain unchanged

### 9.3 Backward Compatibility

- Entities without archetype assignments remain valid
- Pipeline consumers ignoring archetype data will work unchanged
- Extended grammar are additive; no existing fields modified

---

## 10. Non-Goals

| Non-Goal | Clarification |
|----------|---------------|
| Replace overlays | Archetypes complement STACK/CANON/CLUSTER |
| Modify core grammar | The 6-type canonical loop is unchanged |
| Require mechanism data | Grammar-level operation; mechanisms optional |
| Modify existing schemas | New output file only |
| Force classification | Unclassifiable entities remain unassigned |

---

## 11. Future Extensions

| Extension | Description | Priority |
|-----------|-------------|----------|
| ARCH-IS-01 | Inversion → Substitution | Medium |
| ARCH-SE-01 | Substitution → Emergence | Medium |
| ARCH-CF-01 | Collapse → Fragmentation | Low |
| Multi-step | 3+ grammar sequences | Future |
| Archetype chains | Entity progression | Future |

---

## 12. References

| Document | Relationship |
|----------|--------------|
| `040_OS/civilization-loop-engine.md` | Canonical 6-state loop; overlay integration |
| `040_OS/archetype-registry.md` | Archetype ID registry |
| `040_OS/grammar-distribution.md` | Grammar frequency analysis |
| `135_Meta/structure-index.json` | Entity-level data source |
| `135_Meta/archetype-index.json` | Output specification |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.1.0 | 2026-03-05 | Core/extended grammar distinction; projection function; compatibility notes |
| v1.0.0 | 2026-03-05 | Initial specification; 6 archetypes |
