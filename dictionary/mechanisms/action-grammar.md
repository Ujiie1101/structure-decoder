---
type: action-grammar
version: v1.0
date: 2026-03-08
posture_count: 8
signal_types: 6
anti_pattern_categories: 7
---

# Action Grammar v1.0

Defines the grammar for translating structural patterns into decision-oriented guidance.

---

## 1. Core Principle

The Action Layer does NOT predict specific events.

It translates **structural recognition** into **strategic orientation**.

```
Structure Recognition → Scenario Branching → Action Posture
```

The question is NOT: "What exactly will happen?"
The question IS: "Given this structure, how should a person orient?"

---

## 2. Structural Condition Types

Canonical conditions derived from 040_OS grammar types and patterns:

| Condition ID | Name | Definition | Grammar Root |
|--------------|------|------------|--------------|
| SC-01 | escalation-spiral | Positive feedback amplifying deviation from equilibrium | collapse-cascade, MP-01 |
| SC-02 | institutional-erosion | Gradual decay of legitimacy, capacity, or trust | erosion, PO-01 |
| SC-03 | legitimacy-fracture | Sudden loss of authority basis | collapse, V-02 |
| SC-04 | technological-displacement | New technology obsoleting incumbent functions | substitution, TE-03, MP-04 |
| SC-05 | symbolic-inversion | Value hierarchies reversing | inversion, T-03 |
| SC-06 | dependency-trap | Lock-in creating fragility through reduced optionality | V-01, path-dependence |
| SC-07 | coordination-failure | Individual rationality producing collective irrationality | V-03 |
| SC-08 | power-realignment | Authority migrating between structural nodes | substitution-functional |
| SC-09 | fragmentation-cascade | Unity breaking into competing autonomous parts | fragmentation |
| SC-10 | emergence-window | Novel configuration creating temporary opportunity | emergence |

---

## 3. Action Posture Types

Strategic postures recommended under structural conditions:

| Posture ID | Name | Definition | When Applicable |
|------------|------|------------|-----------------|
| AP-01 | preserve-optionality | Maintain multiple paths; avoid irreversible commitments | Uncertainty high; structure unclear |
| AP-02 | decentralize-dependency | Reduce reliance on single nodes or institutions | SC-02, SC-03, SC-06 |
| AP-03 | build-asymmetric-skill | Develop capabilities with high upside, limited downside | SC-04, SC-10 |
| AP-04 | wait-for-confirmation | Delay action until institutional signals clarify | SC-08, high noise |
| AP-05 | move-before-normalization | Act early before new equilibrium locks in | SC-04, SC-10 |
| AP-06 | reduce-cascade-exposure | Exit positions vulnerable to contagion | SC-01, SC-07 |
| AP-07 | hedge-symbolic-position | Maintain credibility across potential value inversions | SC-05 |
| AP-08 | accept-strategic-loss | Recognize sunk costs; exit declining structures | SC-02, SC-03 |

---

## 4. Risk Posture Types

Postures for managing downside exposure:

| Risk ID | Name | Definition |
|---------|------|------------|
| RP-01 | fragility-aware | Acknowledge hidden dependencies; stress-test assumptions |
| RP-02 | tail-risk-conscious | Prepare for low-probability, high-impact scenarios |
| RP-03 | regime-shift-ready | Expect discontinuity; avoid linear extrapolation |
| RP-04 | noise-tolerant | Distinguish signal from noise; avoid overreaction |
| RP-05 | identity-decoupled | Separate self-worth from institutional affiliation |

---

## 5. Decision Signal Types

Observable indicators for monitoring scenario branches:

| Signal Type | Code | Description | Examples |
|-------------|------|-------------|----------|
| Institutional | SIG-I | Formal policy, law, or organizational change | Central bank rate decision, regulation announcement |
| Behavioral | SIG-B | Aggregate human action patterns | Capital flight, talent migration, enrollment decline |
| Rhetorical | SIG-R | Shift in official or elite discourse | Narrative change, framing reversal |
| Technical | SIG-T | System or infrastructure indicators | Liquidity metrics, network metrics, price signals |
| Symbolic | SIG-S | Public gestures, rituals, or status markers | Leadership change, ceremony modification |
| Temporal | SIG-X | Timing and sequencing patterns | Acceleration, delay, synchronization |

---

## 6. Anti-Pattern Categories

Common strategic mistakes inside structural conditions:

| Anti-Pattern ID | Name | Description | Typical Condition |
|-----------------|------|-------------|-------------------|
| ANT-01 | stability-illusion | Mistaking temporary stability for structural recovery | SC-02, SC-01 |
| ANT-02 | symbolism-confusion | Confusing symbolic gestures with actual power shifts | SC-05, SC-08 |
| ANT-03 | noise-overreaction | Responding to noise instead of structural signals | All conditions |
| ANT-04 | identity-lock | Tying identity to declining institution or paradigm | SC-02, SC-04 |
| ANT-05 | linear-extrapolation | Assuming continuation during regime shift | SC-04, SC-08 |
| ANT-06 | sunk-cost-trap | Continuing commitment due to past investment | SC-02, SC-06 |
| ANT-07 | crowd-following | Mimicking majority without structural understanding | SC-01, SC-07 |

---

## 7. Confidence Notation

Action outputs must include confidence qualifiers:

| Qualifier | Notation | Meaning |
|-----------|----------|---------|
| High structural clarity | `[conf:high]` | Pattern well-documented; multiple historical instances |
| Moderate clarity | `[conf:mid]` | Pattern recognized but context-dependent |
| Low clarity | `[conf:low]` | Structural reading uncertain; monitor closely |
| Speculative | `[conf:spec]` | Hypothesis only; insufficient evidence |

---

## 8. Action Grammar Rules

### Rule 1: Structure Before Event
Always identify structural condition before discussing specific events.

### Rule 2: Scenario Not Forecast
Branches are plausible directions, not predictions. Use "may", "tends to", "historically".

### Rule 3: Posture Not Command
Recommendations are orientations, not directives. User retains agency.

### Rule 4: Observable Signals Only
Decision signals must be concrete and verifiable, not abstract.

### Rule 5: Anti-Pattern Explicit
Always state what NOT to do, not just what to do.

### Rule 6: Domain Transferable
Action logic should apply across domains unless explicitly labeled otherwise.

---

## 9. Integration with OS Grammar

| OS Layer | Action Layer Use |
|----------|------------------|
| Grammar Types (erosion, collapse, etc.) | Maps to Structural Conditions |
| Mechanisms (C-01, T-01, etc.) | Informs scenario logic |
| Meta-Patterns (MP-01, etc.) | Provides historical trajectory reference |
| Archetypes (A01, etc.) | Classifies structural situation type |
| Stacks/Canons/Clusters | Pre-built structural templates for action translation |

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-08 | Initial grammar definition |
