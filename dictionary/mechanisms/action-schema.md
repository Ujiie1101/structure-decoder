---
type: action-schema
version: v1.0
date: 2026-03-08
spec: 040_OS/action-grammar.md
output_dir: 142_Action/
---

# Action Schema v1.0

Standard schema for Action Layer outputs.

---

## 1. File Location

```
142_Action/
├── README.md
├── {condition-slug}.md      # Individual action files
└── _index.json              # Machine-readable index
```

---

## 2. Frontmatter Schema

```yaml
---
action_id: "ACT-{seq:3}"           # Unique ID (ACT-001, ACT-002, ...)
name: "kebab-case-name"            # Short identifier
structural_condition: "SC-XX"      # From action-grammar.md
source_patterns:                   # OS patterns this derives from
  - "STACK-XX"
  - "CANON-XX"
  - "CLUSTER-XX"
  - "A0X"
grammar_roots: ["erosion", "collapse"]  # Canonical grammar types
confidence: "high|mid|low|spec"    # Confidence level
domain_scope: "universal|domain-specific"
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

---

## 3. Body Structure

### 3.1 Structural Situation

```markdown
## Structural Situation

[2-4 sentences describing the structural condition in plain language]

**Condition Type**: SC-XX (name)
**Grammar Roots**: erosion, collapse, ...
**Historical Frequency**: [high/moderate/rare]
```

### 3.2 Scenario Branches

```markdown
## Scenario Branches

### Base Case
[Most probable trajectory given current structure]
- Probability framing: "tends to", "historically"
- NOT a prediction

### Risk Case
[Downside scenario if negative factors dominate]
- What accelerates this: [factors]
- Historical precedent: [if any]

### Opportunity Case
[Upside scenario if positive factors align]
- What enables this: [factors]
- Window characteristics: [timing, conditions]
```

### 3.3 Decision Signals

```markdown
## Decision Signals

| Signal | Type | Indicates | Monitor |
|--------|------|-----------|---------|
| [concrete observable] | SIG-X | [which branch strengthening] | [how to observe] |

**Early Warning**: [most important leading indicator]
**Confirmation**: [signal that branch is locked in]
```

### 3.4 Recommended Posture

```markdown
## Recommended Posture

**Primary**: AP-XX (name)
**Secondary**: AP-XX (name)

### Concrete Actions
1. [Specific action aligned with posture]
2. [Specific action aligned with posture]
3. [Specific action aligned with posture]

### Risk Posture
- RP-XX: [application to this situation]
```

### 3.5 Anti-Patterns

```markdown
## Anti-Patterns

| Mistake | Code | Why Dangerous |
|---------|------|---------------|
| [common error] | ANT-XX | [structural reason] |

**Most Common Trap**: [single biggest mistake]
```

### 3.6 Fragility Sources

```markdown
## Fragility Sources

| Source | Mechanism | Mitigation |
|--------|-----------|------------|
| [dependency/vulnerability] | [how it breaks] | [how to reduce] |
```

### 3.7 Optionality Paths

```markdown
## Optionality Paths

| Path | Enables | Cost | Reversibility |
|------|---------|------|---------------|
| [action that preserves options] | [what it opens] | [what it costs] | [high/med/low] |
```

### 3.8 Confidence Note

```markdown
## Confidence Note

**Structural Clarity**: [conf:X]
**Scenario Reliability**: [assessment]
**Key Uncertainty**: [what could invalidate this reading]
```

---

## 4. Minimal Template

```markdown
---
action_id: "ACT-XXX"
name: "example-action"
structural_condition: "SC-XX"
source_patterns: ["STACK-XX"]
grammar_roots: ["erosion"]
confidence: "mid"
domain_scope: "universal"
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# Action: Example Name

## Structural Situation

[Description]

**Condition Type**: SC-XX
**Grammar Roots**: [types]

## Scenario Branches

### Base Case
[Description]

### Risk Case
[Description]

### Opportunity Case
[Description]

## Decision Signals

| Signal | Type | Indicates |
|--------|------|-----------|
| | | |

## Recommended Posture

**Primary**: AP-XX

## Anti-Patterns

| Mistake | Code |
|---------|------|
| | |

## Confidence Note

**Structural Clarity**: [conf:X]
```

---

## 5. Validation Rules

1. `action_id` must be unique
2. `structural_condition` must reference valid SC-XX from action-grammar.md
3. `source_patterns` must reference existing STACK/CANON/CLUSTER/Archetype
4. `grammar_roots` must use only canonical 6 types
5. Scenario branches must be <=3
6. Decision signals must be observable (not abstract)
7. Anti-patterns must reference ANT-XX codes
8. Postures must reference AP-XX or RP-XX codes

---

## 6. Index Schema (_index.json)

```json
{
  "version": "1.0",
  "generated": "YYYY-MM-DD",
  "actions": [
    {
      "action_id": "ACT-001",
      "name": "example",
      "structural_condition": "SC-XX",
      "source_patterns": ["STACK-XX"],
      "confidence": "mid",
      "file": "example.md"
    }
  ]
}
```

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-08 | Initial schema definition |
