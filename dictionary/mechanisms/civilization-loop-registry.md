---
type: civilization-loop-registry
version: v1.0
date: 2026-03-05
state_count: 6
transition_count: 15
meta_pattern_mappings: 6
---

# Civilization Loop Registry v1.0

Deterministic state-machine registry for civilization dynamics.
Maps meta-pattern events to state transitions.

---

## State Model

Six civilization states, aligned to dominant meta-patterns:

| State ID | Name | Mechanism Definition |
|----------|------|----------------------|
| S0 | baseline | Default stable equilibrium. No dominant meta-pattern active. System maintains inertia with gradual micro-changes. Entry point for all timelines. |
| S1 | innovation | Paradigm displacement active. Novel structures emerge and replace incumbent frameworks. High dynamism, rapid adoption cycles, creative destruction operating. |
| S2 | lock-in | Institutional consolidation complete. Path dependency established. Resistance to change increases. Innovation slows as dominant paradigm crystallizes. |
| S3 | decay | Gradual erosion underway. Accumulated structural weaknesses. Legitimacy or capacity declining without acute crisis. Slow-motion deterioration. |
| S4 | crisis | Cascade failure triggered. Systemic instability. Multiple interconnected failures. Acute stress, potential for collapse or transformation. |
| S5 | transformation | Crisis-driven reorganization active. Failed components replaced. New institutional arrangements emerging. Post-crisis restructuring. |

---

## Transition Graph

Allowed state transitions with rule conditions:

| From | To | Transition ID | Rule Condition |
|------|-----|---------------|----------------|
| S0 | S1 | T01 | M01 count >= 2 in window |
| S0 | S2 | T02 | M08 count >= 2 in window |
| S0 | S3 | T03 | M06 count >= 2 in window |
| S1 | S0 | T04 | No M01 in last 3 events |
| S1 | S2 | T05 | M08 count >= 1 AND M01 decreasing |
| S1 | S4 | T06 | M03 count >= 2 (innovation overload) |
| S2 | S0 | T07 | No M08 in last 5 events |
| S2 | S3 | T08 | M06 count >= 1 (locked systems decay) |
| S2 | S4 | T09 | M03 count >= 2 (locked system shock) |
| S3 | S0 | T10 | No M06 in last 5 events |
| S3 | S4 | T11 | M03 count >= 1 OR M06 count >= 3 (decay → crisis) |
| S3 | S5 | T12 | M02 count >= 1 (managed transformation) |
| S4 | S0 | T13 | No M03 in last 5 events (recovery) |
| S4 | S5 | T14 | M02 count >= 1 (crisis triggers transformation) |
| S5 | S0 | T15 | No M02 in last 3 events (stabilization) |
| S5 | S1 | T16 | M01 count >= 2 (transformation enables innovation) |

---

## Meta-Pattern → State Impact Mapping

Each meta-pattern contributes scores to states:

### M01 | paradigm-displacement
```yaml
state_enter:
  - S1: +2.0  # Strong innovation signal
state_stay:
  - S1: +1.0  # Reinforces innovation
state_exit:
  - S2: -0.5  # Weakens lock-in
  - S0: -0.3  # Destabilizes baseline
accelerant: false
```

### M02 | crisis-driven-transformation
```yaml
state_enter:
  - S5: +2.0  # Strong transformation signal
state_stay:
  - S5: +1.0  # Reinforces transformation
state_exit:
  - S4: +0.5  # Can emerge from crisis
  - S3: +0.5  # Can emerge from decay
accelerant: false
```

### M03 | cascade-failure
```yaml
state_enter:
  - S4: +2.5  # Very strong crisis signal
state_stay:
  - S4: +1.5  # Reinforces crisis
state_exit:
  - S0: -1.0  # Strongly destabilizes baseline
  - S1: -0.5  # Disrupts innovation
  - S2: -0.5  # Breaks lock-in
accelerant: false
```

### M04 | value-inversion
```yaml
state_enter: {}  # No direct state entry
state_stay: {}   # No direct state reinforcement
state_exit: {}   # No direct state exit
accelerant: true
accelerant_effect:
  - all_transitions: +0.3  # Speeds any transition
  - S1_enter: +0.5  # Particularly speeds innovation entry
  - S4_enter: +0.5  # Particularly speeds crisis entry
```

### M06 | gradual-decay-cycle
```yaml
state_enter:
  - S3: +2.0  # Strong decay signal
state_stay:
  - S3: +1.0  # Reinforces decay
state_exit:
  - S0: -0.3  # Weakens baseline
  - S2: +0.3  # Can follow lock-in
accelerant: false
```

### M08 | institutional-lock-in
```yaml
state_enter:
  - S2: +2.0  # Strong lock-in signal
state_stay:
  - S2: +1.0  # Reinforces lock-in
state_exit:
  - S1: -0.5  # Suppresses innovation
  - S0: +0.3  # Stabilizes toward baseline
accelerant: false
```

---

## Secondary Meta-Patterns (Lower Frequency)

These meta-patterns have fewer assignments but still contribute:

### M05 | revolutionary-dissolution
```yaml
state_enter:
  - S4: +1.5  # Crisis-adjacent
  - S5: +1.0  # Transformation-adjacent
state_stay:
  - S5: +0.5
state_exit: {}
accelerant: false
```

### M10 | fragmentation-without-recovery
```yaml
state_enter:
  - S4: +1.0  # Crisis signal
  - S3: +0.5  # Decay signal
state_stay:
  - S4: +0.5
state_exit:
  - S0: -0.5  # Hard recovery
accelerant: false
```

### M11 | emergence-proliferation
```yaml
state_enter:
  - S1: +1.5  # Innovation-adjacent
state_stay:
  - S1: +0.5
state_exit: {}
accelerant: false
```

---

## Scoring Parameters

Default parameters for state inference:

| Parameter | Default | Description |
|-----------|---------|-------------|
| window_size | 10 | Rolling event window |
| threshold | 0.15 | Confidence threshold for transitions |
| min_events | 5 | Minimum events before inference |
| decay_rate | 0.1 | Linear decay per position from most recent |
| epsilon | 0.001 | Smoothing constant |

---

## State Transition Diagram

```
                    ┌─────────────────────────┐
                    │                         │
                    ▼                         │
    ┌───────┐     ┌───────┐     ┌───────┐   │
    │  S0   │────▶│  S1   │────▶│  S2   │───┤
    │baseline│◀────│innov. │◀────│lock-in│   │
    └───────┘     └───────┘     └───────┘   │
        │             │             │        │
        │             │             │        │
        ▼             │             ▼        │
    ┌───────┐         │         ┌───────┐   │
    │  S3   │◀────────┴────────▶│  S4   │◀──┘
    │ decay │                   │crisis │
    └───────┘                   └───────┘
        │                           │
        │         ┌───────┐         │
        └────────▶│  S5   │◀────────┘
                  │transf.│
                  └───────┘
                      │
                      ▼
                  (back to S0 or S1)
```

---

## Generation

```bash
# Manual creation
# Updated by: civilization_loop.py validate
```
