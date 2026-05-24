---
type: civilization-loop-engine
version: v0.1.0
date: 2026-03-04
states: 11
overlays_integrated: [stacks, canons, clusters]
grammar_types: [erosion, collapse, substitution, inversion, fragmentation, emergence]
source: dynamics-loop-model + pattern-overlays
---

# Civilization Loop Engine v0.1

## 1. Purpose

The Civilization Loop Engine provides a unified operational model that integrates:
- **Loop states** from the Dynamics Loop Model (state transitions)
- **Overlays** (STACK/CANON/CLUSTER) as structural annotations
- **Grammar types** as transition operators

This engine enables:
- Consistent overlay assignment during entity promotion
- Cross-domain structural comparison via shared state-overlay vocabulary
- Validation that overlays correctly map to loop dynamics
- Detection of incomplete or misclassified structures

**This engine does NOT**:
- Replace existing overlay registries (040_OS/pattern-*.md)
- Introduce new grammar types or mechanisms
- Require schema changes to structure-index.json

---

## 2. Canonical Loop States

| State | Definition | Phase |
|-------|------------|-------|
| **stability** | System operates within normal parameters; negative feedback dominates | Equilibrium |
| **erosion** | Gradual decay of legitimacy, trust, or capacity; buffers depleting | Decline |
| **threshold-proximity** | System approaches critical threshold; early warning signals | Transition |
| **threshold-breach** | Critical threshold crossed; state transition initiated | Transition |
| **collapse-cascade** | Rapid propagation of failures through high-connectivity network | Crisis |
| **collapse-erosion** | Prolonged functional decay until structural disintegration | Crisis |
| **substitution-category** | Foundational framework or legitimacy basis being replaced | Transformation |
| **substitution-functional** | Operational authority migrating between nodes | Transformation |
| **substitution-scarcity** | Value/scarcity concentration shifting to new domain | Transformation |
| **emergence** | Novel properties arising from reconfigured components | Renewal |
| **stabilization** | New equilibrium forming; positive feedback dampening | Renewal |

**State Modifiers** (applicable at any state):
- `[inversion]` — hierarchy/value reversal
- `[fragmentation]` — unity breaking into parts

---

## 3. Transition Operators (Grammar Types)

Grammar types define **how** transitions occur between states.

| Grammar Type | Transition Pattern | Typical State Sequences |
|--------------|-------------------|-------------------------|
| **erosion** | Gradual decay | stability → erosion → threshold-proximity |
| **collapse** | Sudden failure | threshold-breach → collapse-cascade OR collapse-erosion |
| **substitution** | Gradual replacement | collapse-* → substitution-* → emergence |
| **emergence** | Novel reconfiguration | substitution-* → emergence → stabilization |
| **inversion** | Hierarchy reversal | (modifier on any transition) |
| **fragmentation** | Unity dissolution | erosion → fragmentation → substitution-functional |

### Transition Rules

```
ALLOWED:
  stability → erosion
  erosion → threshold-proximity
  erosion → collapse-erosion (slow path)
  erosion → substitution-* (managed transition)
  threshold-proximity → threshold-breach
  threshold-breach → collapse-cascade
  threshold-breach → collapse-erosion
  collapse-* → substitution-*
  substitution-* → emergence
  emergence → stabilization
  stabilization → stability

FORBIDDEN:
  stability → collapse-cascade (must pass through erosion/threshold)
  emergence → erosion (cannot decay before stabilizing)
  collapse-cascade → stability (must complete substitution)
```

---

## 4. Overlay Integration Rules

### 4.1 STACK: Structural Scaffolds

**Definition**: Stacks are recurring mechanism combinations that appear across multiple loop states. They represent structural signatures, not loop positions.

**Integration Rule**:
```
STACK attaches to entities that contain ALL stack components,
regardless of which loop state the entity occupies.

STACK-01 (Threshold-Displacement-Substitution):
  Components: MP-02 + MP-04 + T-01
  Expected states: threshold-breach, substitution-*, emergence

IF entity.mechanisms CONTAINS [MP-02, MP-04, T-01]
   AND entity spans states [threshold-*, substitution-*, emergence]
THEN tag: stack_ids: ["STACK-01"]
```

**Validation**: Stack presence implies entity passes through threshold and substitution phases.

---

### 4.2 CANON: Canonical Exemplars

**Definition**: Canons are canonical structural patterns that define specific state transition sequences. Each canon maps to a characteristic loop path.

**Integration Rule**:
```
CANON defines a specific mechanism→state mapping.
Entity must match canon formula AND exhibit corresponding loop dynamics.
```

| Canon | Formula | Primary Loop Path |
|-------|---------|-------------------|
| **CANON-01** | E-01 → MP-04 → T-01 | stability → emergence → substitution-* → stabilization |
| **CANON-02** | V-02 → MP-01 → C-01/C-02 → MP-03 | erosion → threshold-breach → collapse-cascade |
| **CANON-03** | MP-02 → T-02 → MP-04 | threshold-breach → substitution-category |
| **CANON-04** | TE-02 → F-02 → TE-03 → T-01 | emergence → substitution-functional |
| **CANON-05** | V-01 → T-01 → C-03 | erosion → collapse-erosion → substitution-functional |

**Validation**: Canon tag requires both mechanism match AND loop path alignment.

---

### 4.3 CLUSTER: Empirical Validation

**Definition**: Clusters are empirical groupings of entities that exhibit repeated loop dynamics. They validate that similar mechanism combinations produce similar outcomes.

**Integration Rule**:
```
CLUSTER groups entities by shared crisis/transformation signature.
Entity must match cluster formula AND show historical loop completion.
```

| Cluster | Formula | Loop Signature |
|---------|---------|----------------|
| **CLUSTER-CRISIS** | (C-01 OR C-02) AND V-02 AND (MP-01 OR MP-03) | erosion → threshold-breach → collapse-cascade → substitution-* |

**Validation**: Cluster membership requires documented historical evidence of loop completion.

---

## 5. Overlay-State Mapping Matrix

| Loop State | STACK-01 | CANON-01 | CANON-02 | CANON-03 | CANON-04 | CANON-05 | CLUSTER-CRISIS |
|------------|----------|----------|----------|----------|----------|----------|----------------|
| stability | - | (start) | - | - | - | - | - |
| erosion | - | - | (start) | - | - | (start) | - |
| threshold-proximity | - | - | active | - | - | - | - |
| threshold-breach | active | - | active | active | - | - | - |
| collapse-cascade | - | - | active | - | - | - | active |
| collapse-erosion | - | - | - | - | - | active | - |
| substitution-category | - | - | - | active | - | - | - |
| substitution-functional | active | - | - | - | active | active | - |
| substitution-scarcity | - | - | - | - | active | - | - |
| emergence | active | active | - | - | active | - | - |
| stabilization | - | active | - | - | - | - | - |

---

## 6. Tagging Rubric

### During Promotion (Core → Structure)

**Step 1: Identify Loop Path**
```
1. Extract entity's Mechanism Mapping section
2. Construct loop_state_path from observed states
3. Validate path against allowed transitions
```

**Step 2: Check Stack Eligibility**
```
IF entity.mechanisms CONTAINS ALL of [MP-02, MP-04, T-01]
THEN add: stack_ids: ["STACK-01"]
```

**Step 3: Check Canon Eligibility**
```
FOR each CANON in [CANON-01..CANON-05]:
  IF entity.mechanisms MATCH canon.formula (≥3 mechanisms)
     AND entity.loop_path ALIGNS with canon.loop_path
  THEN add: canon_tags: ["CANON-XX"]
```

**Step 4: Check Cluster Eligibility**
```
FOR CLUSTER-CRISIS:
  IF entity.mechanisms MATCH (C-01 OR C-02) AND V-02 AND (MP-01 OR MP-03)
     AND entity.domain IN [economics, history]
     AND collapse grammar in entity.patterns
  THEN add: cluster_tags: ["CLUSTER-CRISIS"]
```

**Step 5: Validate Consistency**
```
IF entity has CANON-02 OR CLUSTER-CRISIS
   THEN entity.patterns MUST include "collapse"

IF entity has CANON-01 OR CANON-04
   THEN entity.patterns MUST include "emergence"

IF entity has STACK-01
   THEN entity.patterns MUST include "substitution"
```

---

## 7. Examples (Tagged Entities)

### Example 1: john-locke

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → emergence → substitution-category → stabilization |
| **overlays** | CANON-01, STACK-01 |
| **rationale** |
- Contains E-01, MP-04, T-01 → matches CANON-01 (Innovation-Displacement)
- Contains MP-02, MP-04, T-01 → matches STACK-01
- Emergent empiricism displaced rationalist gatekeepers; consent theory substituted divine right

---

### Example 2: anaximander

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → emergence → substitution-category → stabilization |
| **overlays** | CANON-01, STACK-01 |
| **rationale** |
- Contains E-01, MP-04, T-01 → matches CANON-01
- Apeiron as emergent abstraction; displaced elemental monism (Thales)
- Threshold transition from mythological to rational cosmology

---

### Example 3: ltcm-collapse

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → threshold-breach → collapse-cascade → substitution-functional |
| **overlays** | CANON-02, CLUSTER-CRISIS |
| **rationale** |
- Contains V-02, MP-01, C-01, MP-03 → matches CANON-02 (Reflexive-Crisis)
- Matches CLUSTER-CRISIS formula: C-01 + V-02 + MP-01 + MP-03
- Policy lock-in (model orthodoxy) → reflexive spiral → leverage cascade

---

### Example 4: great-depression-1929

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → threshold-breach → collapse-cascade → substitution-category |
| **overlays** | CLUSTER-CRISIS |
| **rationale** |
- Contains C-01, C-02, V-02, MP-01 → matches CLUSTER-CRISIS
- Gold standard lock-in → leverage cascade + confidence contagion
- Led to paradigm substitution (classical → Keynesian)

---

### Example 5: global-financial-crisis-2008

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → threshold-breach → collapse-cascade → substitution-functional |
| **overlays** | CLUSTER-CRISIS |
| **rationale** |
- Contains C-01, C-02, V-02, MP-01 → matches CLUSTER-CRISIS
- Rating model lock-in → repo market cascade + confidence freeze
- Functional substitution via Fed intervention

---

### Example 6: bretton-woods

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → substitution-functional → emergence → stabilization |
| **overlays** | STACK-01 |
| **rationale** |
- Contains MP-02, MP-04, T-01 → matches STACK-01
- Threshold breach (Nixon Shock) → gatekeeper displacement (British pound → dollar)
- No acute collapse; managed substitution

---

### Example 7: printing-revolution

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → emergence → substitution-scarcity → stabilization |
| **overlays** | CANON-04 |
| **rationale** |
- Contains TE-02, F-02, TE-03, T-01 → matches CANON-04 (Technology-Stack)
- Protocol layering (standardized type) → network effects (literacy spiral)
- Reproduction cost collapse disrupted scribal gatekeepers

---

### Example 8: civil-rights-movement

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → threshold-breach → substitution-category → stabilization |
| **overlays** | STACK-01 |
| **rationale** |
- Contains MP-02, MP-04, T-01 → matches STACK-01
- Threshold breach (Brown v. Board) → gatekeeper displacement (Jim Crow)
- Institutional substitution via Civil Rights Act

---

### Example 9: fall-of-rome

| Field | Value |
|-------|-------|
| **loop_state_path** | stability → erosion → collapse-erosion → substitution-functional → emergence |
| **overlays** | CANON-05 (candidate) |
| **rationale** |
- Contains V-01, T-01 → partial CANON-05 match (Empire-Decline)
- Administrative overextension → peripheral autonomy growth
- Prolonged erosion with function migration to foederati/church

---

## 8. Non-Goals

The Civilization Loop Engine explicitly does NOT:

| Non-Goal | Clarification |
|----------|---------------|
| **Create new grammar types** | Uses only: erosion, collapse, substitution, inversion, fragmentation, emergence |
| **Replace overlay registries** | References 040_OS/pattern-*.md as sources of truth |
| **Require schema changes** | Overlay fields remain optional per schema v2.0 |
| **Explain causation** | Classifies sequences, does not explain why transitions occur |
| **Predict outcomes** | Identifies likely paths, not deterministic futures |
| **Force classification** | Uncertain cases should remain untagged |
| **Require backfill** | Existing entities without overlays remain valid |

---

## 9. Validation Checklist

Before committing overlay tags, verify:

| Check | Criterion |
|-------|-----------|
| CLE-01 | Loop path uses only canonical states (11 states) |
| CLE-02 | Loop path follows allowed transitions |
| CLE-03 | Stack assignment requires ALL component mechanisms |
| CLE-04 | Canon assignment requires formula match AND path alignment |
| CLE-05 | Cluster assignment requires formula match AND domain match |
| CLE-06 | Grammar types in frontmatter align with overlay implications |
| CLE-07 | No deprecated mechanism IDs used |
| CLE-08 | Evidence proxies support classification |

---

## 10. References

| Document | Purpose |
|----------|---------|
| `040_OS/dynamics-loop-model.md` | State definitions and transitions |
| `040_OS/pattern-dictionary.md` | Mechanism and grammar definitions |
| `040_OS/pattern-stacks.md` | Stack registry |
| `040_OS/pattern-canon-v1.md` | Canon registry |
| `040_OS/crisis-cascade.md` | Cluster registry |
| `docs/loop-classification-rubric.md` | Classification gate |
| `docs/civilization-loop-rubric.md` | Overlay tagging decision tree |

---

## 11. Archetype Engine Compatibility Note

The **Structural Archetype Engine** (`040_OS/structural-archetype-engine.md`) operates downstream of this engine and classifies entities by grammar transition sequences.

**Key Points**:

1. **6-State Loop Remains Canonical**: This engine's 6 grammar types (emergence, substitution, erosion, collapse, fragmentation, inversion) are unchanged and authoritative.

2. **Extended Grammar Are Annotations**: The Archetype Engine uses two additional grammar terms (`crisis`, `institutionalization`) as **sequence-level annotations** for archetype classification. These are NOT loop states and do NOT modify the canonical loop.

3. **Projection Function**: When extended grammar appear in archetype sequences, they project to core grammar for loop compatibility:
   - `crisis` → `collapse`
   - `institutionalization` → `substitution` (stabilization phase)

4. **Entity `patterns:` Field**: Continues to accept only the 6 canonical grammar types. Extended grammar are inferred from context, never stored.

**No changes to this document's definitions, diagrams, or transition rules are required.**

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v0.1.1 | 2026-03-05 | Add archetype engine compatibility note |
| v0.1.0 | 2026-03-04 | Initial engine; integrates loop model + overlays |
