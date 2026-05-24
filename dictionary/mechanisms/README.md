# 040_OS - Pattern Engine

**Version**: 1.0
**Updated**: 2026-03-08

The operational engine layer for Knowledge OS pattern extraction and structural analysis.

---

## File Relationship Map

```
pattern-dictionary.md (v0.3, Source of Truth)
    ├── refs → pattern-compression-v0.2.md (normalization rules)
    ├── refs → pattern-canon-v1.md (CANON-01~05)
    ├── refs → pattern-stacks.md (STACK-01~02)
    ├── refs → meta-patterns.md (MP-01~13)
    ├── refs → collapse-archetypes.md
    └── refs → substitution-archetypes.md

archetype-registry.md (v1.0, A01~A08)
    └── spec → structural-archetype-engine.md

meta-pattern-registry.md (v1.0, M01~M12)
    └── links → archetype-registry.md (A01~A08)
    └── links → civilization-loop-registry.md (S0~S5)

dynamics-loop-model.md (detailed: 11 states)
    └── integrated → civilization-loop-engine.md (overlay integration)
        └── abstracted → civilization-loop-registry.md (high-level: 6 states)

intervention-engine.md + intervention-registry.md (latest feature)

action-grammar.md (Action Layer grammar definitions)
    └── defines → action-schema.md (output schema)
        └── outputs → 142_Action/ (action files)
```

---

## Layer Abstractions

| Layer | File | Purpose |
|-------|------|---------|
| **Grammar** | pattern-dictionary.md | 6 canonical grammar types |
| **Mechanism** | pattern-dictionary.md | 19 mechanism IDs (C/T/F/V/PO/TE/E) |
| **Meta-Pattern** | meta-patterns.md | 13 higher-order patterns (MP-01~13) |
| **Archetype** | archetype-registry.md | 8 structural archetypes (A01~A08) |
| **Stack** | pattern-stacks.md | 2 mechanism combinations (STACK-01~02) |
| **Canon** | pattern-canon-v1.md | 5 canonical formulas (CANON-01~05) |
| **Cluster** | cluster-*.md | 4 domain groupings (CLUSTER-*) |
| **Loop State** | civilization-loop-registry.md | 6 civilization states (S0~S5) |

---

## ID Schema Reference

| System | Range | Example | Source File |
|--------|-------|---------|-------------|
| Grammar | 6 types | `emergence`, `collapse` | pattern-dictionary.md |
| Mechanism | C/T/F/V/PO/TE/E-XX | `[C-01]`, `[T-01]` | pattern-dictionary.md |
| Meta-Pattern | MP-01~13 | `[MP-04]` | meta-patterns.md |
| Meta-Pattern (registry) | M01~M12 | `M01` | meta-pattern-registry.md |
| Archetype | A01~A08 | `A01` | archetype-registry.md |
| Stack | STACK-XX | `STACK-01` | pattern-stacks.md |
| Canon | CANON-XX | `CANON-04` | pattern-canon-v1.md |
| Cluster | CLUSTER-* | `CLUSTER-CRISIS` | cluster-*.md |
| Loop State | S0~S5 | `S1` | civilization-loop-registry.md |

---

## Known Schema Divergence

**MP-XX vs M-XX**: Two ID systems for meta-patterns exist:
- `MP-01~MP-13` in meta-patterns.md (human documentation, 13 patterns)
- `M01~M12` in meta-pattern-registry.md (machine-readable, 12 patterns with archetype links)

These serve different purposes and are both maintained.

---

## Changelog

| Date | Change |
|------|--------|
| 2026-03-08 | Initial README created; documented file relationships |
