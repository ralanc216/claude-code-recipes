# SWOT and Strategic Framework Analysis

**Recipe #29: From Intuition to Structured Strategy**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 2-4 hours per analysis | Intermediate | Strategy, Executives, Consultants, Product Leaders |

---

## The Problem

Strategic thinking often happens informally—in hallway conversations, during long flights, or in exec meetings. But translating that thinking into structured analysis is hard. You know you need a SWOT or competitive analysis, but creating one that's actually insightful (not just checking a box) takes time. Generic frameworks produce generic outputs. You need analysis that drives real decisions.

**Pain Points:**
- Strategic frameworks feel like bureaucratic exercises
- SWOT analyses are done but not used
- Generic outputs don't drive specific action
- Hard to synthesize multiple perspectives
- Analysis paralysis from too many frameworks
- Disconnect between analysis and decisions

---

## The Outcome

Structured strategic analysis that generates genuine insights and actionable recommendations. Framework-based thinking that clarifies complex situations and points to specific actions. Analysis that decision-makers actually use.

**What You'll Have When Done:**
- Completed strategic framework analysis
- Actionable implications from each element
- Strategic options with evaluation
- Prioritized recommendations
- Communication-ready strategy summary

---

## When to Use This Recipe

**Good Fit:**
- Strategic planning processes
- Major business decisions
- Competitive positioning
- Market entry analysis
- New initiative evaluation
- Board and investor presentations

**Not a Good Fit:**
- Operational day-to-day decisions
- When the answer is already clear
- Academic exercises without decision context
- When data is completely unavailable

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have a clear strategic question or decision
- [ ] You have relevant background information
- [ ] You understand who will use the analysis
- [ ] You have 1-2 hours for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures framework analysis systematically
- Ensures completeness across framework elements
- Generates implications from analysis
- Connects analysis to recommendations
- Creates consistent documentation
- Applies multiple frameworks as needed

**Where Human Judgment Is Essential:**
- Validating insights against reality
- Adding non-obvious internal knowledge
- Political and cultural factors
- Strategic choices and trade-offs
- Commitment to action
- Final decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Strategic question | What you're trying to decide | Focus analysis |
| Company context | Your situation | Internal analysis |
| Market information | Industry dynamics | External analysis |
| Competitive data | Competitor information | Positioning |
| Stakeholder perspectives | What others think | Multiple viewpoints |

**Sample Input:**
```
Strategic Analysis Request

COMPANY: FreshMeal (meal delivery startup)
Stage: Series A, $8M ARR, growing 80% YoY
Market: Meal kit and prepared meal delivery

STRATEGIC QUESTION:
Should we expand from meal kits to prepared meals (heat-and-eat)?

CONTEXT:
Our current business:
- Premium meal kits, $15-20/serving
- Urban millennial professionals
- 60% repeat rate, strong NPS (65)
- Operations: Central kitchen + last-mile partners
- Differentiator: Chef-designed, restaurant-quality

Market dynamics:
- Meal kit market maturing, growth slowing
- Prepared meals growing faster (25% vs. 8%)
- HelloFresh struggling, Blue Apron declining
- New entrants in prepared meals (Factor, CookUnity)
- Customer trend toward less cooking time

Our capabilities:
- Strong culinary team and menu development
- Good logistics/delivery infrastructure
- Brand known for quality
- Limited capital ($5M runway)

Concerns:
- Prepared meals = different operations (cold chain)
- Lower margins? Higher volumes needed?
- Cannibalize existing customers?
- New competitive set

PERSPECTIVES:
- CEO: "We need growth, prepared meals is where market is going"
- VP Ops: "Operations are totally different, major investment needed"
- VP Marketing: "Our brand can stretch, but we'd need repositioning"
- Investors: "Prove you can win before market shifts"
```

---

## Step-by-Step Implementation

### Step 1: Define the Strategic Question
**Time: 10 minutes**

Be clear on:
- What decision are you trying to make?
- What's the scope of analysis?
- Who will use this analysis?
- What frameworks would be most useful?

A focused question leads to focused analysis.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Strategic Framework Analysis Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: SWOT and Strategic Framework Analysis**

```
Please conduct a comprehensive strategic framework analysis.

STRATEGIC QUESTION:
[What you're trying to decide or understand]

COMPANY/CONTEXT:
"""
[PASTE YOUR COMPANY AND SITUATION CONTEXT]
"""

MARKET/EXTERNAL CONTEXT:
"""
[PASTE MARKET AND COMPETITIVE INFORMATION]
"""

STAKEHOLDER PERSPECTIVES:
"""
[PASTE DIFFERENT VIEWPOINTS IF AVAILABLE]
"""

FRAMEWORKS TO APPLY:
[Select which are most relevant]
- SWOT Analysis
- Porter's Five Forces
- PESTEL Analysis
- Value Chain Analysis
- Ansoff Matrix
- McKinsey 7S
- BCG Matrix
- Blue Ocean Strategy

PLEASE PROVIDE:

1. SITUATION SUMMARY
   - Current state (1 paragraph)
   - Strategic question (clarified)
   - Key tensions or trade-offs

2. SWOT ANALYSIS

   **Strengths (Internal, Positive)**
   For each strength:
   - What it is
   - Evidence
   - Strategic implication

   **Weaknesses (Internal, Negative)**
   For each weakness:
   - What it is
   - Evidence
   - Strategic implication

   **Opportunities (External, Positive)**
   For each opportunity:
   - What it is
   - Why it matters
   - How we could capture it

   **Threats (External, Negative)**
   For each threat:
   - What it is
   - Potential impact
   - How we could address it

3. SWOT MATRIX STRATEGIES

   | | Strengths | Weaknesses |
   |---|---|---|
   | **Opportunities** | SO Strategies (use strengths to capture opportunities) | WO Strategies (address weaknesses to capture opportunities) |
   | **Threats** | ST Strategies (use strengths to counter threats) | WT Strategies (address weaknesses to avoid threats) |

4. [ADDITIONAL FRAMEWORK ANALYSIS]
   (Apply additional requested frameworks with same rigor)

5. KEY STRATEGIC INSIGHTS
   - What's most important from this analysis?
   - What's surprising or non-obvious?
   - What questions does this raise?

6. STRATEGIC OPTIONS
   Based on analysis, identify 3-4 strategic options:

   **Option A: [Name]**
   - Description
   - Alignment with SWOT
   - Pros
   - Cons
   - Risks
   - Resource requirements

   **Option B: [Name]**
   ...

7. OPTION EVALUATION
   | Criteria | Weight | Option A | Option B | Option C |

   Criteria might include:
   - Strategic fit
   - Financial attractiveness
   - Feasibility
   - Risk level
   - Time to impact

8. RECOMMENDATION
   - Recommended strategic direction
   - Rationale (tied to analysis)
   - Key success factors
   - Critical risks to manage
   - Immediate next steps

9. IMPLEMENTATION CONSIDERATIONS
   - What would need to be true for this to succeed?
   - Key milestones
   - Resource requirements
   - Governance needed

10. COMMUNICATION SUMMARY
    - One-page summary for stakeholders
    - Key message and supporting points
```

---

### Step 4: Review and Validate
**Time: 15-20 minutes**

Check the analysis:

**Validate SWOT elements:**
- Are strengths real (evidence-based)?
- Are weaknesses honest (not sugarcoated)?
- Are opportunities sized and realistic?
- Are threats properly weighted?

**Check logic:**
- Do strategies flow from analysis?
- Are options distinct and viable?
- Does recommendation align with analysis?

**Test insights:**
- Anything surprising?
- Did it surface what you know informally?
- Any blind spots?

---

### Step 5: Add Depth and Nuance
**Time: 15-20 minutes**

**To add perspective:**
```
The CEO perspective isn't fully reflected. Strengthen the analysis of why the prepared meal opportunity is compelling even given operational challenges.
```

**To challenge assumptions:**
```
Play devil's advocate on the recommendation. What would need to be true for Option B (stay focused on meal kits) to be the better choice?
```

**To add specific framework:**
```
Add a Porter's Five Forces analysis for the prepared meals market. How attractive is this market to enter?
```

**To strengthen implementation:**
```
If we proceed with prepared meals expansion, what are the 5 critical decisions we'd need to make in the first 90 days?
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create these final outputs:

1. STRATEGIC ANALYSIS DOCUMENT (5-7 pages)
   - Full SWOT and framework analysis
   - Options evaluation
   - Recommendation

2. EXECUTIVE SUMMARY (1 page)
   - Key findings
   - Recommendation
   - Next steps

3. BOARD PRESENTATION (8-10 slides)
   - Strategic question
   - Analysis highlights
   - Options
   - Recommendation
   - Discussion

4. DECISION BRIEF (2 pages)
   - Decision required
   - Options summary
   - Recommendation with rationale
   - Action items
```

---

## Example Output

Below is an abbreviated strategic framework analysis example:

---

> **STRATEGIC ANALYSIS: FreshMeal Expansion Decision**
> **Question: Should we expand into prepared meals?**
>
> ---
>
> **SITUATION SUMMARY**
>
> FreshMeal is a successful meal kit startup ($8M ARR, 80% growth) facing a strategic inflection point. The meal kit market is maturing while prepared meals grows faster. The company must decide whether to expand into prepared meals—a higher-growth segment that would require significant operational investment—or double down on meal kits where it has proven success but limited growth runway.
>
> **Key Tension:** Growth opportunity vs. operational complexity and capital constraints.
>
> ---
>
> **SWOT ANALYSIS**
>
> **STRENGTHS**
>
> | Strength | Evidence | Strategic Implication |
> |----------|----------|----------------------|
> | Culinary excellence | NPS 65, chef-designed menus | Transferable to prepared meals |
> | Strong brand equity | Premium positioning, loyal customers | Can stretch to new format |
> | Logistics infrastructure | Last-mile partnerships | Partially leverageable |
> | Repeat rate (60%) | Above industry average | Customer base for expansion |
>
> **WEAKNESSES**
>
> | Weakness | Evidence | Strategic Implication |
> |----------|----------|----------------------|
> | Limited capital | $5M runway | Constrains investment |
> | No cold chain expertise | Current ops don't require | Major capability gap |
> | Small team | Startup scale | Stretched capacity |
> | Single product line | All revenue from meal kits | Vulnerability |
>
> **OPPORTUNITIES**
>
> | Opportunity | Why It Matters | Capture Approach |
> |-------------|----------------|------------------|
> | Prepared meals growth (25% CAGR) | Larger, faster market | Expansion |
> | Customer behavior shift | Less cooking time wanted | Meet changing needs |
> | Competitor struggles | HelloFresh, Blue Apron weak | Take share |
> | Cross-sell to existing base | 60% repeat customers | Low-cost acquisition |
>
> **THREATS**
>
> | Threat | Impact | Mitigation |
> |--------|--------|------------|
> | Meal kit market decline | Core business at risk | Diversify |
> | Well-funded prepared meal competitors | Factor, CookUnity scaling | Move fast |
> | Operational execution risk | Could damage brand | Careful rollout |
> | Cannibalization | May lose kit customers | Positioning strategy |
>
> ---
>
> **SWOT MATRIX STRATEGIES**
>
> |  | Strengths | Weaknesses |
> |--|-----------|------------|
> | **Opportunities** | **SO: Brand-led expansion** — Use culinary reputation to enter prepared meals as premium player | **WO: Partnership model** — Partner for cold chain vs. build |
> | **Threats** | **ST: Preemptive move** — Enter prepared meals before meal kit decline accelerates | **WT: Focused pilot** — Test prepared meals with limited investment |
>
> ---
>
> **PORTER'S FIVE FORCES: Prepared Meals Market**
>
> | Force | Assessment | Implication |
> |-------|------------|-------------|
> | Buyer Power | Medium — some switching, but convenience sticky | Need differentiation beyond price |
> | Supplier Power | Low — commodity inputs | Favorable |
> | Threat of Substitutes | High — restaurants, grocery, DIY | Must be genuinely convenient |
> | Threat of New Entrants | Medium — capital needed, but not prohibitive | Must build moat |
> | Competitive Rivalry | Medium-High — growing, but not commoditized yet | Window of opportunity exists |
>
> **Market Attractiveness:** Moderate-Good. Growing market with competitive intensity but room for differentiated players.
>
> ---
>
> **STRATEGIC OPTIONS**
>
> **Option A: Full Prepared Meals Expansion**
>
> Launch prepared meals as second core product line in 6 months.
>
> - Investment: $3M (cold chain, new kitchen, team)
> - Expected impact: $4M+ additional ARR by Year 2
> - Pros: Largest growth potential, market timing
> - Cons: High capital use, execution risk
> - Risk level: High
>
> **Option B: Partnership-Led Expansion**
>
> Partner with existing prepared meal producer; white-label under FreshMeal brand.
>
> - Investment: $500K (brand, integration, marketing)
> - Expected impact: $2M additional ARR by Year 2
> - Pros: Lower capital, faster launch, reduced execution risk
> - Cons: Lower margins, less control, partner risk
> - Risk level: Medium
>
> **Option C: Double Down on Meal Kits**
>
> Focus exclusively on meal kits; capture share from struggling competitors.
>
> - Investment: $1M (marketing, expansion)
> - Expected impact: $3M additional ARR by Year 2
> - Pros: Focus, lower risk, known playbook
> - Cons: Market ceiling, long-term vulnerability
> - Risk level: Low-Medium
>
> **Option D: Prepared Meals Pilot**
>
> Launch limited prepared meal offering to test demand before full commitment.
>
> - Investment: $800K (limited cold chain, testing)
> - Expected impact: $500K ARR + learning
> - Pros: Learning with limited risk
> - Cons: May not achieve scale, competitor window
> - Risk level: Low
>
> ---
>
> **OPTION EVALUATION**
>
> | Criteria | Weight | Option A | Option B | Option C | Option D |
> |----------|--------|----------|----------|----------|----------|
> | Growth potential | 30% | 5 | 3 | 2 | 2 |
> | Capital efficiency | 25% | 2 | 4 | 4 | 4 |
> | Strategic fit | 20% | 5 | 3 | 3 | 4 |
> | Execution risk | 15% | 2 | 4 | 4 | 5 |
> | Speed to market | 10% | 3 | 4 | 5 | 3 |
> | **Weighted Score** | | **3.4** | **3.5** | **3.2** | **3.4** |
>
> ---
>
> **RECOMMENDATION: Option D → Option A (Staged Approach)**
>
> Begin with a prepared meals pilot (Option D), with clear milestones to graduate to full expansion (Option A) within 12 months.
>
> **Rationale:**
> 1. **Validates demand** before committing majority of capital
> 2. **Manages execution risk** while building capabilities
> 3. **Maintains optionality** if pilot signals go-to-market issues
> 4. **Still positions for first-mover** if successful
>
> **Stage Gates:**
> - Month 3: Pilot launch, 1 market, 3 prepared meal SKUs
> - Month 6: If NPS >50 and repeat >40%, expand to 2 markets
> - Month 9: If unit economics positive, trigger full build-out
> - Month 12: Full prepared meals launch
>
> **Key Success Factors:**
> 1. Cold chain partner quality for pilot phase
> 2. Menu translation (kit → prepared) preserves quality reputation
> 3. Pricing achieves minimum margins (35%+)
> 4. Existing customer adoption without cannibalization
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> FreshMeal should pursue prepared meals expansion, but through a staged approach that manages capital and execution risk. Begin with a focused pilot (3 SKUs, 1 market, partnership-enabled cold chain) with clear milestones to full rollout. This approach:
>
> - ✅ Captures the prepared meal growth opportunity
> - ✅ Manages capital constraints ($800K initial vs. $3M full build)
> - ✅ Tests key assumptions before full commitment
> - ✅ Maintains optionality if market doesn't develop as expected
>
> **Immediate Next Steps:**
> 1. Identify cold chain partners for pilot (Week 1-2)
> 2. Select pilot market (Week 2)
> 3. Develop pilot menu (Week 3-4)
> 4. Build measurement framework (Week 2-3)
> 5. Board approval for pilot investment (Week 4)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| SWOT is generic | Not enough specific context | Add: "Here are specific facts about our situation: [details]" |
| Analysis doesn't drive action | Disconnect from decisions | Ask: "What specific decisions does each element inform?" |
| Options all look similar | Not enough differentiation | Ask: "Make options more distinct—what's the most aggressive vs. conservative approach?" |
| Can't validate insights | Missing internal knowledge | Add: "Here's what we know from our experience: [insights]" |
| Recommendation feels weak | Not grounded in analysis | Ask: "Tie the recommendation explicitly to SWOT elements" |
| Too academic | Framework for framework's sake | Focus: "What are the 3 insights that actually matter for our decision?" |

---

## Tips from Experience

1. **Frameworks are means, not ends.** The goal is insight, not completed templates. Skip elements that don't add value.

2. **Specificity matters.** "Strong brand" is useless. "NPS of 65, 40% above industry average" drives decisions.

3. **Tensions reveal truth.** The most interesting strategic questions live in the conflict between SWOT elements.

4. **Challenge your strengths.** Every strength has a shadow weakness. Every opportunity has a hidden threat.

5. **Implications matter most.** Each SWOT element should connect to "so what?" and "now what?"

6. **Analysis without action is pointless.** Always end with specific recommendations and next steps.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Analysis generates genuine "aha" insights
- [ ] Decision-makers use the analysis
- [ ] Recommendations are specific and actionable
- [ ] Strategic choice is clearer after analysis
- [ ] Implementation follows from analysis

**Track over time:**
- Decisions influenced by strategic analysis
- Accuracy of strategic predictions
- Quality of strategic discussions
- Time from analysis to decision

---

## Variations

### Quick SWOT
For rapid strategic assessment:
```
Conduct a quick SWOT for:

[Situation description]

Provide:
- Top 3 strengths (with evidence)
- Top 3 weaknesses (with evidence)
- Top 3 opportunities (sized)
- Top 3 threats (weighted)
- Single most important strategic implication

Keep it under 1 page.
```

### Competitive Positioning Analysis
For market positioning:
```
Analyze competitive positioning for:

[Company and competitors]

Include:
1. Positioning map (2x2)
2. Differentiation analysis
3. Competitive advantage assessment
4. Positioning recommendations
5. Messaging implications
```

### Market Entry Analysis
For new market decisions:
```
Conduct market entry analysis for:

[Company] entering [Market]

Apply:
1. PESTEL analysis of target market
2. Porter's Five Forces for the market
3. Entry mode analysis (build/buy/partner)
4. Entry strategy recommendations
5. Go/no-go recommendation
```

### Strategic Options Generation
For brainstorming strategic alternatives:
```
Generate strategic options for:

[Strategic challenge]

Provide 5 distinct strategic options ranging from:
- Conservative (low risk, incremental)
- Moderate (balanced approach)
- Aggressive (high risk, transformational)

For each: description, pros, cons, risks, resource requirements.
```

---

## Building Your Repeatable System

After several strategic analyses, establish your system:

1. **Create a framework selection guide** for which tools when
2. **Build templates** for commonly used frameworks
3. **Maintain an insights library** from past analyses
4. **Establish review process** for strategic analysis quality
5. **Connect analysis to planning** processes

**Sample Setup:**
```
strategic-analysis/
├── templates/
│   ├── swot-prompt.txt
│   ├── five-forces-prompt.txt
│   └── strategy-framework-guide.md
├── analyses/
│   ├── 2024-prepared-meals/
│   │   ├── full-analysis.md
│   │   ├── executive-summary.md
│   │   └── presentation.pptx
│   └── archive/
├── frameworks/
│   ├── framework-selection-guide.md
│   └── framework-examples/
└── insights/
    └── strategic-lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**structure situation → apply frameworks → generate insights → develop options → recommend action**—applies broadly:

| Role | Application |
|------|-------------|
| **Strategy** | All strategic analysis and planning |
| **Executives** | Major business decisions |
| **Product** | Product strategy and roadmap |
| **Marketing** | Market positioning and planning |
| **Consultants** | Client strategic engagements |
| **Investors** | Investment analysis |

---

## Next Steps

1. **Identify a strategic question:** What decision needs analysis?
2. **Gather context:** Compile relevant information
3. **Run the analysis:** Apply appropriate frameworks
4. **Validate and refine:** Test insights against reality
5. **Drive to action:** Ensure recommendations are acted upon

---

*Recipe #29 of 100 in the Claude Code Knowledge Worker Recipe Collection*
