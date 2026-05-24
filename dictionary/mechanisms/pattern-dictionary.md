---
type: pattern-dictionary
version: v0.4.0
date: 2026-03-20
mechanism_count: 23
collapse_subtypes: 2
substitution_subtypes: 3
grammar_type_count: 6
meta_pattern_count: 22
stack_count: 2
canon_count: 5
cluster_count: 4
source: pattern-compression-v0.2 + structural-analysis-177
---

# Pattern Dictionary v0.2.0

## Quick Reference

**Canonical Grammar Types (use in frontmatter `patterns:` field):**
- `erosion` — gradual wearing away of structure
- `collapse` — sudden failure when threshold exceeded
  - `collapse-cascade` — rapid threshold breach with self-amplifying failure propagation
  - `collapse-erosion` — prolonged decay until symbolic/structural disintegration
- `substitution` — gradual replacement of entity/function
  - `substitution-category` — foundational organizing framework replaced
  - `substitution-functional` — operational authority shifts between nodes
  - `substitution-scarcity` — value/scarcity locus shifts to new domain
- `inversion` — reversal of hierarchy, value, or direction
- `fragmentation` — breaking of unity into parts
- `emergence` — novel properties from component interactions

**Collapse Archetypes (refinement of `collapse` grammar):**
- See `040_OS/collapse-archetypes.md` for collapse spectrum model

**Substitution Archetypes (refinement of `substitution` grammar):**
- See `040_OS/substitution-archetypes.md` for substitution spectrum model

**Mechanism IDs (use in body text with `[ID]` notation):**
- Cascade: C-01, C-02, C-03, C-04
- Transformation: T-01, T-02, T-03, T-04
- Feedback: F-01, F-02, F-03
- Vulnerability: V-01, V-02, V-03, V-04, V-05
- Political: PO-01, PO-02
- Technology: TE-01, TE-02, TE-03
- Economics: E-01, E-02

**Meta-Patterns (use in body text with `[MP-XX]` notation):**
- See `040_OS/meta-patterns.md` for MP-01 through MP-22
- MP-14 to MP-19: Discovered patterns from gap analysis (2026-03-15)
- MP-20: Game Layer Migration — competitive advantage shifts to higher abstraction layer (2026-03-18)
- MP-21: Asymmetric Dependency — build-up slow, breakdown fast, rebuild incomplete (2026-03-20)
- MP-22: Overextension Layer Lock-in — winning at Layer N blocks migration to Layer N+1 (2026-03-25)

**Canonicalization:**
- See `040_OS/pattern-compression-v0.2.md` for synonym mapping and do-not-use list

**Pattern Stacks (STACK-XX):**
- See `040_OS/pattern-stacks.md` for stack registry
- STACK-01: Threshold-Displacement-Substitution (MP-02 + MP-04 + T-01)
- STACK-02: Crisis-Cascade (MP-01 + V-02 + C-01)

**Canon Patterns (CANON-XX):**
- See `040_OS/pattern-canon-v1.md` for full definitions
- CANON-01: Innovation-Displacement (E-01 → MP-04 → T-01)
- CANON-02: Reflexive-Crisis (V-02 → MP-01 → C-01/C-02 → MP-03)
- CANON-03: Paradigm-Transformation (MP-02 → T-02 → MP-04)
- CANON-04: Technology-Stack (TE-02 → F-02 → TE-03 → T-01)
- CANON-05: Empire-Decline (V-01 → T-01 → C-03)

**Canonical Clusters (CLUSTER-XX):**
- See `040_OS/crisis-cascade.md` for crisis cluster
- CLUSTER-CRISIS: Financial crisis dynamics (V-02 + MP-01 + C-01/C-02)
- CLUSTER-REVOLUTION: Political revolution dynamics (V-01/V-02 + C-02 + MP-02 + T-01)
- CLUSTER-TECH_SHIFT: Technology paradigm shifts (TE-02/TE-03 + F-02 + MP-04 + T-01)
- CLUSTER-EMPIRE: Empire formation/decline (V-01 + V-03 + T-01)

**Operational Files:**
- `040_OS/grammar-distribution.md` — Grammar type frequencies + phase estimator
- `040_OS/transfer-graph.md` — Cross-domain transfer weights

---

## Usage

Each mechanism entry follows OS grammar:
- **ID**: Unique identifier for cross-reference
- **Definition**: Category-neutral, reusable across domains
- **Activation Conditions**: When the mechanism triggers
- **Observable Proxies**: Measurable indicators
- **Failure/Inversion**: When the mechanism breaks or reverses
- **Synonyms**: Acceptable alternative terms
- **Exclusions**: What this mechanism is NOT

---

## CASCADE MECHANISMS

### C-01 | Leverage Cascade

**Definition**
An initial shock triggers forced liquidation among leveraged actors, causing price decline, which triggers further liquidation. The feedback loop amplifies exponentially until external intervention or exhaustion of leveraged positions.

**Activation Conditions**
- High leverage ratios (debt-to-equity > 3:1 or margin > 40%)
- Correlated positions across multiple actors
- Mark-to-market accounting or margin call requirements
- Limited circuit breakers or cooling-off periods

**Observable Proxies**
- Margin call volume spike
- Bid-ask spread widening
- Forced liquidation filings
- Correlation breakdown in previously uncorrelated assets
- Volatility index surge

**Failure/Inversion Conditions**
- Central bank liquidity injection (lender of last resort)
- Trading halts or circuit breakers
- Coordinated bailout of leveraged entities
- Leverage caps preventing initial buildup

**Common Synonyms**
- Margin spiral
- Deleveraging cascade
- Fire sale contagion
- Forced selling loop

**Exclusions / Non-examples**
- Gradual price decline without forced selling (normal correction)
- Single actor default without systemic propagation
- Panic without leverage (pure confidence loss = C-02)

**Example Instances**
1. Great Depression 1929: 300M shares on 40-50% margin; margin calls forced liquidation
2. GFC 2008: Repo haircuts jumped from near-zero to 40%+; forced asset sales
3. Roman Empire: Fiscal extraction exceeded regeneration; taxation "cascade" depleted base

---

### C-02 | Confidence Contagion

**Definition**
Loss of trust in one institution propagates to structurally similar institutions through information cascades and self-fulfilling expectations. Actors withdraw resources preemptively, causing the feared outcome.

**Activation Conditions**
- High interconnection or perceived similarity between institutions
- Information asymmetry (actors cannot distinguish solvent from insolvent)
- First-mover advantage in withdrawal (early exiters protected)
- Absence of credible insurance or guarantee

**Observable Proxies**
- Sequential failures in short time window
- Withdrawal queue formation
- CDS spread contagion across sector
- Social media panic velocity
- Flight to safety asset spike

**Failure/Inversion Conditions**
- Credible deposit insurance or guarantee
- Transparent stress test disclosure
- Coordinated communication by authorities
- Circuit breakers on withdrawals

**Common Synonyms**
- Bank run contagion
- Panic propagation
- Trust cascade failure
- Self-fulfilling crisis

**Exclusions / Non-examples**
- Single institution failure without propagation
- Rational response to actual insolvency disclosure
- Leverage-driven cascade without confidence element (= C-01)

**Example Instances**
1. Banking panics 1930-33: Four distinct waves; one-third of US banks failed
2. GFC 2008: Lehman bankruptcy froze commercial paper market worldwide
3. Democracy backsliding: Institutional erosion spreads across branches

---

### C-03 | Retaliation Cascade

**Definition**
A unilateral protective or aggressive action triggers symmetric counter-actions from affected parties. Each round escalates, producing collective harm exceeding any individual's original grievance.

**Activation Conditions**
- Multiple actors with retaliation capability
- No credible commitment mechanism to prevent escalation
- Domestic political incentives favoring "strength"
- Absence of neutral arbiter or enforcement

**Observable Proxies**
- Sequential policy announcements in response to prior actions
- Escalating rhetoric in official communications
- Total trade/interaction volume decline
- Third-party "choosing sides" behavior
- Diplomatic recall or sanctions expansion

**Failure/Inversion Conditions**
- Binding international agreement with enforcement
- Overwhelming power asymmetry (one side cannot retaliate)
- Credible third-party mediation
- Domestic political shift favoring cooperation

**Common Synonyms**
- Tit-for-tat escalation
- Trade war spiral
- Sanctions cascade
- Reciprocal punishment loop

**Exclusions / Non-examples**
- One-sided action without response capability
- Coordinated multilateral action (collective, not retaliatory)
- Internal policy change without external trigger

**Example Instances**
1. Smoot-Hawley tariffs 1930: Triggered counter-tariffs; 66% world trade decline
2. US-China trade war: Sequential tariff escalations 2018-2019
3. Roman frontier retaliation: Punitive expeditions triggered barbarian coalitions

---

### C-04 | Terror Multiplication

**Definition**
Dramatic violence or threat against a subset creates reputational effects that influence far larger populations. The display of overwhelming force reduces the need for actual force by inducing preemptive compliance or surrender.

**Activation Conditions**
- Capacity for dramatic, visible violence
- Target population aware of prior examples
- Communication channels to spread reputation
- Alternatives (resistance, flight) appear worse than compliance

**Observable Proxies**
- Surrender without combat after reputation spreads
- Fear-based compliance exceeding direct coercion
- Stories/rumors preceding actual arrival
- Disproportionate psychological impact vs. actual casualties

**Failure/Inversion Conditions**
- Target population has "nothing to lose" (desperation resistance)
- Credibility lost through failed demonstrations
- Counter-narrative successfully framing resistance as viable
- External intervention protecting targets

**Common Synonyms**
- Shock and awe
- Reputational violence
- Exemplary punishment
- Deterrence through demonstration

**Exclusions / Non-examples**
- Sustained attrition warfare (not reputation-based)
- Secret violence without publicity
- Proportional punishment (not designed for multiplication)

**Example Instances**
1. Mongol conquests: Massacre of resisters induced mass surrender; estimated 40M deaths prevented more
2. Atomic bombings 1945: Two cities ended war; conventional invasion estimated 500K+ casualties
3. Roman decimation: 10% execution disciplined entire legions

---

## TRANSFORMATION MECHANISMS

### T-01 | Institutional Substitution

**Definition**
A declining institution's functions gradually transfer to external actors without formal displacement. The original institution persists nominally while new actors assume operational control.

**Activation Conditions**
- Declining institution cannot perform core functions
- Alternative actors capable of functional delivery
- Gradual rather than abrupt transition
- No single moment of formal handover

**Observable Proxies**
- New actors performing old institution's functions
- Original institution's budget/headcount decline
- User/client migration patterns
- Dual reporting structures
- "Acting" or "interim" status normalizing

**Failure/Inversion Conditions**
- Institutional revival or reform
- External actor rejection by constituents
- Regulatory prohibition of substitution
- Sudden rather than gradual collapse (= vacuum, not substitution)

**Common Synonyms**
- Functional displacement
- Gradual takeover
- Shadow institution
- Creeping replacement

**Exclusions / Non-examples**
- Formal merger or acquisition (explicit, not gradual)
- Complete institutional collapse without successor
- Internal reorganization within same institution

**Example Instances**
1. Roman Empire: Foederati gradually assumed military functions
2. Printing Revolution: Publishers replaced scribal guilds
3. Early Christianity: Church hierarchy replaced synagogue networks

---

### T-02 | Procedural Transformation

**Definition**
Power redistribution achieved through changing decision rules rather than direct confrontation. The same actors operate under new procedures that favor different outcomes.

**Activation Conditions**
- Existing rules disadvantage would-be reformers
- Reform coalition can control rule-making process
- New rules appear neutral but shift power
- Opposition cannot block procedural change

**Observable Proxies**
- Voting rule modifications
- Committee restructuring
- Quorum or threshold changes
- Scheduling or agenda control shifts
- Definition changes (who counts as member/voter)

**Failure/Inversion Conditions**
- Constitutional entrenchment of procedures
- Supermajority requirements for rule changes
- Court intervention to restore original procedures
- Coalition fragmentation during transition

**Common Synonyms**
- Rule-based power shift
- Constitutional transformation
- Procedural coup
- Structural reform

**Exclusions / Non-examples**
- Direct force or violence to change outcomes
- Personnel change without rule change
- Persuasion within existing rules

**Example Instances**
1. French Revolution: Estate-based voting → head-count voting
2. Democracy: Gerrymandering, primary rule changes
3. Keynesian Revolution: Policy paradigm shift in macroeconomics

---

### T-03 | State Co-optation

**Definition**
A movement or organization allies with state power, trading autonomy for rapid expansion through state resources and legitimation. The movement's character transforms through the alliance.

**Activation Conditions**
- Movement has achieved critical mass
- State leadership sees strategic benefit in alliance
- Movement leadership willing to compromise autonomy
- Alternative paths (revolution, exile) appear less attractive

**Observable Proxies**
- Official recognition or legal status grants
- State funding or resource provision
- Movement leaders in government positions
- Doctrinal moderation or "mainstreaming"
- Opposition factions expelled or marginalized

**Failure/Inversion Conditions**
- State collapse eliminates alliance benefits
- Movement schism over co-optation
- New leadership rejecting alliance terms
- State shifts to suppression

**Common Synonyms**
- State capture (from movement side)
- Establishment incorporation
- Official religion/ideology adoption
- Mainstreaming

**Exclusions / Non-examples**
- Movement takeover of state (revolution, not co-optation)
- State suppression of movement
- Informal tolerance without alliance

**Example Instances**
1. Early Christianity: Constantine's Edict of Milan; 10% → 56.5% in 50 years
2. Nationalism: State-nation alignment creating "official" nationalisms
3. Totalitarianism: Party-state fusion under single leadership

---

### T-04 | Boundary Shift

**Definition**
Previously fixed conceptual, ethical, or categorical boundaries migrate to new positions through gradual normalization or sudden paradigm change. What was unthinkable becomes debatable, then acceptable, then default.

**Activation Conditions**
- Existing boundary under pressure (new technology, crisis, ideological shift)
- Early transgressors face manageable consequences
- Incremental steps rather than single leap
- Narrative reframing of boundary crossing as progress/necessity

**Observable Proxies**
- "Overton window" movement in discourse
- Policy/practice changes preceding formal rule changes
- Language shifts (euphemism adoption, category redefinition)
- Generational attitude gaps on previously settled questions

**Failure/Inversion Conditions**
- Strong institutional defense of existing boundary
- Backlash reestablishing prior limits
- Transgression produces undeniable harm
- Alternative framing successfully delegitimizes shift

**Common Synonyms**
- Overton window shift
- Normalization
- Category creep
- Ethical drift

**Exclusions / Non-examples**
- Formal rule change through legitimate process (explicit, not drift)
- Individual deviance without social acceptance
- Temporary crisis exception without permanent shift

**Example Instances**
1. CRISPR germline editing: From "unthinkable" (2012) to "He Jiankui incident" (2018) to regulated research (2020s)
2. Drone warfare: From manned aircraft norm to autonomous weapons debate
3. Privacy boundaries: Social media normalized public sharing previously considered private

---

## FEEDBACK MECHANISMS

### F-01 | Accountability Feedback Loop

**Definition**
Periodic evaluation creates information signals that discipline behavior ex ante. Actors modify behavior in anticipation of future judgment, not just in response to past consequences.

**Activation Conditions**
- Regular, credible evaluation cycles
- Consequences linked to evaluation outcomes
- Information from evaluation reaches relevant actors
- Actors have capacity to modify behavior

**Observable Proxies**
- Pre-evaluation behavior changes
- Polling/survey influence on decisions
- Quarter-end or election-cycle timing effects
- Anticipatory announcements
- "Reputation management" activities

**Failure/Inversion Conditions**
- Evaluation becomes purely ceremonial
- Consequences decoupled from evaluation
- Information asymmetry prevents judgment
- Actors cannot change behavior in response

**Common Synonyms**
- Electoral discipline
- Market discipline
- Reputation feedback
- Performance accountability

**Exclusions / Non-examples**
- One-time judgment without recurrence
- Consequences without prior signal (surprise punishment)
- Internal monitoring without external evaluation

**Example Instances**
1. Democracy: Elections discipline incumbent behavior
2. Classical Economics: Market prices signal scarcity, guide production
3. Internet: Reputation systems (ratings, reviews) discipline behavior

---

### F-02 | Network Effect Amplification

**Definition**
System value scales superlinearly with user count, creating positive feedback where adoption accelerates adoption. Critical mass triggers bandwagon dynamics; below threshold, adoption stalls.

**Activation Conditions**
- User value depends on other users' presence
- Low switching costs in early phase
- Visible adoption signals to potential users
- Interoperability or shared standards

**Observable Proxies**
- S-curve adoption pattern
- Accelerating growth rate at inflection point
- Winner-take-most market structure
- High retention once critical mass achieved
- Network density metrics

**Failure/Inversion Conditions**
- Incompatible fragmentation (multiple networks)
- Negative network effects (congestion, spam)
- Platform self-destruction through extraction
- Superior alternative at early stage

**Common Synonyms**
- Metcalfe's Law effects
- Bandwagon effect
- Critical mass dynamics
- Platform network effects

**Exclusions / Non-examples**
- Linear scaling with users (no superlinear component)
- Supply-side economies of scale (production, not network)
- Viral marketing without network value increase

**Example Instances**
1. Internet: Value ∝ n²; rapid adoption post-1995
2. Printing Revolution: Literacy-books spiral; 30K → 12M in 50 years
3. Renaissance: Knowledge networks across city-states

---

### F-03 | Debt-Deflation Spiral

**Definition**
Falling prices increase real debt burden, forcing debtors to sell assets, which drives prices lower, further increasing debt burden. "The more debtors pay, the more they owe" (Irving Fisher).

**Activation Conditions**
- High nominal debt levels
- Deflation or disinflation environment
- Fixed nominal debt contracts (no indexation)
- Debtors have higher spending propensity than creditors

**Observable Proxies**
- Real debt burden increase despite payments
- Asset price decline concurrent with deflation
- Default rate acceleration
- Credit contraction metrics
- Wealth transfer from debtors to creditors

**Failure/Inversion Conditions**
- Monetary expansion stops deflation
- Debt restructuring or forgiveness
- Inflation indexation of debt contracts
- Lender of last resort intervention

**Common Synonyms**
- Fisher debt-deflation
- Deflationary spiral
- Real debt amplification
- Balance sheet recession

**Exclusions / Non-examples**
- Inflation eroding debt burden (opposite)
- Default without deflation (credit event only)
- Price decline without debt amplification

**Example Instances**
1. Great Depression: 31% money supply contraction; real debt burden surge
2. GFC 2008: Asset deflation increased mortgage burden
3. Roman currency debasement: Inverse pattern (inflation eroded savings)

---

## VULNERABILITY MECHANISMS

### V-01 | Overextension-Fragmentation

**Definition**
Coordination span exceeds coordination capacity, enabling peripheral actors to optimize locally rather than globally. Central authority weakens as periphery gains de facto autonomy.

**Activation Conditions**
- Geographic or organizational scale expansion
- Communication/monitoring costs increase with distance
- Peripheral actors have independent resource base
- Central benefits of coordination decline relative to costs

**Observable Proxies**
- Regional policy divergence from center
- Delayed or ignored central directives
- Local revenue retention increase
- Independent peripheral diplomacy
- Center-periphery communication lag

**Failure/Inversion Conditions**
- Communication technology reduces coordination costs
- Fiscal centralization removes peripheral autonomy
- External threat creates coordination imperative
- Peripheral actors lack capacity for independence

**Common Synonyms**
- Imperial overstretch
- Administrative fragmentation
- Decentralization by default
- Span of control failure

**Exclusions / Non-examples**
- Deliberate decentralization (policy choice, not failure)
- External conquest fragmentation
- Internal conflict/civil war (violent, not gradual)

**Example Instances**
1. Roman Empire: Provincial governors prioritized local interests
2. French Revolution: Committee proliferation fragmented authority
3. Totalitarianism: "Chaotic" structure despite total control claims

---

### V-02 | Policy Constraint Lock-in

**Definition**
Adherence to prior commitments or orthodoxies prevents adaptive response when conditions change. The commitment that provided stability becomes a constraint preventing necessary adjustment.

**Activation Conditions**
- Strong prior commitment (legal, ideological, reputational)
- Changed conditions requiring different response
- Exit costs from commitment exceed perceived adjustment benefits
- Decision-makers socialized in prior paradigm

**Observable Proxies**
- Repeated affirmations of commitment despite evidence
- Workarounds that honor letter but not spirit
- Policy reversals framed as "technical adjustments"
- Expert consensus challenging orthodoxy
- Delayed crisis response

**Failure/Inversion Conditions**
- Crisis severe enough to override commitment costs
- Leadership change from outside paradigm
- External force majeure (war, regime change)
- Gradual redefinition of commitment meaning

**Common Synonyms**
- Orthodoxy trap
- Path dependence failure
- Paradigm lock-in
- Commitment trap

**Exclusions / Non-examples**
- Beneficial commitment that enables coordination
- Flexible framework allowing adaptation
- Principled refusal despite feasibility (values, not lock-in)

**Example Instances**
1. Great Depression: Federal Reserve bound by gold standard orthodoxy
2. GFC 2008: Rating agencies locked into flawed models
3. Kodak: Commitment to film business model despite digital evidence

---

### V-03 | Mercenary Loyalty Degradation

**Definition**
Actors recruited through extrinsic incentives (payment, contract) lack institutional loyalty and will defect when alternatives offer superior terms. Outsourced functions become vulnerability points.

**Activation Conditions**
- Core functions performed by contracted actors
- Contractors have portable skills/resources
- Alternative employers or opportunities exist
- Original institution weakens relative to alternatives

**Observable Proxies**
- Contractor turnover rates
- Competing offers to key personnel
- Quality decline in contracted services
- Contractor leverage in renegotiations
- Former contractors competing against institution

**Failure/Inversion Conditions**
- Identity/mission alignment beyond contract
- No alternative employers (monopsony)
- Exit barriers (non-competes, specialized skills)
- Institution revival increasing relative attractiveness

**Common Synonyms**
- Contractor loyalty gap
- Outsourcing vulnerability
- For-hire defection risk
- Extrinsic motivation fragility

**Exclusions / Non-examples**
- Internal employee turnover (different loyalty dynamics)
- Contractor failure due to incompetence, not defection
- Strategic partnership with aligned interests

**Example Instances**
1. Roman barbarization: Foederati commanders displaced the empire
2. Outsourcing dynamics: Contractors build competing capabilities
3. Platform creator exodus: Creators migrate to better-paying platforms

---

### V-04 | Risk Opacity Amplification

**Definition**
Intermediate structures (securitization, supply chains, organizational hierarchy) transform transparent single-entity risk into opaque aggregate structures. Participants cannot accurately price risk because underlying components are hidden. When risk materializes, cascade is amplified because no participant anticipated true exposure.

**Activation Conditions**
- Multiple layers between originator and ultimate risk-bearer
- Information asymmetry favoring originators over end-holders
- Incentive to package/transfer rather than retain risk
- Third-party validators with conflicts of interest
- Complexity exceeding evaluator capacity

**Observable Proxies**
- Spreads between rated risk and realized default rates
- Increasing reliance on third-party validation
- Declining due diligence effort per unit of exposure
- Concentration of exposure discovered only post-crisis
- "Nobody saw it coming" post-mortem discourse

**Failure/Inversion Conditions**
- Regulatory transparency requirements
- Skin-in-the-game mandates
- Technology enabling real-time tracking
- Catastrophic failure creating institutional memory

**Common Synonyms**
- Complexity opacity
- Securitization black box
- Supply chain opacity
- Algorithmic opacity

**Exclusions / Non-examples**
- [TE-02] Protocol Layering where abstraction clarifies
- Deliberate secrecy with single party holding full information
- Simple information asymmetry without layered structure

**Example Instances**
1. GFC 2008: CDO structures; 73% of 2006 AAA MBS became junk
2. Supply chain chip shortage 2021: hidden fab concentration
3. Enron SPE structures: complexity designed to obscure debt

---

### V-05 | Epistemic Opacity

**Definition**
Relevant knowledge exists only in distributed form across many individual minds and cannot be aggregated by any central authority. Attempts to centralize decisions fail because the necessary information is local, tacit, and context-dependent.

**Activation Conditions**
- Information distributed across many actors
- Knowledge is tacit/contextual (cannot be fully articulated)
- Central planner lacks price signals or equivalent feedback
- Complexity exceeds any single actor's comprehension

**Observable Proxies**
- Central plans systematically mis-allocate resources
- Local adaptations outperform centralized directives
- "Knowledge problem" discourse in policy debates
- Persistent information asymmetries despite transparency efforts

**Failure/Inversion Conditions**
- Domain is simple enough for central comprehension
- Effective aggregation mechanism exists (markets, prediction markets)
- AI/technology enables sufficient information processing
- Standardization reduces context-dependence

**Common Synonyms**
- Knowledge problem (Hayek)
- Distributed cognition
- Local knowledge advantage
- Calculation problem

**Exclusions / Non-examples**
- Deliberate information hiding (opacity by choice, not structure)
- Simple asymmetric information (one party knows, other doesn't)
- Temporary information lag (eventually aggregable)

**Example Instances**
1. Soviet planning failures: Gosplan couldn't replicate price system information
2. Corporate headquarters vs. local branches: HQ directives often suboptimal
3. Medical diagnosis: Patient's felt experience inaccessible to external observer

---

## DOMAIN-SPECIFIC HIGH-TRANSFER MECHANISMS

### PO-01 | Atomization-Capture

**Definition**
Systematic destruction of intermediate social bonds (class, community, family, profession) creates isolated individuals susceptible to totalistic ideological capture. The movement offers substitute belonging.

**Activation Conditions**
- Pre-existing social bond erosion
- Mass urbanization or displacement
- Economic disruption destroying traditional roles
- Ideology offering comprehensive worldview

**Observable Proxies**
- Decline in associational membership
- Rise in loneliness/isolation metrics
- Totalistic movement membership surge
- "Born again" or radical conversion narratives
- Former identity rejection

**Failure/Inversion Conditions**
- Resilient intermediate institutions
- Competing ideologies fragment capture
- Movement overreach triggers resistance
- Economic stabilization restores traditional roles

**Common Synonyms**
- Social atomization
- Mass society capture
- Totalitarian recruitment
- Community destruction and replacement

**Exclusions / Non-examples**
- Voluntary community change (chosen, not forced)
- Gradual secularization (without capture)
- Elite capture without mass atomization

**Example Instances**
1. Totalitarianism (Arendt): "Masses grown out of fragments of atomized society"
2. Social media: Platform mediates atomized users into pseudo-community
3. Cult formation: Isolation followed by intense group belonging

---

### PO-02 | Onion Layering

**Definition**
Concentric organizational structure with radicalization gradient: extreme core, normalized periphery. Outer layers provide legitimacy and recruitment; inner layers pursue radical aims. Front organizations conceal true nature.

**Activation Conditions**
- Need to maintain public legitimacy while pursuing radical goals
- Graduated commitment pathway for recruits
- Organizational capacity for compartmentalization
- Sufficient scale to maintain multiple layers

**Observable Proxies**
- Discrepancy between public statements and internal documents
- "Levels" or "degrees" of membership
- Front organizations with innocuous names
- Progressive radicalization of long-term members
- Inner circle access restrictions

**Failure/Inversion Conditions**
- Exposure of inner layer to public scrutiny
- Defection of inner members with documentation
- Insufficient recruitment to outer layers
- State penetration of compartmentalization

**Common Synonyms**
- Concentric radicalization
- Front organization structure
- Graduated extremism
- Dual-face architecture

**Exclusions / Non-examples**
- Uniform organization without gradient
- Transparent hierarchy (radical but open)
- Single-layer extremist group

**Example Instances**
1. Totalitarianism: Leader → inner circle → SS/SA → party → sympathizers
2. QAnon: "Asking questions" surface → deep conspiracy core
3. Some corporate cultures: Public values vs. internal practices

---

### TE-01 | End-to-End Principle

**Definition**
System architecture placing intelligence and complexity at endpoints while keeping core infrastructure simple ("dumb pipes"). Enables innovation at edges without core modification.

**Activation Conditions**
- Diverse endpoint needs that cannot be predicted
- Core infrastructure serving multiple applications
- Low marginal cost of endpoint customization
- Governance allowing endpoint autonomy

**Observable Proxies**
- Application diversity without infrastructure change
- Low barrier to new endpoint development
- Core stability across application generations
- "Permissionless innovation" discourse
- Minimal feature set in core protocols

**Failure/Inversion Conditions**
- Core captures application-layer value (platform power)
- Security/trust requirements force core intelligence
- Standardization pressure homogenizes endpoints
- Regulatory mandates in core layer

**Common Synonyms**
- Dumb pipes architecture
- Edge intelligence
- Thin core / fat edge
- Decentralized innovation

**Exclusions / Non-examples**
- Intelligent network with simple endpoints (telephone model)
- Vertically integrated stack
- Platform-controlled application ecosystem

**Example Instances**
1. Internet: TCP/IP as dumb pipes; HTTP/HTML at application layer
2. Organizational design: Decision-making at subsidiaries
3. Platform architecture: API-first design enabling third-party apps

---

### TE-02 | Protocol Layering

**Definition**
Complex systems self-organize into hierarchical layers with defined interfaces. Each layer can evolve independently as long as interface contracts are honored. Separation of concerns enables parallel development.

**Activation Conditions**
- System complexity exceeds single-layer management
- Multiple teams or actors developing components
- Need for backward compatibility
- Interface definition capability

**Observable Proxies**
- Layer terminology in system description
- Interface specification documents
- Layer-specific teams or organizations
- "Shim" or "adapter" patterns at boundaries
- Layer-specific failure modes

**Failure/Inversion Conditions**
- "Leaky abstractions" violating layer boundaries
- Performance requirements forcing layer bypass
- Interface ossification preventing evolution
- Layer collapse under integration pressure

**Common Synonyms**
- Separation of concerns
- Abstraction layers
- Stack architecture
- Modular hierarchy

**Exclusions / Non-examples**
- Monolithic system without layer distinction
- Peer-to-peer flat architecture
- Loosely coupled but non-hierarchical modules

**Example Instances**
1. Internet: TCP/IP 4-layer model (link, network, transport, application)
2. Legal systems: Constitution → statute → regulation → interpretation
3. Organizations: Strategy → policy → process → execution

---

### TE-03 | Reproduction Cost Collapse

**Definition**
Technological change reduces marginal cost of information/content reproduction toward zero, breaking natural monopolies of knowledge producers and enabling mass distribution.

**Activation Conditions**
- New reproduction technology available
- High prior reproduction costs (scarcity-based value)
- Content/knowledge suitable for mechanical reproduction
- Distribution infrastructure in place

**Observable Proxies**
- Unit cost decline by order of magnitude
- Output volume explosion
- New entrant proliferation
- Incumbent gatekeeper decline
- Business model disruption discourse

**Failure/Inversion Conditions**
- Legal protection (copyright, DRM) restoring scarcity
- Network effects creating new gatekeepers
- Quality differentiation restoring premium
- Attention scarcity replacing production scarcity

**Common Synonyms**
- Marginal cost zeroing
- Abundance economics
- Gatekeeping disruption
- Democratization through cheap reproduction

**Exclusions / Non-examples**
- Physical goods with irreducible material costs
- Services requiring human presence
- Reduction without mass distribution

**Example Instances**
1. Printing Revolution: Book cost reduced to 1/8; 30K → 12M in 50 years
2. Internet/Digital: Near-zero marginal distribution cost
3. AI/LLM: Content creation cost collapse

---

### E-01 | Invisible Hand Coordination

**Definition**
Self-interested actions by atomized agents, mediated through price signals or other information mechanisms, produce beneficial aggregate outcomes without intentional coordination or central planning.

**Activation Conditions**
- Agents pursuing individual utility
- Information signal system (prices, ratings, reputation)
- Free entry and exit
- No single agent can dominate signal

**Observable Proxies**
- Price convergence to clearing levels
- Resource allocation shifts without directive
- "Spontaneous order" emergence
- Decentralized problem-solving
- Market equilibrium restoration after shock

**Failure/Inversion Conditions**
- Market power concentration (monopoly)
- Information asymmetry (adverse selection, moral hazard)
- Externalities not reflected in signals
- Coordination problems (prisoner's dilemma)

**Common Synonyms**
- Spontaneous order
- Market coordination
- Decentralized optimization
- Price mechanism

**Exclusions / Non-examples**
- Central planning with price-like signals
- Explicit coordination through negotiation
- Command-and-control resource allocation

**Example Instances**
1. Classical Economics: Market prices guiding production and consumption
2. Open source: Reputation/utility signals guiding contribution
3. Democracy: Vote aggregation producing collective decisions

---

### E-02 | Knowledge Spillover

**Definition**
Innovation or discovery in one domain unintentionally enables advancement in other domains. Value created flows beyond the original creator's capture, producing positive externalities that accelerate adjacent development.

**Activation Conditions**
- Novel knowledge or technique created
- Transferable across domain boundaries
- Inadequate appropriation mechanisms (patents, secrecy)
- Adjacent domains receptive to transfer

**Observable Proxies**
- Citations/adoptions from unrelated fields
- Inventor does not capture proportional value
- "Enabling technology" discourse
- Sequential innovation building on uncompensated base

**Failure/Inversion Conditions**
- Strong IP protection capturing value
- Tacit knowledge requiring direct transfer
- Domain specificity preventing generalization
- Absorptive capacity lacking in adjacent domains

**Common Synonyms**
- Positive externality
- Technology transfer
- Enabling innovation
- R&D spillover

**Exclusions / Non-examples**
- Licensed technology transfer (compensated)
- Internal knowledge sharing within firm
- Deliberate open-sourcing (intentional, not spillover)

**Example Instances**
1. DARPA research: Military R&D creating Internet, GPS, AI for civilian use
2. Bell Labs: Corporate research producing transistor, Unix, information theory
3. Xerox PARC: GUI, Ethernet invented but commercialized by others

---

## COLLAPSE ARCHETYPES

Collapse is a canonical grammar type. The following subtypes refine collapse dynamics for precise classification.

### collapse-cascade

**Definition**
A high-connectivity system experiences rapid threshold breach, triggering self-amplifying failure cascades that eliminate stabilizing buffers.

**Activation Conditions**
- High interdependence across subsystems
- Compressed feedback loops (fast propagation)
- Low modular insulation (no circuit breakers)
- Trust, liquidity, or confidence shock

**Failure Modes**
- Strong circuit breakers halt propagation
- Decentralized redundancy absorbs shock
- Adaptive substitution fills gaps before cascade

**Cross-Domain Candidates**
- Economics: Financial crises, market crashes
- Politics: Revolutionary cascades, regime collapse
- Technology: Infrastructure failures, platform collapses
- Religion: Schism cascades, faith crises

---

### collapse-erosion

**Definition**
A system undergoes prolonged legitimacy or function decay, gradually transferring capacity outward until symbolic or structural disintegration occurs.

**Activation Conditions**
- Slow legitimacy decline over extended period
- Peripheral autonomy growth
- Resource diffusion from center to periphery
- Administrative overstretch exceeding coordination capacity

**Failure Modes**
- Institutional reform renews legitimacy
- Centralization rebound restores control
- Resource re-aggregation reverses diffusion

**Cross-Domain Candidates**
- History: Empire dissolution, institutional decline
- Religion: Denominational fragmentation, authority decay
- Economics: Corporate decline, brand erosion
- Art: Movement dissolution, canon rejection

---

## SUBSTITUTION ARCHETYPES

Substitution is a canonical grammar type. The following subtypes refine substitution dynamics for precise classification.

### substitution-category

**Definition**
A foundational organizing category of perception or legitimacy is replaced by an alternative framework.

**Activation Conditions**
- Legitimacy instability in existing framework
- Conceptual contradiction exposed
- Normative inversion pressure from challengers

**Failure Modes**
- Strong doctrinal insulation prevents challenger penetration
- Institutional suppression of alternative frameworks
- Symbolic rigidity blocks category transition

**Cross-Domain Candidates**
- Religion: Reform movements, theological paradigm shifts
- Politics: Regime legitimacy replacement, constitutional transformation
- Philosophy: Paradigm shifts, foundational category revision
- Art: Aesthetic canon replacement

---

### substitution-functional

**Definition**
Operational authority or systemic function shifts from one structural node to another.

**Activation Conditions**
- Central node inefficiency or capacity decline
- Peripheral node competence growth
- Crisis-triggered delegation of functions

**Failure Modes**
- Strong central reassertion recaptures functions
- Institutional lock-in prevents migration
- Network fragmentation before transfer completes

**Cross-Domain Candidates**
- History: Empire decentralization, administrative devolution
- Economics: Market disintermediation, platform emergence
- Technology: Protocol layer shifts, infrastructure migration
- Politics: Federalization, power devolution

---

### substitution-scarcity

**Definition**
The primary locus of value or scarcity concentration shifts to a new structural domain.

**Activation Conditions**
- Technological change reduces prior scarcity
- Cost collapse in incumbent domain
- Resource diffusion enables new concentration point

**Failure Modes**
- Regulatory containment restores old scarcity
- Asset re-centralization by incumbents
- Cultural resistance to new value regime

**Cross-Domain Candidates**
- Economics: Capital → data economy, land → industrial capital
- Technology: Attention → algorithmic allocation, compute → inference
- Art: Object scarcity → experience scarcity
- Religion: Clerical authority → textual access

---

## Appendix: Deprecated Patterns

The following terms were used in earlier Core files and should be migrated to canonical forms per `040_OS/pattern-compression-v0.2.md`:

| Deprecated | → | Canonical |
|------------|---|-----------|
| transformation | → | substitution (or T-series) |
| gradual-decline | → | erosion |
| institutional-decay | → | erosion |
| schism | → | fragmentation |
| prisoners-dilemma | → | [V-03] Coordination Failure |
| retaliatory-spiral | → | [MP-01] Reflexive Spiral |
| information-asymmetry (as pattern) | → | [V-04] Information Asymmetry |
| gatekeeper-displacement (as pattern) | → | [MP-04] Gatekeeper Displacement |
| speculative-bubble | → | [MP-01] + [C-01] |
| systemic-contagion | → | [C-02] Confidence Contagion |
| normalization-of-deviance | → | [F-01] accountability failure |

---

*End of Pattern Dictionary v0.2*
