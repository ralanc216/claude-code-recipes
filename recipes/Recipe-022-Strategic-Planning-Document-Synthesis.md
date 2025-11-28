# Strategic Planning Document Synthesis

**Recipe #22: From Scattered Inputs to Cohesive Strategy**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 20 minutes (first time) / 15 minutes (repeat) | 15-25 hours per planning cycle | Advanced | Executives, Strategy Teams, Department Heads |

---

## The Problem

Strategic planning season means drowning in inputs—market research, financial data, competitive analysis, customer feedback, stakeholder interviews, industry trends. You have more information than you can possibly process, but you need to synthesize it into a coherent strategic plan with clear objectives, initiatives, and resource requirements. The analysis paralysis is real, and the deadline is immovable.

**Pain Points:**
- Too many inputs, not enough synthesis
- Difficulty connecting analysis to strategy
- Plans that are either too abstract or too tactical
- Lack of coherence across strategic elements
- Time pressure forcing rushed conclusions
- Multiple stakeholder perspectives to incorporate
- Strategy documents that sit on shelves unused

---

## The Outcome

A comprehensive strategic plan that synthesizes all your inputs into a coherent narrative with clear objectives, prioritized initiatives, resource requirements, and success metrics. A document that can guide decision-making and align the organization around shared priorities.

**What You'll Have When Done:**
- Strategic situation assessment
- Clear strategic objectives and priorities
- Initiative portfolio with rationale
- Resource and investment requirements
- Implementation roadmap
- Success metrics and governance
- Communication-ready strategy document

---

## When to Use This Recipe

**Good Fit:**
- Annual strategic planning
- Multi-year strategy development
- Major strategic pivots or transformations
- New leader strategic review
- Post-M&A strategy integration
- Investor/board strategy presentations

**Not a Good Fit:**
- Operational planning (too tactical)
- Quick strategic questions (overkill)
- When inputs haven't been gathered yet
- Daily business decisions

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have gathered key inputs (market research, financials, competitive, etc.)
- [ ] You understand the planning scope and time horizon
- [ ] Key stakeholder perspectives are documented
- [ ] You know the constraints (budget, capabilities, etc.)
- [ ] You have 4-6 hours for comprehensive strategy work

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Synthesizes multiple source documents
- Identifies themes and patterns across inputs
- Structures strategic frameworks
- Generates initiative portfolios
- Creates consistent strategic documentation
- Ensures logical flow and coherence

**Where Human Judgment Is Essential:**
- Strategic choices and trade-offs
- Political and organizational realities
- Resource allocation decisions
- Stakeholder buy-in and alignment
- Implementation feasibility
- Final strategic decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Market research | Industry reports, trend analysis | External context |
| Financial data | Historical performance, projections | Financial baseline |
| Competitive analysis | Competitive intelligence | Market positioning |
| Customer feedback | NPS data, customer interviews | Customer insight |
| Stakeholder input | Leadership interviews, surveys | Internal perspectives |
| Existing strategy | Current strategic plan | Starting point |

**Sample Input:**
```
Strategic Planning: FY2025 Corporate Strategy

Company: TechFlow (B2B SaaS, 500 employees, $80M ARR)
Planning horizon: 3 years (2025-2027)
Current situation: Growing 25% YoY but market is commoditizing

INPUTS PROVIDED:

1. Market Analysis (attached)
   - Market growing 15% annually
   - Consolidation happening (3 acquisitions this year)
   - AI disruption accelerating
   - Customer expectations rising

2. Financial Performance
   - ARR: $80M (25% growth)
   - Gross margin: 72%
   - Net retention: 110%
   - CAC payback: 18 months
   - Cash: $40M, runway 24+ months

3. Competitive Landscape
   - 2 well-funded competitors gaining share
   - Legacy vendors struggling
   - New AI-native entrants emerging

4. Customer Feedback Summary
   - NPS: 42 (good but declining)
   - Top requests: AI features, better integrations, mobile
   - Churn reasons: Competition, changing needs, price

5. Leadership Input Summary
   - CEO: Focus on sustainable growth, AI is priority
   - CFO: Improve unit economics before scaling
   - CTO: Need platform modernization, tech debt high
   - CRO: Market window closing, need to move faster
   - CPO: Product differentiation eroding

Constraints:
- Cannot raise capital in current market
- Headcount growth limited to 15%
- Must maintain profitability path
```

---

## Step-by-Step Implementation

### Step 1: Organize Your Inputs
**Time: 30-60 minutes**

Gather and organize all strategic inputs:
- Save documents in an accessible location
- Summarize key points from each source
- Note areas of agreement and tension
- Identify gaps in your information

The quality of synthesis depends on input quality.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
cd ~/Documents/strategic-planning
claude
```

---

### Step 3: Run the Strategic Synthesis Prompt
**Time: 15-20 minutes for Claude to process**

---

**PRIMARY PROMPT: Strategic Planning Document Synthesis**

```
Help me synthesize strategic inputs into a comprehensive strategic plan.

CONTEXT:
- Organization: [Name and description]
- Planning horizon: [Time period]
- Current situation: [Brief summary]
- Key challenge/opportunity: [Central strategic question]

STRATEGIC INPUTS:

1. MARKET ANALYSIS:
"""
[Paste market research summary or key points]
"""

2. FINANCIAL PERFORMANCE:
"""
[Paste financial data and trends]
"""

3. COMPETITIVE LANDSCAPE:
"""
[Paste competitive analysis]
"""

4. CUSTOMER INSIGHTS:
"""
[Paste customer feedback summary]
"""

5. STAKEHOLDER PERSPECTIVES:
"""
[Paste leadership/stakeholder input]
"""

6. CURRENT STRATEGY:
"""
[Paste current strategic priorities if any]
"""

CONSTRAINTS:
- [Financial constraints]
- [Resource constraints]
- [Capability constraints]
- [Timeline constraints]

PLEASE SYNTHESIZE INTO:

1. EXECUTIVE SUMMARY
   - Strategic situation in 1 paragraph
   - Core strategic thesis
   - Key choices we're making
   - Expected outcomes

2. STRATEGIC SITUATION ASSESSMENT
   - Market context and trends
   - Competitive position
   - Internal capabilities and gaps
   - Key strategic issues to address
   - SWOT or appropriate framework

3. STRATEGIC VISION AND OBJECTIVES
   - Where we're going (3-year vision)
   - How we'll win (strategic positioning)
   - 3-5 strategic objectives with:
     * Clear statement
     * Rationale (why this objective)
     * Success metrics
     * Time horizon

4. STRATEGIC PRIORITIES AND INITIATIVES
   For each strategic objective:
   - Key initiatives required
   - Initiative description and scope
   - Resource requirements
   - Dependencies
   - Timeline
   - Success criteria

5. RESOURCE AND INVESTMENT PLAN
   - Investment required by initiative
   - Capability gaps to address
   - Headcount implications
   - Technology investments
   - Trade-offs and choices

6. IMPLEMENTATION ROADMAP
   - Phase 1 (Year 1): Focus and priorities
   - Phase 2 (Year 2): Scaling and expansion
   - Phase 3 (Year 3): Optimization and growth
   - Key milestones and gates

7. RISK AND CONTINGENCY
   - Strategic risks identified
   - Risk mitigation approaches
   - Contingency triggers
   - Alternative scenarios

8. GOVERNANCE AND TRACKING
   - How we'll track progress
   - Review cadence
   - Decision rights
   - Accountability structure

9. COMMUNICATION PLAN
   - Key messages by audience
   - Communication timeline
   - Engagement approach

Format as a comprehensive strategic planning document.
```

---

### Step 4: Review and Challenge
**Time: 45-60 minutes**

Critically evaluate the strategic synthesis:

**Logic check:**
- Does the strategy flow from the analysis?
- Are objectives SMART and achievable?
- Are initiatives properly scoped?
- Do investments match priorities?

**Coherence check:**
- Does everything connect?
- Are there contradictions?
- Does it tell a compelling story?

**Reality check:**
- Can we actually execute this?
- Are the trade-offs clear?
- What are we choosing NOT to do?

---

### Step 5: Refine Strategic Elements
**Time: 30-45 minutes**

**To strengthen the strategic thesis:**
```
The strategic thesis feels too generic. Make it more specific and differentiated—what are we uniquely choosing to do that competitors won't or can't?
```

**To clarify trade-offs:**
```
What are we explicitly choosing NOT to do in this strategy? Make the trade-offs explicit and explain why we're making these choices.
```

**To improve initiative definition:**
```
Initiative 2 (Platform Modernization) is too vague. Break it into specific workstreams with clearer scope and deliverables.
```

**To stress-test the plan:**
```
Play devil's advocate: What could go wrong with this strategy? What are the biggest risks and how would we know early if it's not working?
```

**To add scenario planning:**
```
Create three scenarios: optimistic, baseline, and pessimistic. Show how our strategy adapts in each scenario.
```

---

### Step 6: Finalize Deliverables
**Time: 30 minutes**

```
Create these final outputs:

1. FULL STRATEGIC PLAN (20-30 pages)
   - Complete document with all sections
   - Appendices with supporting data
   - Professional formatting

2. EXECUTIVE PRESENTATION (15-20 slides)
   - Board/leadership presentation format
   - Key messages and visuals
   - Discussion questions for approval

3. ONE-PAGE STRATEGY SUMMARY
   - Single page that captures essence
   - Suitable for all-hands communication
   - Clear, memorable, actionable

4. STRATEGY SCORECARD
   - Key metrics to track
   - Targets for each period
   - Owner assignments
```

---

## Example Output

Below is an abbreviated strategic plan example:

---

> **TECHFLOW STRATEGIC PLAN: 2025-2027**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> TechFlow faces a strategic inflection point: strong market position and healthy growth (25% YoY) are threatened by commoditization, well-funded competitors, and AI disruption. Our strategic response is to **transform from a feature-led product company to an AI-powered platform company**, creating sustainable differentiation through intelligence, extensibility, and ecosystem value.
>
> **Core Strategic Thesis:**
> We will win by becoming the AI-native platform that turns customer data into actionable intelligence, while competitors compete on features we pioneered. We're betting that customers will pay a premium for outcomes over outputs.
>
> **Key Strategic Choices:**
> 1. Invest heavily in AI (25% of R&D) despite short-term margin pressure
> 2. Build platform/ecosystem vs. point solution features
> 3. Move upmarket to enterprise vs. protecting SMB base
> 4. Partner for integration vs. build everything ourselves
>
> **Expected Outcomes (2027):**
> - ARR: $150M (25% CAGR maintained)
> - AI-powered revenue: 40% of new ARR
> - Enterprise mix: 50% (from 30%)
> - Net retention: 125% (from 110%)
>
> ---
>
> **STRATEGIC SITUATION ASSESSMENT**
>
> **Market Context:**
> - TAM growing 15% annually to $8B by 2027
> - AI integration becoming table stakes
> - Consolidation accelerating (5 acquisitions expected in 24 months)
> - Customer expectations outpacing product evolution
>
> **Competitive Position:**
> | Dimension | Our Position | Trend |
> |-----------|--------------|-------|
> | Market share | #3 (12%) | Stable |
> | Product perception | Strong but aging | ⬇️ Declining |
> | Brand/trust | High | Stable |
> | Technology | Capable but debt-laden | ⬇️ At risk |
> | Team | Strong but stretched | Stable |
>
> **SWOT Analysis:**
>
> | Strengths | Weaknesses |
> |-----------|------------|
> | Customer relationships | Technical debt |
> | Domain expertise | AI capabilities |
> | Cash position | Enterprise sales motion |
> | Brand reputation | Platform extensibility |
>
> | Opportunities | Threats |
> |--------------|---------|
> | AI transformation | Well-funded competitors |
> | Platform play | Market commoditization |
> | Enterprise segment | AI-native entrants |
> | Ecosystem/partners | Talent competition |
>
> ---
>
> **STRATEGIC OBJECTIVES**
>
> **Objective 1: Become the AI-Intelligent Platform**
> *Transform our product from workflow tool to intelligence platform*
>
> - **Rationale:** AI is the only sustainable differentiation; features get copied in 6-12 months
> - **Success Metrics:**
>   - 3+ AI features in production by Q4 2025
>   - AI-influenced revenue: 40% of new ARR by 2027
>   - AI NPS above 50
> - **Timeline:** 18 months to platform parity, 36 months to leadership
>
> **Objective 2: Win in Enterprise**
> *Shift revenue mix from SMB-heavy to enterprise-led*
>
> - **Rationale:** Enterprise has higher LTV, stickier relationships, and ability to pay for value
> - **Success Metrics:**
>   - Enterprise revenue: 50% of ARR by 2027 (from 30%)
>   - Average contract value: $150K (from $80K)
>   - Logo acquisition: 50 enterprise logos/year
> - **Timeline:** Motion changes in 2025, mix shift visible by 2026
>
> **Objective 3: Build the Platform Ecosystem**
> *Create an integration and partner ecosystem that increases switching costs*
>
> - **Rationale:** Platforms win; point solutions get displaced
> - **Success Metrics:**
>   - 25+ active integrations
>   - Partner-sourced revenue: 20% of new ARR
>   - Developer community: 5,000 active developers
> - **Timeline:** Foundation in 2025, acceleration in 2026-2027
>
> ---
>
> **STRATEGIC INITIATIVES**
>
> | Initiative | Objective | Investment | Timeline | Owner |
> |------------|-----------|------------|----------|-------|
> | AI Platform Build | 1 | $6M | 2025-2026 | CTO |
> | Enterprise Sales Motion | 2 | $4M | 2025 | CRO |
> | Platform & API Overhaul | 3 | $5M | 2025-2026 | CPO |
> | Technical Debt Reduction | All | $3M | 2025 | CTO |
> | Partner Program Launch | 3 | $2M | 2025 | CEO |
>
> ---
>
> **IMPLEMENTATION ROADMAP**
>
> **Phase 1 (2025): Foundation**
> - Q1-Q2: AI team formation, platform architecture
> - Q2-Q3: Enterprise pilot program, first AI feature
> - Q3-Q4: Partner program launch, platform beta
>
> **Phase 2 (2026): Acceleration**
> - Full AI suite launch
> - Enterprise sales team at scale
> - Platform GA with developer ecosystem
>
> **Phase 3 (2027): Leadership**
> - Market-leading AI capabilities
> - 50% enterprise revenue
> - Thriving ecosystem
>
> ---
>
> **RISKS AND CONTINGENCIES**
>
> | Risk | Likelihood | Impact | Mitigation |
> |------|------------|--------|------------|
> | AI execution failure | Medium | High | Stage-gate approach, partner backup |
> | Enterprise sales miss | Medium | Medium | Maintain SMB growth, adjust pace |
> | Competitor acquisition | High | High | Speed of execution, customer lock-in |
> | Talent gap | Medium | High | Aggressive hiring, acqui-hire options |
>
> **Contingency Triggers:**
> - If AI revenue <10% by end 2025 → reassess approach, consider acquisition
> - If enterprise sales <70% of target → slow investment, protect SMB
> - If major competitor acquired → accelerate timeline, consider capital raise

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Strategy too generic | Inputs too high-level | Add: "What specific choices are we making that competitors aren't?" |
| Can't reconcile conflicting inputs | Stakeholder disagreement captured | Ask: "Which perspective should take priority and why?" |
| Initiatives too vague | Insufficient scoping | Ask: "Break this initiative into specific workstreams with deliverables" |
| Resource requirements unclear | Not quantified | Ask: "What specific headcount, budget, and technology investments are required?" |
| Strategy feels disconnected from analysis | Logic gap | Ask: "Show the explicit connection between analysis findings and strategic choices" |
| Too many priorities | Lack of focus | Ask: "If we could only do 3 things, what would they be and why?" |

---

## Tips from Experience

1. **Strategy is about choice.** A strategy that tries to do everything is not a strategy. Make the trade-offs explicit.

2. **Start with the problem.** What are we solving? Why does the current approach not work? Ground strategy in reality.

3. **Connect analysis to action.** Every strategic initiative should trace back to a finding in your situation assessment.

4. **Test with scenarios.** Ask "what if we're wrong?" and ensure the strategy has enough flexibility.

5. **Communicate, communicate, communicate.** A strategy no one knows about is not a strategy. Plan for communication.

6. **Build in checkpoints.** Strategy isn't static. Plan for quarterly reviews and adjustment triggers.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Strategy is coherent—everything connects
- [ ] Trade-offs are explicit—what we're NOT doing is clear
- [ ] Initiatives have clear scope and owners
- [ ] Resources are allocated to match priorities
- [ ] Leadership can articulate the strategy consistently

**Track over time:**
- Initiative progress against milestones
- Strategic metrics vs. targets
- Resource allocation vs. plan
- Employee understanding of strategy (survey)
- Competitor response to our moves

---

## Variations

### Functional/Department Strategy
For a department strategic plan:
```
Help me develop a functional strategy for [Department].

Corporate strategy context: [Company's strategic priorities]
Department scope: [What we own]
Current performance: [How we're doing]
Challenges: [Key issues]

Create a department strategic plan that:
1. Aligns to corporate strategy
2. Addresses department-specific challenges
3. Includes capability building
4. Has clear metrics and initiatives
```

### Strategic Pivot/Transformation
For a major strategic change:
```
Help me plan a strategic pivot.

Current state: [Where we are today]
Why change is needed: [Forcing function]
Desired end state: [Where we need to be]
Constraints: [What we can't change]

Develop a transformation plan including:
1. Strategic rationale for the pivot
2. End-state vision
3. Transition approach
4. Risk management
5. Change management
6. Success metrics
```

### Quick Strategy Refresh
For updating existing strategy:
```
Help me refresh our strategic plan.

Current strategy: [Paste existing]
What's changed: [New information, results, context]
Remaining valid: [What still holds]

Provide:
1. Assessment of what needs to change
2. Recommended adjustments
3. Updated priorities
4. Communication of changes
```

### M&A Strategic Rationale
For acquisition strategy:
```
Help me develop strategic rationale for [acquisition/merger].

Our company: [Description]
Target company: [Description]
Strategic fit hypothesis: [Why this makes sense]

Develop:
1. Strategic rationale
2. Synergy analysis
3. Integration considerations
4. Risk assessment
5. Alternative approaches considered
6. Recommendation
```

---

## Building Your Repeatable System

After several planning cycles, establish your system:

1. **Create an input collection framework** ensuring consistent data
2. **Build a strategic planning calendar** with key milestones
3. **Maintain strategic templates** for consistency
4. **Establish review cadence** for strategy tracking
5. **Document lessons learned** from each cycle

**Sample Setup:**
```
strategic-planning/
├── templates/
│   ├── strategic-plan-prompt.txt
│   ├── initiative-template.md
│   └── scorecard-template.xlsx
├── inputs/
│   ├── market-research/
│   ├── financial-data/
│   ├── competitive-analysis/
│   └── stakeholder-input/
├── plans/
│   ├── FY2025/
│   │   ├── strategic-plan-v1.md
│   │   ├── executive-presentation.pptx
│   │   └── scorecard.xlsx
│   └── archive/
└── tracking/
    └── quarterly-reviews/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**gather diverse inputs → synthesize patterns → develop coherent strategy → plan execution → create communication**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Corporate and business unit strategy |
| **Department Heads** | Functional strategies |
| **Product Leaders** | Product strategy and roadmap |
| **Consultants** | Client strategic engagements |
| **Investors** | Portfolio strategy |
| **Board Members** | Strategic oversight |

---

## Next Steps

1. **Gather your inputs:** Compile the sources you'll need
2. **Set aside time:** Block 4-6 hours for deep strategic work
3. **Engage stakeholders:** Get their input before synthesizing
4. **Run the synthesis:** Use this recipe to create your plan
5. **Iterate and refine:** Review with key leaders before finalizing

---

*Recipe #22 of 100 in the Claude Code Knowledge Worker Recipe Collection*
