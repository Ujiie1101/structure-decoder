---
type: intervention-registry
version: v1.0
date: 2026-03-06
intervention_count: 10
categories: [institutional, economic, technological, narrative]
output: 135_Meta/intervention-scenarios/
engine: scripts/intervention_simulation.py
---

# Intervention Registry v1.0

Canonical registry of structural interventions for Knowledge OS simulation engine.

---

## Schema

Each intervention defines:
- **intervention_id**: Unique ID (I01-I99)
- **name**: kebab-case identifier
- **type**: institutional | economic | technological | narrative
- **definition**: Mechanism-focused description
- **target_patterns**: Primary patterns affected
- **expected_effects**: Intended structural changes
- **risk_effects**: Unintended structural risks
- **state_bias**: Civilization loop state transition effects
- **historical_examples**: Known precedents

---

## Registry

### I01 | Regulatory Tightening

| Field | Value |
|-------|-------|
| intervention_id | I01 |
| name | regulatory-tightening |
| type | institutional |
| definition | Increasing regulatory oversight, compliance requirements, and enforcement mechanisms to constrain undesired behaviors |
| target_patterns | `[collapse, fragmentation, erosion]` |
| expected_effects | Reduce systemic risk, increase stability, prevent collapse cascade |
| risk_effects | Innovation suppression, institutional rigidity, compliance overhead |
| state_bias | `{S3→S2: +0.20, S3→S4: -0.15, erosion→stability: +0.15}` |
| historical_examples | Dodd-Frank Act (2010), Sarbanes-Oxley (2002), Glass-Steagall (1933) |

---

### I02 | Deregulation

| Field | Value |
|-------|-------|
| intervention_id | I02 |
| name | deregulation |
| type | institutional |
| definition | Reducing regulatory constraints to enable market freedom and innovation |
| target_patterns | `[emergence, substitution]` |
| expected_effects | Accelerate innovation, increase competition, enable new entrants |
| risk_effects | Systemic risk accumulation, erosion of safeguards, collapse vulnerability |
| state_bias | `{stability→emergence: +0.25, erosion→collapse: +0.15}` |
| historical_examples | Reagan deregulation (1980s), UK Big Bang (1986), Airline Deregulation (1978) |

---

### I03 | Centralization

| Field | Value |
|-------|-------|
| intervention_id | I03 |
| name | centralization |
| type | institutional |
| definition | Consolidating decision-making authority and control into fewer nodes |
| target_patterns | `[fragmentation, substitution]` |
| expected_effects | Reduce coordination costs, increase efficiency, enable rapid response |
| risk_effects | Single point of failure, reduced resilience, power concentration |
| state_bias | `{fragmentation→substitution: +0.20, stability→erosion: +0.10}` |
| historical_examples | EU integration, Federal Reserve creation, Chinese SOE consolidation |

---

### I04 | Decentralization

| Field | Value |
|-------|-------|
| intervention_id | I04 |
| name | decentralization |
| type | institutional |
| definition | Distributing authority and control across multiple autonomous nodes |
| target_patterns | `[fragmentation, emergence]` |
| expected_effects | Increase resilience, enable local adaptation, reduce single points of failure |
| risk_effects | Coordination failure, inconsistency, reduced economies of scale |
| state_bias | `{substitution→fragmentation: +0.15, collapse→emergence: +0.10}` |
| historical_examples | Blockchain adoption, EU subsidiarity, US federalism |

---

### I05 | Technology Adoption

| Field | Value |
|-------|-------|
| intervention_id | I05 |
| name | technology-adoption |
| type | technological |
| definition | Accelerating deployment and integration of new technological capabilities |
| target_patterns | `[emergence, substitution]` |
| expected_effects | Productivity gains, capability expansion, competitive advantage |
| risk_effects | Disruption of existing systems, skill gaps, dependency risks |
| state_bias | `{stability→emergence: +0.30, substitution→stabilization: +0.15}` |
| historical_examples | Internet adoption (1990s), Mobile revolution, AI integration |

---

### I06 | Technology Restriction

| Field | Value |
|-------|-------|
| intervention_id | I06 |
| name | technology-restriction |
| type | technological |
| definition | Limiting deployment, access, or development of specific technologies |
| target_patterns | `[emergence, substitution]` |
| expected_effects | Risk mitigation, maintain existing structures, security preservation |
| risk_effects | Innovation suppression, competitive disadvantage, black markets |
| state_bias | `{emergence→stability: +0.20, emergence→substitution: -0.25}` |
| historical_examples | COCOM export controls, Nuclear non-proliferation, AI moratoriums |

---

### I07 | Subsidy Expansion

| Field | Value |
|-------|-------|
| intervention_id | I07 |
| name | subsidy-expansion |
| type | economic |
| definition | Increasing government financial support for specific sectors or activities |
| target_patterns | `[erosion, collapse]` |
| expected_effects | Stabilize struggling sectors, maintain employment, support transition |
| risk_effects | Market distortion, moral hazard, fiscal burden, zombie firms |
| state_bias | `{erosion→stability: +0.20, collapse→substitution: +0.10}` |
| historical_examples | Agricultural subsidies, Green energy incentives, COVID relief programs |

---

### I08 | Tariff Escalation

| Field | Value |
|-------|-------|
| intervention_id | I08 |
| name | tariff-escalation |
| type | economic |
| definition | Increasing import duties and trade barriers to protect domestic industries |
| target_patterns | `[substitution, fragmentation]` |
| expected_effects | Protect domestic industry, reduce import dependency, increase self-sufficiency |
| risk_effects | Trade wars, retaliatory measures, reduced efficiency, consumer costs |
| state_bias | `{substitution→fragmentation: +0.20, stability→erosion: +0.15}` |
| historical_examples | Smoot-Hawley (1930), US-China trade war, Brexit trade barriers |

---

### I09 | Narrative Integration

| Field | Value |
|-------|-------|
| intervention_id | I09 |
| name | narrative-integration |
| type | narrative |
| definition | Constructing and propagating unifying narratives to build social cohesion |
| target_patterns | `[fragmentation, inversion]` |
| expected_effects | Increase social cohesion, reduce conflict, build legitimacy |
| risk_effects | Propaganda risks, suppression of dissent, reality distortion |
| state_bias | `{fragmentation→substitution: +0.15, inversion→stability: +0.20}` |
| historical_examples | New Deal rhetoric, EU founding myths, Post-war reconstruction narratives |

---

### I10 | Legitimacy Reconstruction

| Field | Value |
|-------|-------|
| intervention_id | I10 |
| name | legitimacy-reconstruction |
| type | narrative |
| definition | Rebuilding institutional trust through transparency, accountability, and reform |
| target_patterns | `[erosion, collapse]` |
| expected_effects | Restore trust, rebuild institutions, stabilize social contract |
| risk_effects | Slow process, incomplete reforms, cynicism if perceived as performative |
| state_bias | `{erosion→stability: +0.25, collapse→substitution: +0.15}` |
| historical_examples | Post-Watergate reforms, Post-2008 financial reforms, Truth commissions |

---

## Summary Table

| ID | Name | Type | Target Patterns | Primary Effect |
|----|------|------|-----------------|----------------|
| I01 | regulatory-tightening | institutional | collapse, fragmentation | Stabilization |
| I02 | deregulation | institutional | emergence, substitution | Innovation |
| I03 | centralization | institutional | fragmentation | Efficiency |
| I04 | decentralization | institutional | fragmentation, emergence | Resilience |
| I05 | technology-adoption | technological | emergence, substitution | Transformation |
| I06 | technology-restriction | technological | emergence | Preservation |
| I07 | subsidy-expansion | economic | erosion, collapse | Support |
| I08 | tariff-escalation | economic | substitution, fragmentation | Protection |
| I09 | narrative-integration | narrative | fragmentation, inversion | Cohesion |
| I10 | legitimacy-reconstruction | narrative | erosion, collapse | Trust |

---

## Validation Rules

1. `intervention_id` must be unique (I01-I99)
2. `type` must be: institutional, economic, technological, or narrative
3. `target_patterns` must use core grammar only
4. `state_bias` transitions must reference valid loop states
5. `historical_examples` should have ≥2 instances

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2026-03-06 | Initial registry; 10 interventions |
