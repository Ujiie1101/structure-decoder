---
type: mechanism-index
version: v0.2.1
date: 2026-02-25
source_files: 55
---

# Mechanism Index v0.2.0

## Purpose

This index tracks mechanism usage across 120_Core files to:
1. Identify high-utility mechanisms (frequently applied)
2. Detect under-utilized mechanisms (may need refinement or removal)
3. Guide disambiguation between similar mechanisms
4. Provide quick lookup for representative examples

---

## Core Mechanisms Usage

| ID | Name | Count | Top 3 Entities | Closest Neighbor |
|----|------|-------|----------------|------------------|
| **V-02** | Policy Constraint Lock-in | 22 | ltcm, asian-crisis, enron, shock-therapy, neoliberalism | V-04 (opacity vs. rigidity) |
| **C-02** | Confidence Contagion | 20 | ltcm, asian-crisis, arab-spring, rwandan-genocide | C-01 (belief vs. forced) |
| **T-02** | Procedural Transformation | 18 | fascism, cultural-revolution, neoliberalism, populism | T-01 (rules vs. functions) |
| **F-02** | Network Effect Amplification | 16 | arab-spring, solidarity-poland, dot-com-bubble, populism | F-01 (network vs. evaluation) |
| **C-01** | Leverage Cascade | 13 | ltcm, asian-crisis, russian-revolution, arab-spring | C-02 (forced vs. belief-driven) |
| **V-01** | Overextension-Fragmentation | 13 | soviet-collapse, arab-spring, fascism, russian-revolution | V-03 (span vs. loyalty) |
| **F-01** | Accountability Feedback Loop | 12 | democracy, classical-economics, neoliberalism | F-02 (evaluation vs. network) |
| **T-01** | Institutional Substitution | 11 | fall-of-roman-empire, solidarity-poland, early-christianity | T-03 (gradual vs. explicit alliance) |
| **TE-02** | Protocol Layering | 10 | internet-emergence, printing-revolution, parmenides | V-04 (clarifies vs. obscures) |
| **PO-02** | Onion Layering | 9 | enron, ftx, fascism, one-party-state, rwandan-genocide | PO-01 (structure vs. atomization) |
| **PO-01** | Atomization-Capture | 9 | cultural-revolution, fascism, populism, rwandan-genocide | PO-02 (precondition vs. structure) |
| **E-01** | Invisible Hand Coordination | 9 | classical-economics, neoliberalism, thales | F-01 (signal type differs) |
| **F-03** | Debt-Deflation Spiral | 7 | ltcm, asian-crisis, european-debt-crisis, zimbabwe | C-01 (debt-specific vs. general leverage) |
| **C-03** | Retaliation Cascade | 6 | european-debt-crisis, cultural-revolution, rwandan-genocide | C-01/C-02 (intentional vs. automatic) |
| **TE-03** | Reproduction Cost Collapse | 6 | printing-revolution, industrial-revolution, neoliberalism | TE-02 (production vs. organization) |
| **V-04** | Risk Opacity Amplification | 5 | ltcm, enron, ftx, financial-deregulation | TE-02 (obscures vs. clarifies) |
| **V-03** | Mercenary Loyalty Degradation | 5 | soviet-collapse, ftx, russian-revolution | V-01 (loyalty vs. span) |
| **T-03** | State Co-optation | 5 | fascism, one-party-state, early-christianity | T-01 (explicit alliance vs. gradual) |
| **TE-01** | End-to-End Principle | 3 | internet-emergence, anaximander, anaxagoras | TE-02 (architecture principle vs. layering) |

---

## Meta-Patterns Usage

| ID | Name | Count | Top 3 Entities | Closest Neighbor |
|----|------|-------|----------------|------------------|
| **MP-01** | Reflexive Spiral | 21 | ltcm, cultural-revolution, fascism, rwandan-genocide | MP-03 (amplification vs. undermining) |
| **MP-02** | Threshold Transition | 21 | arab-spring, soviet-collapse, russian-revolution, rwandan-genocide | MP-09 (transition type differs) |
| **MP-03** | Self-Undermining Success | 20 | ltcm, enron, ftx, soviet-collapse, one-party-state | MP-01 (success-failure vs. spiral) |
| **MP-07** | Shock-Redistribution | 10 | shock-therapy, russian-revolution, solidarity-poland, rwandan-genocide | MP-09 (redistribution vs. vacuum) |
| **MP-04** | Gatekeeper Displacement | 9 | populism, neoliberalism, printing-revolution | MP-11 (gatekeeping vs. language) |
| **MP-12** | Network Parasitism | 7 | arab-spring, solidarity-poland, early-christianity | T-01 (parasitism vs. substitution) |
| **MP-09** | Vacuum-Authoritarian Cycle | 6 | russian-revolution, fascism, one-party-state | MP-07 (vacuum vs. redistribution) |
| **MP-05** | Charisma-Institution Transition | 6 | one-party-state, early-christianity, early-buddhism | MP-04 (founder vs. gatekeeper) |
| **MP-10** | Fixity Enables Accumulation | 5 | printing-revolution, internet-emergence, parmenides | MP-11 (preservation vs. access) |
| **MP-11** | Vernacular Democratization | 4 | printing-revolution, early-buddhism, nationalism | MP-04 (language vs. gatekeeping) |
| **MP-06** | Competitive Patronage Escalation | 6 | baroque, vc-ecosystem, tech-talent, university-rankings, cold-war, renaissance | MP-07 (competition vs. shock) |
| **MP-08** | Counter-Reformation Lag | 4 | baroque, financial-deregulation, neoliberalism, keynesian-economics | MP-02 (lag vs. threshold) |
| **MP-13** | Shock-Fatigue Cycle | 4 | baroque, dot-com-bubble, populism, modernism | MP-01 (attention decay vs. amplification) |

---

## Disambiguation Rules

### Cascade Family (C-01, C-02, C-03)

| Mechanism | Trigger Type | Propagation | Key Question |
|-----------|--------------|-------------|--------------|
| C-01 Leverage | Forced liquidation | Automatic (margin) | Is there mechanical forcing? |
| C-02 Confidence | Belief shift | Information cascade | Is trust the variable? |
| C-03 Retaliation | Intentional response | Symmetric counter | Is response deliberate? |

**Rule**: If actors are forced by position (debt, margin), use C-01. If actors respond to beliefs about others, use C-02. If actors deliberately retaliate, use C-03.

### Transformation Family (T-01, T-02, T-03)

| Mechanism | Nature | Relationship | Key Question |
|-----------|--------|--------------|--------------|
| T-01 Substitution | Gradual, implicit | Function transfer | Is handover formal? |
| T-02 Procedural | Rule change | Power shift via rules | Are rules the lever? |
| T-03 Co-optation | Alliance, explicit | Trade autonomy for resources | Is there explicit alliance? |

**Rule**: If function transfers without formal agreement, use T-01. If power shifts through rule modification, use T-02. If movement allies with state, use T-03.

### Feedback Family (F-01, F-02, F-03)

| Mechanism | Signal Type | Direction | Key Question |
|-----------|-------------|-----------|--------------|
| F-01 Accountability | Evaluation signal | Discipline behavior | Is there periodic evaluation? |
| F-02 Network | Value scaling | Adoption accelerates | Does value scale with users? |
| F-03 Debt-Deflation | Price-debt | Debt burden amplifies | Is debt burden increasing? |

**Rule**: If periodic judgment disciplines, use F-01. If network value scales superlinearly, use F-02. If deflation increases real debt, use F-03.

### Vulnerability Family (V-01, V-02, V-03, V-04)

| Mechanism | Failure Mode | Key Question |
|-----------|--------------|--------------|
| V-01 Overextension | Coordination capacity exceeded | Is span too large? |
| V-02 Lock-in | Prior commitment blocks adaptation | Is orthodoxy preventing change? |
| V-03 Mercenary | Extrinsic loyalty enables defection | Are contractors defecting? |
| V-04 Opacity | Layered structure obscures risk | Is risk hidden by structure? |

**Rule**: If coordination span exceeds capacity, use V-01. If commitment blocks adaptation, use V-02. If contractors defect, use V-03. If structure hides risk, use V-04.

### V-04 vs TE-02 Distinction

This is the most critical disambiguation:

| Criterion | TE-02 Protocol Layering | V-04 Risk Opacity |
|-----------|-------------------------|-------------------|
| **Function** | Separates concerns | Obscures dependencies |
| **Direction** | Abstraction clarifies | Abstraction confuses |
| **Outcome** | Coordination improved | Risk mispriced |
| **Design** | Intentional separation | Often unintentional |

**Rule**: If layers enable independent evolution and clarify interfaces, use TE-02. If layers prevent accurate risk assessment, use V-04.

### PO-01 vs PO-02 Relationship

PO-01 (Atomization-Capture) is often a **precondition** for PO-02 (Onion Layering).
- Use PO-01 when analyzing how isolated individuals become susceptible
- Use PO-02 when analyzing organizational structure with concentric layers
- When both present (e.g., totalitarianism), map both

### MP-01 vs MP-03 Distinction

| Pattern | Structure | Endpoint |
|---------|-----------|----------|
| MP-01 Reflexive Spiral | A → B → more A | External stop or exhaustion |
| MP-03 Self-Undermining | Success → condition change → failure | Success creates own failure |

**Rule**: If feedback amplifies indefinitely until external intervention, use MP-01. If success itself changes conditions leading to failure, use MP-03.

### MP-13 vs MP-01 Distinction

| Pattern | What Changes | Direction |
|---------|--------------|-----------|
| MP-01 Reflexive Spiral | System variable (leverage, terror) | Amplification |
| MP-13 Shock-Fatigue | Audience capacity (attention, shock response) | Exhaustion |

**Rule**: If the mechanism amplifies a system variable, use MP-01. If the mechanism depletes audience capacity requiring escalation, use MP-13.

---

## Under-Utilized Mechanisms (Watch List)

Mechanisms with count ≤ 3 may need:
1. More entity coverage to validate
2. Refinement to increase applicability
3. Potential merge with related mechanism

| ID | Count | Status | Next Action |
|----|-------|--------|-------------|
| TE-01 | 3 | LOW | Target more Technology entities |

**Previously underused, now validated (v0.2.1):**
- **MP-06 (1→6)**: Validated via baroque, vc-ecosystem, tech-talent, university-rankings, cold-war
- MP-08 (1→4): Validated via baroque, financial-deregulation, neoliberalism
- MP-13 (1→4): Validated via baroque, dot-com-bubble, populism
- V-04 (1→5): Validated via LTCM, Enron, FTX, financial-deregulation
- PO-01 (1→9): Validated via cultural-revolution, fascism, populism, rwandan-genocide
- V-03 (2→5): Validated via soviet-collapse, ftx, russian-revolution

---

## High-Utility Mechanisms (Stable Core)

Mechanisms with count ≥ 10 are well-validated and stable:

| ID | Count | Domains Used | Status |
|----|-------|--------------|--------|
| V-02 Policy Constraint Lock-in | 22 | Phil, Hist, Econ, Pol | STABLE |
| C-02 Confidence Contagion | 20 | Econ, Pol, Hist | STABLE |
| T-02 Procedural Transformation | 18 | Phil, Hist, Rel, Econ, Pol | STABLE |
| F-02 Network Effect Amplification | 16 | Phil, Hist, Rel, Econ, Pol, Tech, Art | STABLE |
| C-01 Leverage Cascade | 13 | Hist, Econ, Pol | STABLE |
| V-01 Overextension-Fragmentation | 13 | Hist, Econ, Pol | STABLE |
| F-01 Accountability Feedback Loop | 12 | Phil, Rel, Econ, Pol | STABLE |
| T-01 Institutional Substitution | 11 | Phil, Hist, Rel, Pol, Tech, Art | STABLE |
| TE-02 Protocol Layering | 10 | Phil, Rel, Econ, Pol, Tech | STABLE |

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| v0.1.1 | 2026-02-25 | Initial index from 30 Core files. Added V-04 and MP-13 from proposed-additions-review. |
| v0.2.0 | 2026-02-25 | Updated from 50 Core files (+20 Economics/Politics). V-04, PO-01, V-03, F-03, C-03 now validated. MP-06 still underused. |
| v0.2.1 | 2026-02-25 | MP-06 independence test completed. Added 4 MP-06 target entities (baroque, vc-ecosystem, tech-talent, university-rankings) + Cold War update. MP-06 now validated (1→6). 55 total Core files. |

---

*End of Mechanism Index v0.2.1*
