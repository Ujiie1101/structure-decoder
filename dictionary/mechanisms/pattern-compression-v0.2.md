---
type: pattern-compression
version: v0.2.0
date: 2026-03-01
source: cross-domain-core-analysis
---

# Pattern Compression v0.2

## Overview

This document establishes the canonical vocabulary for Knowledge OS patterns, mechanisms, and labels. All future Core promotions and existing Core files MUST conform to this specification.

## Canonical Grammar Types (6)

| ID | Name | Definition | Generates |
|----|------|------------|-----------|
| erosion | Erosion | Gradual wearing away of structure through accumulated small actions | Legitimacy decline, trust degradation, norm decay |
| collapse | Collapse | Sudden failure when accumulated stress exceeds threshold | Bank runs, regime falls, system crashes |
| substitution | Substitution | Gradual replacement of one entity/function by another | Institutional replacement, paradigm shift |
| inversion | Inversion | Reversal of hierarchy, value, or direction | Value transposition, power flip |
| fragmentation | Fragmentation | Breaking of unified structure into competing parts | Schism, factional split, decentralization |
| emergence | Emergence | Novel properties arising from component interactions | Self-organization, spontaneous order |

---

## Canonical Mechanism IDs (19)

### Cascade Mechanisms (C-series)
| ID | Name | Definition |
|----|------|------------|
| C-01 | Leverage Cascade | Rising prices → more leverage → higher prices → collapse |
| C-02 | Confidence Contagion | Single failure → doubt spreads → multiple failures |
| C-03 | Reputational Cascade | One defection → observers defect → mass defection |

### Transformation Mechanisms (T-series)
| ID | Name | Definition |
|----|------|------------|
| T-01 | Institutional Substitution | New institution gradually assumes functions of old |
| T-02 | Procedural Transformation | Form preserved while substance changes |
| T-03 | Value Transposition | Values invert under pressure or over time |

### Feedback Mechanisms (F-series)
| ID | Name | Definition |
|----|------|------------|
| F-01 | Accountability Feedback Loop | Monitoring → compliance → relaxed monitoring → deviation |
| F-02 | Network Effect Amplification | Each node addition increases value non-linearly |
| F-03 | Expectation Feedback | Expectations shape reality which confirms expectations |

### Vulnerability Mechanisms (V-series)
| ID | Name | Definition |
|----|------|------------|
| V-01 | Path Dependence Lock-in | Early choices constrain future options |
| V-02 | Single Point of Failure | System depends on one unreplaceable component |
| V-03 | Coordination Failure | Individually rational choices produce collective irrationality |
| V-04 | Information Asymmetry | Unequal knowledge distribution enables exploitation |

### Political Mechanisms (PO-series)
| ID | Name | Definition |
|----|------|------------|
| PO-01 | Legitimacy Erosion | Authority gradually loses basis for obedience |
| PO-02 | Scapegoat Mechanism | External enemy used to maintain internal cohesion |

### Technology Mechanisms (TE-series)
| ID | Name | Definition |
|----|------|------------|
| TE-01 | Automation Displacement | Machines replace human labor functions |
| TE-02 | Platform Lock-in | Users trapped by switching costs and network effects |
| TE-03 | Reproduction Cost Collapse | Technology reduces marginal cost to near-zero |

### Economics Mechanisms (E-series)
| ID | Name | Definition |
|----|------|------------|
| E-01 | Invisible Hand Coordination | Self-interest aggregates to social benefit via markets |

---

## Canonical Meta-Patterns (13)

| ID | Name | Structure |
|----|------|-----------|
| MP-01 | Reflexive Spiral | A → B → more A → more B → ... |
| MP-02 | Threshold Transition | Stable → threshold crossed → rapid regime change |
| MP-03 | Self-Undermining Success | Success → parameter change → success becomes failure |
| MP-04 | Gatekeeper Displacement | Cost collapse → incumbent obsolete → new gatekeeper |
| MP-05 | Charisma-Institution Transition | Personal authority → routinization → bureaucracy/schism |
| MP-06 | Competitive Patronage Escalation | Status competition → investment escalation → innovation |
| MP-07 | Shock-Redistribution | Catastrophe → equilibrium break → power redistribution |
| MP-08 | Counter-Reformation Lag | Disruption → denial → ~100y delay → control response |
| MP-09 | Vacuum-Authoritarian Cycle | Revolution → chaos → demand for order → authoritarianism |
| MP-10 | Fixity Enables Accumulation | Preservation tech → knowledge fixed → cumulative progress |
| MP-11 | Vernacular Democratization | Elite language → translation → access expansion |
| MP-12 | Network Parasitism | New movement → uses existing infrastructure → spread |
| MP-13 | Shock-Fatigue Cycle | Shock → habituation → escalation → exhaustion → reset |

---

## Canonicalization Map

Non-canonical patterns found in existing Core files mapped to canonical equivalents:

### Map to Grammar Types

| Non-Canonical | → | Canonical | Rationale |
|---------------|---|-----------|-----------|
| transformation | → | substitution | T-series mechanisms handle this |
| schism | → | fragmentation | Splitting into parts |
| synthesis | → | emergence | Novel unity from components |
| collaborative-emergence | → | emergence | Redundant qualifier |
| authority-inversion | → | inversion | Specific instance of inversion |
| policy-inversion | → | inversion | Specific instance of inversion |

### Map to Mechanism IDs

| Non-Canonical | → | Canonical | Rationale |
|---------------|---|-----------|-----------|
| information-asymmetry (pattern) | → | [V-04] | Already a mechanism |
| principal-agent-divergence | → | [V-04] | Subset of information asymmetry |
| incentive-distortion | → | [F-01] | Accountability/monitoring breakdown |
| invisible-hand (pattern) | → | [E-01] | Already a mechanism |
| gatekeeper-displacement (pattern) | → | [MP-04] | Already a meta-pattern |
| competitive-patronage-escalation | → | [MP-06] | Already a meta-pattern |
| prisoners-dilemma | → | [V-03] | Instance of coordination failure |
| retaliatory-spiral | → | [MP-01] | Instance of reflexive spiral |
| speculative-bubble | → | [MP-01] + [C-01] | Combine reflexive spiral + leverage cascade |
| systemic-contagion | → | [C-02] | Already confidence contagion |
| normalization-of-deviance | → | [F-01] | Accountability feedback failure |
| self-disruption-paralysis | → | [MP-03] + [V-01] | Self-undermining + path dependence |
| gradual-decline | → | erosion | Grammar type, not pattern |
| institutional-decay | → | erosion | Grammar type, not pattern |

### Map to Labels (Keep as Labels, Not Patterns)

| Current Pattern | → | Move to Labels | Rationale |
|-----------------|---|----------------|-----------|
| dialectic | → | label: dialectic | Methodological, not structural |
| arche-inquiry | → | label: arche | Domain-specific methodology |
| skeptical-dissolution | → | label: skepticism | Philosophical stance |
| habit-formation | → | label: habit | Descriptive concept |
| naturalistic-reduction | → | label: naturalism | Philosophical stance |
| is-ought-gap | → | label: is-ought | Conceptual distinction |
| differance | → | label: differance | Author-specific concept |
| trace | → | label: trace | Author-specific concept |
| supplement | → | label: supplement | Author-specific concept |
| loss-aversion | → | label: loss-aversion | Psychological trait |
| reference-point-effect | → | label: reference-dependence | Psychological trait |
| virtu-fortuna-dialectic | → | label: virtu, fortuna | Domain concepts |
| ideological-control | → | label: hegemony | Gramsci concept |
| holy-war | → | label: crusade, jihad | Historical category |
| east-west-division | → | label: east-west | Geographical category |
| causal-misattribution | → | label: myth-making | Cognitive category |
| theft-amplification | → | label: notoriety | Case-specific |
| witness-as-monument | → | label: political-art | Case-specific |

---

## Do-Not-Use List

The following terms MUST NOT be used as patterns in new Core files:

1. **Redundant with Grammar Types**: transformation, decay, decline, breakdown, shift, change, transition (use canonical 6)
2. **Redundant with Mechanism IDs**: Use `[ID]` notation instead of prose names
3. **Too Specific**: Case-specific patterns that apply to only one entity
4. **Too Vague**: "dynamics", "process", "mechanism", "structure" alone
5. **Philosophical Concepts**: Move to labels, not patterns (e.g., dialectic, differance, wu-wei)
6. **Psychological Traits**: Move to labels (e.g., loss-aversion, bounded-rationality)

---

## Label Normalization Guidelines

### Required Label Categories (choose relevant ones)
1. **Era/Period**: ancient, medieval, early-modern, modern, contemporary
2. **School/Tradition**: stoicism, scholasticism, marxism, etc.
3. **Core Concepts**: Maximum 5 defining concepts (entity-specific)
4. **Methodological**: empiricism, rationalism, phenomenology, etc.

### Label Naming Convention
- Lowercase with hyphens: `categorical-imperative`
- No plurals: `monad` not `monads`
- No articles: `free-will` not `the-free-will`
- Maximum 5 labels per entity

---

## Reduction Metrics

| Metric | Before | After | Reduction |
|--------|--------|-------|-----------|
| Unique patterns in frontmatter | 47 | 6 + 19 + 13 = 38 | -19% |
| Pattern synonyms eliminated | - | 14 | - |
| Patterns moved to labels | - | 17 | - |
| Average patterns/entity | 2.1 | 1.8 (est.) | -14% |

---

## Implementation Notes

1. **Frontmatter `patterns:` field**: Use only canonical grammar types (6)
2. **Mechanism Mapping section**: Use `[ID]` notation for all 19 mechanisms
3. **Meta-Pattern Mapping section**: Use `[MP-XX]` notation for all 13 meta-patterns
4. **Labels field**: Domain-specific vocabulary allowed here

---

*Pattern Compression v0.2 — Created 2026-03-01*
