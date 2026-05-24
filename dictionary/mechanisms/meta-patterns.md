---
type: meta-patterns
version: v0.2.2
date: 2026-03-20
pattern_count: 21
source: pattern-compression-v0.1
---

# Meta-Patterns v0.1.1

## Usage

Meta-patterns are abstract structures that generate multiple specific mechanisms. They operate at a higher level of abstraction than mechanisms and describe recurrent dynamics across domains.

Format:
- **Name**: Pattern identifier
- **Structure**: Abstract form (A→B→C notation where applicable)
- **Generates**: Types of mechanisms this pattern tends to produce
- **Observable Proxies**: How to detect the pattern operating
- **Example Instances**: 2-3 cases from research corpus

---

## SYSTEM DYNAMICS PATTERNS

### MP-01 | Reflexive Spiral

**Structure**
A → B → more A → more B → ...

Effect reinforces cause in positive feedback loop. Initial perturbation triggers response that amplifies original perturbation. Continues until external intervention or resource exhaustion.

**Generates**
- Cascade mechanisms (C-01, C-02)
- Bubble dynamics
- Arms races
- Reputation cascades
- Terror-atomization loops

**Observable Proxies**
- Accelerating rate of change
- Deviation from historical mean increasing over time
- Self-reference in causal chain
- Amplification rather than dampening of shocks
- "Runaway" or "spiral" language in actor discourse

**Example Instances**
1. Leverage Cascade: Rising prices → more leverage → higher prices → more leverage
2. Totalitarian terror: Terror → atomization → susceptibility → more terror
3. Speculative bubble: Price rise → media coverage → new buyers → price rise

---

### MP-02 | Threshold Transition

**Structure**
Stable state → critical variable crosses threshold → rapid regime change → new stable state

System remains in equilibrium until key parameter crosses critical value, then transitions rapidly to qualitatively different state. Phase transition dynamics.

**Generates**
- Regime change mechanisms
- Adoption cascades
- Bank run triggers
- Revolution triggers
- Paradigm shifts

**Observable Proxies**
- Long stability followed by sudden change
- "Tipping point" language
- Bifurcation in outcome distribution
- Path dependence after transition
- Hysteresis (different thresholds for forward/backward transition)

**Example Instances**
1. Political transitions: Authoritarian stability → legitimacy threshold → rapid democratization
2. Network adoption: Slow growth → critical mass → exponential adoption
3. Bank runs: Confidence stable → withdrawal threshold → cascade

---

### MP-03 | Self-Undermining Success

**Structure**
Success → parameter change → success becomes failure

System's successful operation changes conditions such that the same behaviors no longer produce success. What worked undermines the conditions for its own continuation.

**Generates**
- Diminishing returns mechanisms
- Disruption dynamics
- Antibiotic resistance patterns
- Imperial overextension
- Bureaucratization

**Observable Proxies**
- Declining returns to same inputs
- "What got us here won't get us there" discourse
- Increasing effort for same results
- Conditions that enabled success no longer present
- Successful actors facing unexpected failure

**Example Instances**
1. Capital accumulation: Success → diminishing returns → stationary state
2. Innovation → disruption of own market → obsolescence
3. Antibiotic success → resistance evolution → drug failure

---

## ORGANIZATIONAL PATTERNS

### MP-04 | Gatekeeper Displacement

**Structure**
Reproduction cost collapse → incumbent gatekeeper function obsolete → new gatekeepers emerge → cycle repeats

Technological change eliminates scarcity that gatekeepers controlled; new gatekeepers emerge at new scarcity points.

**Generates**
- Institutional substitution (T-01)
- Reproduction cost collapse effects (TE-03)
- Platform emergence
- Disintermediation cycles

**Observable Proxies**
- Incumbent revenue/influence decline
- New intermediary emergence
- "Disintermediation" discourse followed by "re-intermediation"
- Scarcity shift (from production to attention, from access to curation)
- Former gatekeepers repositioning or exiting

**Example Instances**
1. Scribes → printing press → publishers → internet → platforms
2. Record labels → digital distribution → streaming platforms
3. Travel agents → online booking → aggregators

**Inverse Pattern: Gatekeeper Counterattack**

When incumbent gatekeepers retain sufficient power (capital, regulatory influence, platform control), they can **close the gates** rather than be displaced.

Structure: Displacement threat detected → gatekeeper mobilizes resources → regulatory/technical barriers erected → new technology adoption delayed/blocked

Example Instances:
1. Apple vs Vibe Coding (2026): App Store ($160B ecosystem) threatened by AI-generated apps → Apple blocks Replit/Vibecode updates citing "quality control"
2. News publishers vs aggregators: Link taxes and copyright claims to block news aggregation
3. Taxi industry vs ride-sharing: Regulatory lobbying to restrict Uber/Lyft licensing

Observable Proxies:
- "Quality" or "safety" justifications for restrictions
- Regulatory capture accelerating during displacement threat
- Incumbent revenue defense correlating with restriction timing

---

### MP-05 | Charisma-Institution Transition

**Structure**
Charismatic authority → founder mortality/absence → routinization crisis → institutional authority OR schism

Movements founded on personal charisma must institutionalize or fragment when founder is no longer present. Weber's "routinization of charisma."

**Generates**
- Hierarchical response to fragmentation
- Succession crises
- Canon formation
- Bureaucratization

**Observable Proxies**
- Succession struggle upon founder departure
- Codification of previously oral/personal knowledge
- Emergence of bureaucratic roles
- "Founding principles" disputes
- Splinter movements claiming true inheritance

**Example Instances**
1. Early Christianity: Jesus → apostolic disputes → episcopal hierarchy
2. Startups: Founder era → professionalization → corporate structure
3. Political movements: Charismatic leader → institutionalized party

---

### MP-06 | Competitive Patronage Escalation

**Structure**
Multiple power centers → prestige competition through investment → each escalation raises baseline → continuous innovation

Competing actors invest in cultural/technological/organizational production for status; competition drives standards upward.

**Generates**
- Innovation incentives
- Arms race dynamics
- Prestige goods production
- Talent concentration

**Observable Proxies**
- Sequential announcements exceeding prior commitments
- "Keeping up with" language
- Talent bidding wars
- Investment concentration in prestige domains
- Acceleration of standards

**Example Instances**
1. Renaissance city-states: Florence, Venice, Milan competing through patronage
2. University rankings: Schools competing through spending
3. Tech company campuses: Escalating amenities for talent attraction

---

## CRISIS PATTERNS

### MP-07 | Shock-Redistribution

**Structure**
Catastrophic event → existing equilibrium destabilized → resource/power redistribution → new equilibrium

Major disruption breaks path dependency, enabling redistribution normally blocked by incumbent interests or coordination problems.

**Generates**
- Post-crisis policy windows
- Wealth/power redistribution
- Institutional reform opportunities
- Social contract renegotiation

**Observable Proxies**
- Crisis followed by major policy change
- "Never let a crisis go to waste" discourse
- Pre-crisis losers gaining post-crisis
- Path-dependent arrangements disrupted
- Negotiating leverage shift

**Example Instances**
1. Black Death → wage increase → serfdom collapse → worker bargaining power
2. WWII → welfare state expansion → labor rights
3. Pandemic → remote work normalization → geographic redistribution

---

### MP-08 | Counter-Reformation Lag

**Structure**
Disruptive change → incumbent denial/delay → ~100 year lag → institutional response → new equilibrium with control mechanisms

Incumbent institutions respond to disruption only after it becomes irreversible; response attempts to reassert control within new constraints.

**Generates**
- Regulatory catch-up cycles
- Censorship apparatus formation
- Standard-setting battles
- Legitimation crisis responses

**Observable Proxies**
- Long delay between disruption and official response
- Initial dismissal followed by overreaction
- Control mechanisms arriving after widespread adoption
- "Closing the barn door" criticism
- Response effectiveness limited by prior diffusion

**Example Instances**
1. Printing press (1450) → Index Librorum Prohibitorum (1559): ~100 years
2. Internet (1990s) → GDPR (2018): ~25 years (accelerated?)
3. Social media (2005) → Content moderation crisis (2020s): ~15 years

---

### MP-09 | Vacuum-Authoritarian Cycle

**Structure**
Revolution/collapse → power vacuum → instability → demand for order → centralized authority reconstitution

Post-revolutionary instability creates conditions for authoritarian restoration; the very disorder that revolution created generates demand for its opposite.

**Generates**
- Post-revolutionary authoritarian patterns
- Stability-seeking behavior
- Strongman emergence
- Revolutionary thermidor

**Observable Proxies**
- Rising crime/disorder post-revolution
- Nostalgia for pre-revolutionary order
- Strongman popularity surge
- Revolutionary faction mutual destruction
- Order restoration as primary political demand

**Example Instances**
1. French Revolution → Directory instability → Napoleon
2. Weimar Republic → chaos → Hitler
3. Russian Revolution → civil war → Stalin consolidation

---

## KNOWLEDGE PATTERNS

### MP-10 | Fixity Enables Accumulation

**Structure**
Preservation technology → knowledge fixed → accumulation replaces rediscovery → cumulative progress

Without preservation, knowledge must be rediscovered cyclically. Preservation technology transforms knowledge from cyclical to cumulative, enabling standing on shoulders.

**Generates**
- Scientific revolution conditions
- Institutional memory formation
- Standard reference creation
- Cross-generational knowledge transfer

**Observable Proxies**
- Citation/reference to prior work
- Declining "reinvention" rates
- Standard texts/references emergence
- Version control or archival systems
- "Building on" vs. "rediscovering" language

**Example Instances**
1. Printing press: Multiple identical copies enable cumulative science
2. Version control: Code accumulation without loss
3. Wikipedia: Continuous improvement without restart

---

### MP-11 | Vernacular Democratization

**Structure**
Elite language monopoly → translation to mass language → access expansion → power redistribution

Knowledge controlled through specialized language becomes accessible through translation to common language, shifting power from gatekeepers to general population.

**Generates**
- Literacy expansion
- Professional boundary dissolution
- Democratization of expertise
- Backlash from professional classes

**Observable Proxies**
- Mass-language publications increasing
- "Plain language" movements
- Professional jargon criticism
- Self-service replacing expert consultation
- Gatekeeping resistance

**Example Instances**
1. Latin → vernacular Bibles (Luther)
2. Programming → no-code tools
3. Legal/medical jargon → AI-assisted plain language

---

### MP-12 | Network Parasitism

**Structure**
New movement → utilizes existing infrastructure → rapid spread without infrastructure building → eventual independence or displacement

Movements spread fastest by parasitizing existing organizational infrastructure rather than building new networks.

**Generates**
- Movement diffusion patterns
- Platform-based business models
- Institutional capture dynamics
- Infrastructure appropriation

**Observable Proxies**
- New entity using old entity's resources
- Rapid spread without proportional investment
- Tension between parasite and host
- Eventual separation or host displacement
- "Leveraging" existing assets language

**Example Instances**
1. Early Christianity: Synagogue network parasitism
2. Uber: Utilizing existing car infrastructure
3. Startups on AWS: Building on cloud infrastructure

---

### MP-13 | Shock-Fatigue Cycle

**Structure**
Shock → Attention capture → Habituation → Escalation required → Diminishing returns → Exhaustion → Reset (or system transformation)

Transgression or novelty initially captures attention, but repeated exposure creates habituation. Maintaining attention requires escalation, which depletes capacity until system reaches exhaustion. Reset occurs through generational turnover, catastrophic event, or transformation.

**Generates**
- Escalation mechanisms (arms races, transgression spirals)
- Exhaustion failures (innovation exhaustion, outrage fatigue)
- Reset opportunities (post-exhaustion new entrant openings)
- Planned obsolescence dynamics

**Observable Proxies**
- Decreasing attention duration per equivalent stimulus
- Escalating intensity over time
- "What will they do next?" anticipation discourse
- Post-saturation backlash or "return to basics" movements
- Movement/style lifecycle compression

**Example Instances**
1. Modernist movements: Impressionism (20y) → Cubism (10y) → 1960s movements (2-3y)
2. Political scandal cycles: each must exceed previous; eventual "scandal fatigue"
3. Marketing shock tactics: Benetton initially effective, then normalized

---

## DISCOVERED PATTERNS (2026-03-15)

The following meta-patterns were discovered through gap analysis of unobserved mechanism × meta-pattern combinations.

### MP-14 | Captured Stability Accumulation

**Structure**
Regulatory/institutional capture → stability without competition → long-term investment horizon → knowledge accumulation → eventual disruption when capture breaks

Paradoxically, capture can create conditions for accumulation by removing competitive pressure and enabling long-term thinking.

**Generates**
- Research labs in monopolies
- Standards lock-in with innovation
- Tenure-based scholarship

**Observable Proxies**
- Long-tenured researchers in captured environments
- Basic research investment in monopoly/oligopoly contexts
- "The price of stability is capture" discourse

**Example Instances**
1. Bell Labs: AT&T's captured regulatory environment enabled 40 years of fundamental research
2. Japanese Keiretsu: Cross-shareholding "capture" enabling long-term R&D
3. Microsoft 1995-2005: Antitrust period paradoxically enabled Office/Windows accumulation

**Source Gap**: V-03 × MP-10

---

### MP-15 | Automation-Displacement Vacuum

**Structure**
Process automation → structural unemployment → social dislocation → political vacuum → authoritarian/populist response → (new) automation-enabled control

Automation creates the chaos that demands authoritarian solutions, which then use automation for control.

**Generates**
- Luddite movements
- Protectionist politics
- Surveillance states
- "Forgotten worker" populism

**Observable Proxies**
- Unemployment concentrated in automatable sectors
- "Forgotten worker" political discourse
- Strongman promises of job restoration
- Surveillance automation as governance tool

**Example Instances**
1. Industrial Revolution → Factory Acts: Automation chaos led to state intervention
2. Rust Belt → 2016 US Election: Manufacturing automation correlated with populist voting
3. AI → (predicted): Displacement creating governance crisis, surveillance as response

**Source Gap**: TE-01 × MP-09

---

### MP-16 | Democratized Blindness

**Structure**
Elite model with limitations → vernacular translation → mass adoption without limitation awareness → systematic misapplication → model blindness at scale

When expert models become accessible to masses, simplification strips away the warnings, and errors scale.

**Generates**
- Financial illiteracy despite tools
- Medical misdiagnosis from self-diagnosis
- AI hallucination acceptance
- Oversimplified framework abuse

**Observable Proxies**
- "One weird trick" simplifications
- Mass adoption preceding mass education on limitations
- Systematic errors in popularized model applications
- Expert backlash against oversimplification

**Example Instances**
1. Options trading democratization: Retail traders applying Black-Scholes without understanding
2. MBTI mass adoption: Clinical tool misused for hiring and relationships
3. WebMD: Medical model democratized, hypochondria epidemic
4. ChatGPT: AI capabilities democratized, hallucination blindness spreading

**Source Gap**: V-04 × MP-11

---

### MP-17 | Accountability Fatigue Loop

**Structure**
Accountability mechanism → repeated violations → evaluator habituation → escalation required for equivalent response → accountability breakdown

**CRITICAL**: This is how democracies and markets fail. Accountability systems have finite attention capacity.

**Generates**
- Scandal normalization
- Compliance theater
- Audit fatigue
- "Outrage exhaustion"

**Observable Proxies**
- Declining consequence severity for equivalent violations
- "Nothing matters anymore" discourse
- Ritual compliance replacing substantive accountability
- Selective enforcement (only exceptional cases prosecuted)

**Example Instances**
1. Trump administration: Scandals that would have ended previous presidencies became normalized
2. Corporate governance: Enron → Sarbanes-Oxley → fatigue → FTX
3. Security alerts: Repeated warnings → user habituation → ignored alerts → breach

**Source Gap**: F-01 × MP-13

**Dictionary Impact**: Add explicit warning to F-01 documentation.

---

### MP-18 | Coordination Signal Fatigue

**Structure**
Self-organizing system → repeated signals → habituation → signal escalation required → diminishing coordination efficiency

Markets and democracies rely on signals to coordinate; when signals become normalized, the system loses coordination capacity.

**Generates**
- Central bank intervention fatigue
- Democratic mandate erosion
- Platform algorithm escalation

**Observable Proxies**
- Decreasing market response to equivalent announcements
- "Priced in" discourse before events occur
- Escalating stimulus required for same effect

**Example Instances**
1. QE fatigue: QE1 (2008) massive impact → QE2 (2010) muted → QE3 "QE infinity" required
2. Federal Reserve forward guidance: Diminishing surprise capacity
3. SNS algorithms: Increasing engagement bait required as users habituate

**Source Gap**: E-01 × MP-13

---

### MP-19 | Crisis Response Fatigue

**Structure**
Crisis event → intervention → habituation → next event requires larger response → eventually response capacity exhausted

Each bailout creates expectation of next bailout, requiring larger intervention to achieve same stabilization effect.

**Generates**
- Moral hazard accumulation
- Intervention escalation
- "Too big to fail" expansion

**Observable Proxies**
- Each crisis intervention larger than previous
- Baseline intervention size increasing
- Crisis intervals shortening while intervention size grows

**Example Instances**
1. Fed interventions: 1987 (modest) → 1998 (LTCM) → 2008 (TARP) → 2020 (unlimited)
2. Bank bailouts: Each larger than previous
3. Eurozone crisis: Greece → larger facilities → "whatever it takes"

**Source Gap**: E-02 × MP-13

**Sub-pattern: Exception Cascade**

A specific mechanism within Crisis Response Fatigue focusing on the irreversibility of "temporary" exceptions.

Structure: Crisis → "temporary" exception → beneficiaries form → lobbying for continuation → withdrawal politically impossible → next crisis requires larger exception

Why exceptions persist:
1. **Beneficiary lock-in**: Exception creates winners who lobby to maintain it
2. **Baseline shift**: New "normal" anchors to exception state
3. **Capacity depletion**: Each exception reduces room for next intervention

Example Instances:
1. Venezuela sanctions (2026): "Temporary" easing for oil prices → beneficiaries form → continuation pressure
2. Jones Act waiver (2026): 106-year law suspended "temporarily" → shipping industry adapts → reversal difficult
3. Nixon Shock (1971): "Temporary" gold window closure → 54 years later, still "temporary"
4. TARP (2008): "Emergency" program → 6 years to wind down
5. COVID emergency (2020): "2 weeks to flatten curve" → 1,167 days

Observable Proxies:
- "Temporary" language in policy announcements
- Beneficiary lobbying appearing within months
- "Sunset clause" extensions
- "The exception has become the rule" discourse

---

### MP-20 | Game Layer Migration

**Structure**
Competition at Layer N → saturation/commoditization → advantage shifts to Layer N+1 → early movers at N+1 dominate → new game established

Competitive advantage migrates upward through abstraction layers. Those optimizing at the old layer lose to those who recognize the shift.

**Generates**
- Platform disruption
- "Meta-game" dominance
- Paradigm obsolescence
- First-mover advantage at new layer

**Observable Proxies**
- Diminishing returns at current layer
- "Everyone is doing X now" discourse
- New entrants winning despite inferior Layer N performance
- Experts at old layer dismissing new layer as "not real"
- Language shift from tactics to strategy/infrastructure

**Example Instances**
1. AI prompting → context architecture: Individual prompt optimization saturates; persistent context design becomes differentiator
2. Stock picking → algorithmic trading → market structure: Each layer shift obsoletes previous expertise
3. SEO keywords → domain authority → platform ownership: Google rewards layer migration
4. Feature competition → platform effects → ecosystem control: Apple/Google transcended feature wars
5. Individual skill → team coordination → organizational design: Management science evolution

**Diagnostic Application**
- "What layer is the current competition happening at?"
- "Is that layer saturating? What's the next layer up?"
- "Who is already operating at the higher layer?"
- "What would it cost to migrate?"

**Source**: Extracted from "Claude Cowork Starter Pack" analysis (2026-03-18)

---

### MP-21 | Asymmetric Dependency

**Structure**
Build-up (slow) → Adaptation → Dependency formation → Breakdown (fast) → Rebuild (incomplete)

Effects take long to construct but short to lose. Once lost, restoration is partial at best. Creates structural lock-in where stopping is more dangerous than continuing.

**Generates**
- Medical dependency patterns
- Policy irreversibility
- Vendor lock-in
- Infrastructure path dependency

**Observable Proxies**
- Build-up timescale >> breakdown timescale
- "Can't stop now" discourse
- Resumption producing diminished returns
- Discontinuation rates high despite risks
- "Metabolic whiplash" or equivalent terminology

**Mathematical Signature**
- T(build) > 2 × T(breakdown)
- Effect(resume) < Effect(original)
- Risk(discontinue) > Risk(continue) after threshold

**Example Instances**
1. GLP-1 medications (2026): Cardiovascular protection takes years to build; 6 months off → +4% risk, 1 year → +14%, 2 years → +22%. Resumption only partially restores protection.
2. Quantitative Easing: Years to stabilize markets; "taper tantrum" (2013) showed days to destabilize. Each QE round requires larger doses.
3. Social media presence: Years to build followers; account suspension = instant loss. Platform migration recovers fraction.
4. Cloud migration: 1-3 years to migrate; re-migration even longer. "Vendor lock-in" as common terminology.
5. Car-centric urban design: Decades to build highway network; decades more to transition to transit. Detroit still locked in despite industry decline.

**Diagnostic Questions**
- "How long did it take to build this effect?"
- "How fast would the effect disappear if stopped?"
- "If resumed, would the effect return to previous levels?"
- "Who benefits from the asymmetry continuing?"

**Relationship to Other Patterns**
- Amplifies MP-19 (Crisis Response Fatigue): Each intervention creates asymmetric dependency
- Inverse of MP-07 (Shock-Redistribution): Shocks destroy fast, but rebuilding is slow and incomplete

**Source**: Extracted from GLP-1 cardiovascular study analysis (2026-03-20)

---

### MP-22 | Overextension Layer Lock-in

**Structure**
Layer N dominance → Resource concentration on N → Layer N+1 emerges → Structural inability to invest in N+1 → Competitors win at N+1 → Original dominant player collapses

Winning "too much" at the current layer of competition creates structural barriers to migrating to the next layer. Resources, organizational structure, success narratives, and sunk costs all lock the dominant player into the obsolescing layer.

**Generates**
- Incumbent disruption patterns
- "Innovator's Dilemma" dynamics
- Empire decline patterns
- Platform displacement
- Industry leadership inversion

**Observable Proxies**
- Increasing investment in current layer with diminishing returns
- "We're also investing in next-gen" rhetoric without proportional allocation
- Organizational structure optimized for current layer
- Dismissal of new layer as "not real" or "temporary trend"
- Layer N metrics improving while market position deteriorates
- Competitors weak at Layer N but strong at Layer N+1

**Structural Barriers (Why Winners Can't Move)**
1. **Sunk Cost Lock**: Hundreds of billions invested in current layer infrastructure
2. **Success Narrative Lock**: "This is what made us great" belief system
3. **Organizational Lock**: Promotions reward Layer N expertise; Layer N+1 advocates marginalized
4. **Financial Lock**: Current layer generates revenue; next layer requires investment

**Diagnostic Questions**
- "What layer is the current competition happening at?"
- "Is that layer saturating? What's the next layer up?"
- "Who is already operating at the higher layer?"
- "What percentage of R&D goes to current layer vs. next layer?"
- "Would the organization promote someone who succeeds at the next layer?"

**Differentiation from Related Patterns**
- MP-03 (Self-Undermining Success): Success changes conditions → same behavior fails
- **MP-22**: Success at Layer N → structural inability to move to Layer N+1
- MP-03 is about **condition change**; MP-22 is about **layer migration blockage**

**Example Instances**
1. Intel vs NVIDIA (2014-2024): Intel invested $165B in process miniaturization (Layer N: chip manufacturing). Stuck at 14nm for 7 years. NVIDIA invested in CUDA ecosystem (Layer N+1: AI infrastructure). Result: 42x market cap difference.
2. Japanese Department Stores (1991-2020): Peak ¥9.7T in floor space competition (Layer N). Amazon built logistics/data layer (Layer N+1). COVID revealed layer obsolescence.
3. British Empire (1870-1945): Colonial network dominance (Layer N). Germany/US invested in Second Industrial Revolution (Layer N+1: electricity, chemicals, mass production). Two world wars later, empire dissolved.
4. Newspaper Industry (2000-2020): Print advertising dominance (Layer N). Google/Facebook built targeting/data layer (Layer N+1). Ad revenue fell to 1/10 of peak.

**Mathematical Signature**
- Investment(Layer N) / Investment(Layer N+1) > 10:1 signals lock-in risk
- Market share(Layer N) inversely correlated with market share(Layer N+1)
- Time(Layer saturation to collapse) typically 7-15 years

**Source Gap**: V-01 (Overextension-Fragmentation) × MP-20 (Game Layer Migration)

**Source**: Discovered through gap analysis (2026-03-25)

---

### MP-23 | Knowledge Compound（知識複利）

**Structure**
Structure understanding A → enables Structure understanding B → enables C → ... (accelerating returns)

Unlike physical capital (depletes with use) or financial capital (linear returns), structural capital exhibits compound growth: understanding one structure makes recognizing the next easier. Creates accelerating returns to learning.

**Generates**
- Autodidact advantage patterns
- Expert generalist emergence
- Cross-domain innovation
- Learning efficiency curves
- "Rich get richer" knowledge dynamics

**Observable Proxies**
- Decreasing time to understand new domains
- Increasing frequency of cross-domain pattern recognition
- "This is like X" analogical reasoning
- Ability to extract structure from novel situations
- Teaching ability (can transmit structure, not just facts)

**Key Characteristics**

| Capital Type | Use Effect | Inheritance | Taxation |
|--------------|-----------|-------------|----------|
| Economic | Depletes | High | High |
| Social | Conditional | Medium | None |
| Cultural | Stable | Low | None |
| **Structural** | **Compounds** | **None** | **None** |

**Why Inheritance is Impossible**
1. **Experiential Dependency**: Structure recognition requires personal pattern-matching experience
2. **Active Construction**: Cannot be passively transferred; must be actively built
3. **Tacit Component**: Much of structural knowledge resists explicit articulation
4. **Individual Encoding**: Same structure is encoded differently in different minds

**Fukuzawa Connection**
> 「その違いは学ぶと学ばざるとによりてできるものなり」
> ──『学問のすゝめ』（1872年）

Fukuzawa identified this dynamic 152 years ago: the gap between people comes from learning vs. not learning. What he called "実学" (practical learning) is structural capital—understanding mechanisms, not memorizing facts.

**Example Instances**
1. Charlie Munger's "Mental Models": Explicitly collects structures across domains; reports accelerating ability to evaluate new businesses
2. Renaissance Polymaths: Leonardo da Vinci transferred structural understanding across painting, anatomy, engineering, architecture
3. Startup Serial Entrepreneurs: Second startup typically faster than first; structure of company-building transfers
4. Language Learning: Third language easier than second; meta-structure of language acquisition transfers

**Implications for Pedigree Leverage**
- Economic/social capital can be inherited → maintains class structure
- Structural capital cannot be inherited → creates escape path
- "Three generations to destroy wealth" → third generation lacks structural capital parents built
- **This is where the family lottery losers can win**

**Mathematical Signature**
- Learning time for domain N: T(N) = T(1) / log(N) approximately
- Cross-domain pattern recognition frequency: f(N) ∝ N²
- Teaching ability correlates with structural capital depth

**Source**: Day 40 (福沢諭吉×学問のすゝめ)

---

*End of Meta-Patterns v0.2.4*
*Updated: 2026-04-05*
*Pattern count: 23 (13 original + 10 discovered)*
