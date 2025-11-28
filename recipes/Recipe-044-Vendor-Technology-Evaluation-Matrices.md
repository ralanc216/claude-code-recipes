# Vendor/Technology Evaluation Matrices

**Recipe #44: From Scattered Information to Structured Decisions**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 4-6 hours per evaluation | Intermediate | Procurement, IT, Operations, Project Managers |

---

## The Problem

Choosing vendors or technologies is high-stakes but often poorly structured. Teams gather demos, proposals, and research, but the evaluation process is messy. Each stakeholder weights criteria differently. Comparisons are incomplete. The loudest voice or best salesperson wins, not the best solution. After the decision, nobody can clearly explain why one option beat another—making it hard to defend the choice or learn from it.

**Pain Points:**
- No standardized evaluation framework
- Apples-to-oranges comparisons
- Stakeholder bias and politics
- Missing information from some vendors
- Decisions that can't be justified
- Analysis paralysis from too much data
- Post-decision regret and "what ifs"

---

## The Outcome

A structured, defensible evaluation framework with weighted scoring, clear criteria, and documented rationale. A recommendation that stakeholders can understand and support, with transparent methodology that survives scrutiny.

**What You'll Have When Done:**
- Weighted evaluation matrix
- Normalized scores across options
- Clear comparison on each criterion
- Risk assessment for each option
- Recommendation with rationale
- Decision documentation for future reference

---

## When to Use This Recipe

**Good Fit:**
- Software and SaaS vendor selection
- Technology platform decisions
- Service provider evaluation
- Hardware and equipment procurement
- Professional services firm selection
- Partnership evaluations

**Not a Good Fit:**
- Simple, low-cost purchases
- Single-source situations
- Emergency procurement (no time)
- Highly political decisions (evaluation won't matter)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have requirements documented
- [ ] You have vendor/option information collected
- [ ] Key stakeholders have agreed on criteria
- [ ] You have 2-4 hours for evaluation development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures evaluation frameworks
- Creates weighted scoring matrices
- Normalizes diverse information
- Identifies gaps in evaluation data
- Generates comparison narratives
- Highlights strengths and weaknesses

**Where Human Judgment Is Essential:**
- Criteria selection and weighting
- Requirements prioritization
- Information verification
- Political and relationship factors
- Final decision making
- Stakeholder alignment

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Requirements | What you need | Evaluation criteria |
| Vendor info | Proposals, demos, research | Scoring input |
| Stakeholder priorities | Who cares about what | Weight calibration |
| Budget constraints | Financial parameters | Cost analysis |
| Risk factors | What could go wrong | Risk assessment |

**Sample Input:**
```
Vendor Evaluation Request

PROJECT: Marketing Automation Platform Selection

BUSINESS CONTEXT:
- Replacing aging email marketing tool
- Need to scale from 50K to 500K contacts
- Integration with Salesforce CRM critical
- Team of 5 marketers, 1 admin
- Budget: $50-80K annually

VENDORS TO EVALUATE:
1. HubSpot Marketing Hub (Professional)
2. Marketo (Adobe)
3. Pardot (Salesforce)
4. ActiveCampaign

INFORMATION GATHERED:
[For each vendor, include: pricing, capabilities, proposal details, demo notes, references]

REQUIREMENTS (from stakeholders):

Must-Have:
- Email marketing with dynamic content
- Lead scoring and nurturing
- Salesforce bi-directional sync
- Landing page builder
- A/B testing
- GDPR compliance

Nice-to-Have:
- Social media scheduling
- SMS capabilities
- Advanced analytics
- AI recommendations
- Account-based marketing features

STAKEHOLDER PRIORITIES:
- Marketing Director: Ease of use, reporting
- Marketing Ops: Integrations, reliability
- Sales Leadership: Salesforce sync, lead quality
- IT: Security, supportability
- Finance: Total cost, contract flexibility

EVALUATION WEIGHTS (initial thoughts):
- Functionality: 30%
- Ease of use: 20%
- Integration: 20%
- Cost: 15%
- Vendor stability: 10%
- Implementation: 5%

CONCERNS:
- HubSpot: Will we outgrow it? Enterprise features?
- Marketo: Complexity, cost
- Pardot: Mixed reviews on UI, limited outside Salesforce
- ActiveCampaign: Enterprise readiness, scalability
```

---

## Step-by-Step Implementation

### Step 1: Define Evaluation Criteria
**Time: 15-20 minutes**

Work with stakeholders to:
- List all evaluation criteria
- Categorize into groups
- Assign weights reflecting true priorities
- Define scoring scale (usually 1-5)
- Clarify what each score means

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Evaluation Matrix Prompt
**Time: 7-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Vendor/Technology Evaluation Matrix**

```
Please help me create a vendor evaluation matrix.

PROJECT CONTEXT:
[What you're evaluating and why]

OPTIONS TO EVALUATE:
1. [Option A]
2. [Option B]
3. [Option C]
(etc.)

REQUIREMENTS:
Must-Have:
[List must-have requirements]

Nice-to-Have:
[List nice-to-have requirements]

STAKEHOLDER PRIORITIES:
[Who cares about what]

PROPOSED CRITERIA AND WEIGHTS:
[Your initial criteria categories and weightings]

INFORMATION GATHERED FOR EACH OPTION:
[Paste relevant information: proposals, pricing, capabilities, demo notes]

BUDGET PARAMETERS:
[Financial constraints]

PLEASE CREATE:

1. EVALUATION FRAMEWORK

   Finalize criteria structure:

   | Category | Weight | Sub-Criteria |
   |----------|--------|--------------|

   Define scoring scale:
   - 5 = Exceeds requirements
   - 4 = Fully meets requirements
   - 3 = Adequately meets requirements
   - 2 = Partially meets requirements
   - 1 = Does not meet requirements
   - 0 = Missing/Not applicable

2. DETAILED SCORING MATRIX

   For each option, score each criterion:

   | Criterion | Weight | Option A | Option B | Option C | Notes |
   |-----------|--------|----------|----------|----------|-------|

   Include:
   - Raw scores (1-5)
   - Weighted scores
   - Category subtotals
   - Overall total

3. MUST-HAVE REQUIREMENTS CHECK

   | Requirement | Option A | Option B | Option C |
   |-------------|----------|----------|----------|
   (Pass/Fail for each)

   Note: Any option failing a must-have should be eliminated or flagged

4. COMPARATIVE ANALYSIS

   For each criterion category:
   - Which option leads and why
   - Key differentiators
   - Where options are comparable
   - Notable strengths and weaknesses

5. COST ANALYSIS

   | Cost Element | Option A | Option B | Option C |
   |--------------|----------|----------|----------|
   | Year 1       |          |          |          |
   | Year 2       |          |          |          |
   | Year 3       |          |          |          |
   | 3-Year Total |          |          |          |
   | Hidden Costs |          |          |          |

6. RISK ASSESSMENT

   For each option:
   | Risk | Likelihood | Impact | Mitigation |

   Overall risk rating (Low/Medium/High)

7. STAKEHOLDER ALIGNMENT

   | Stakeholder Group | Preferred Option | Why |

   Note any conflicts or concerns

8. SENSITIVITY ANALYSIS

   - What if we changed weight on [criteria]?
   - Does any option dominate regardless of weighting?
   - Where is the decision most sensitive?

9. RECOMMENDATION

   - Recommended option with rationale
   - Second choice and when it would be preferred
   - Key risks to monitor
   - Implementation considerations

10. DECISION DOCUMENTATION

    Summary for approval:
    - Process followed
    - Options evaluated
    - Key findings
    - Recommendation and rationale
    - Approvals needed

Be objective and base scores on documented evidence where possible.
```

---

### Step 4: Review and Validate Scoring
**Time: 20-30 minutes**

For each score:
- Does evidence support this score?
- Are scores consistent across options?
- Are there gaps in information?
- Do stakeholders agree with the assessment?

---

### Step 5: Refine the Analysis
**Time: 15-20 minutes**

**To adjust scoring:**
```
I think the score for [Option X] on [Criterion Y] is too high/low. Here's why: [evidence]. Please adjust and recalculate.
```

**To add nuance:**
```
The [category] scoring doesn't capture an important distinction: [detail]. How should we factor this in?
```

**To explore alternatives:**
```
Run a sensitivity analysis: What if we weighted [criterion] at 30% instead of 20%? Does the recommendation change?
```

**To address gaps:**
```
We're missing information on [aspect] for [Option]. What questions should we ask to complete the evaluation?
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create the final evaluation package:

1. EXECUTIVE SUMMARY (1 page)
   - Options evaluated
   - Key findings
   - Recommendation
   - Critical success factors

2. DETAILED EVALUATION MATRIX
   - Complete scoring with notes
   - Supporting evidence references

3. PRESENTATION DECK OUTLINE
   - For stakeholder presentation
   - Key slides needed
   - Talking points

4. DECISION RECORD
   - For documentation/audit
   - Process followed
   - Rationale captured

5. NEXT STEPS
   - Implementation planning
   - Contract negotiation priorities
   - Stakeholder communications
```

---

## Example Output

Below is an abbreviated evaluation matrix example:

---

> **MARKETING AUTOMATION PLATFORM EVALUATION**
>
> ---
>
> ## Executive Summary
>
> **Evaluated Options:** HubSpot Marketing Hub, Marketo, Pardot, ActiveCampaign
>
> **Recommendation:** HubSpot Marketing Hub (Professional)
>
> **Rationale:** HubSpot scored highest overall (4.2/5.0) with particular strengths in ease of use, implementation speed, and total cost of ownership. While Marketo offers more advanced enterprise features, the complexity and cost premium don't align with our current scale and team capabilities. Pardot would be the choice if deeper Salesforce integration justifies the trade-offs in flexibility.
>
> **Key Findings:**
> - All options meet must-have requirements
> - HubSpot and ActiveCampaign lead on ease of use
> - Marketo leads on advanced features but with significant complexity
> - Pardot offers best Salesforce integration but limited standalone capability
> - 3-year TCO ranges from $138K (ActiveCampaign) to $312K (Marketo)
>
> ---
>
> ## Evaluation Framework
>
> | Category | Weight | Sub-Criteria |
> |----------|--------|--------------|
> | Functionality | 30% | Core features, advanced features, scalability |
> | Ease of Use | 20% | UI/UX, learning curve, team adoption |
> | Integration | 20% | Salesforce sync, other integrations, API |
> | Cost | 15% | License, implementation, ongoing |
> | Vendor Stability | 10% | Company strength, product roadmap, support |
> | Implementation | 5% | Timeline, resources, risk |
>
> **Scoring Scale:**
> - 5 = Exceeds requirements significantly
> - 4 = Fully meets requirements
> - 3 = Adequately meets requirements
> - 2 = Partially meets requirements
> - 1 = Does not meet requirements
>
> ---
>
> ## Detailed Scoring Matrix
>
> | Criterion | Weight | HubSpot | Marketo | Pardot | ActiveCampaign |
> |-----------|--------|---------|---------|--------|----------------|
> | **FUNCTIONALITY** | **30%** | | | | |
> | Core email features | 10% | 5 | 5 | 4 | 4 |
> | Lead scoring/nurturing | 10% | 4 | 5 | 4 | 3 |
> | Scalability | 5% | 4 | 5 | 4 | 3 |
> | Advanced features | 5% | 3 | 5 | 3 | 2 |
> | *Category Subtotal* | | **4.1** | **5.0** | **3.8** | **3.1** |
> | | | | | | |
> | **EASE OF USE** | **20%** | | | | |
> | User interface | 10% | 5 | 3 | 3 | 5 |
> | Learning curve | 5% | 5 | 2 | 3 | 5 |
> | Admin complexity | 5% | 4 | 2 | 3 | 4 |
> | *Category Subtotal* | | **4.8** | **2.5** | **3.0** | **4.8** |
> | | | | | | |
> | **INTEGRATION** | **20%** | | | | |
> | Salesforce sync | 10% | 4 | 4 | 5 | 3 |
> | Other integrations | 5% | 5 | 4 | 3 | 4 |
> | API capability | 5% | 4 | 5 | 3 | 3 |
> | *Category Subtotal* | | **4.3** | **4.3** | **4.0** | **3.3** |
> | | | | | | |
> | **COST** | **15%** | | | | |
> | License cost | 8% | 4 | 2 | 3 | 5 |
> | Implementation cost | 4% | 4 | 2 | 3 | 4 |
> | Total cost of ownership | 3% | 4 | 2 | 3 | 5 |
> | *Category Subtotal* | | **4.0** | **2.0** | **3.0** | **4.8** |
> | | | | | | |
> | **VENDOR STABILITY** | **10%** | | | | |
> | Company financials | 5% | 5 | 5 | 5 | 4 |
> | Product roadmap | 3% | 5 | 4 | 4 | 4 |
> | Support quality | 2% | 4 | 3 | 4 | 4 |
> | *Category Subtotal* | | **4.8** | **4.2** | **4.4** | **4.0** |
> | | | | | | |
> | **IMPLEMENTATION** | **5%** | | | | |
> | Timeline | 2% | 4 | 2 | 3 | 5 |
> | Resources required | 2% | 4 | 2 | 3 | 4 |
> | Risk | 1% | 4 | 3 | 4 | 4 |
> | *Category Subtotal* | | **4.0** | **2.3** | **3.3** | **4.5** |
>
> ---
>
> ## Overall Scores
>
> | Option | Weighted Score | Rank |
> |--------|---------------|------|
> | **HubSpot** | **4.2** | **1** |
> | ActiveCampaign | 3.8 | 2 |
> | Pardot | 3.5 | 3 |
> | Marketo | 3.4 | 4 |
>
> ---
>
> ## Must-Have Requirements Check
>
> | Requirement | HubSpot | Marketo | Pardot | ActiveCampaign |
> |-------------|---------|---------|--------|----------------|
> | Email with dynamic content | ✅ | ✅ | ✅ | ✅ |
> | Lead scoring/nurturing | ✅ | ✅ | ✅ | ✅ |
> | Salesforce bi-directional sync | ✅ | ✅ | ✅ | ⚠️ Limited |
> | Landing page builder | ✅ | ✅ | ✅ | ✅ |
> | A/B testing | ✅ | ✅ | ✅ | ✅ |
> | GDPR compliance | ✅ | ✅ | ✅ | ✅ |
>
> **Note:** ActiveCampaign Salesforce integration is functional but less robust than competitors. Evaluate whether depth of integration is truly must-have.
>
> ---
>
> ## Cost Analysis (3-Year TCO)
>
> | Cost Element | HubSpot | Marketo | Pardot | ActiveCampaign |
> |--------------|---------|---------|--------|----------------|
> | Year 1 License | $57,600 | $72,000 | $60,000 | $42,000 |
> | Year 2 License | $57,600 | $79,200 | $63,000 | $42,000 |
> | Year 3 License | $57,600 | $87,120 | $66,150 | $42,000 |
> | Implementation | $15,000 | $50,000 | $25,000 | $8,000 |
> | Training | $5,000 | $15,000 | $8,000 | $4,000 |
> | Ongoing Support | Included | $8,000/yr | Included | Included |
> | **3-Year Total** | **$192,800** | **$312,320** | **$230,150** | **$138,000** |
>
> ---
>
> ## Risk Assessment
>
> | Option | Key Risks | Likelihood | Impact | Overall |
> |--------|-----------|------------|--------|---------|
> | **HubSpot** | May need upgrade to Enterprise within 2 years | Medium | Medium | 🟡 Medium |
> | **Marketo** | Complexity leads to underutilization | High | Medium | 🟡 Medium |
> | **Pardot** | Limited flexibility outside Salesforce ecosystem | Medium | Medium | 🟡 Medium |
> | **ActiveCampaign** | Scalability concerns at 500K contacts | Medium | High | 🟡 Medium |
>
> ---
>
> ## Stakeholder Alignment
>
> | Stakeholder | Preferred Option | Notes |
> |-------------|-----------------|-------|
> | Marketing Director | HubSpot | Values ease of use and reporting |
> | Marketing Ops | HubSpot or Marketo | Wants power but concerned about Marketo complexity |
> | Sales Leadership | Pardot | Deep Salesforce integration |
> | IT | HubSpot | Lower support burden |
> | Finance | ActiveCampaign | Lowest cost |
>
> **Conflict:** Sales prefers Pardot for Salesforce integration. Recommendation: HubSpot Salesforce sync is robust enough for our needs; demo the integration specifically to Sales leadership.
>
> ---
>
> ## Sensitivity Analysis
>
> **If Integration weight increased to 30% (from 20%):**
> - Pardot moves to #2 (score: 3.6)
> - Recommendation unchanged
>
> **If Cost weight increased to 25% (from 15%):**
> - ActiveCampaign moves to #1 (score: 3.9)
> - Consider ActiveCampaign if budget is primary constraint
>
> **If Functionality weight increased to 40% (from 30%):**
> - Marketo moves to #2 (score: 3.6)
> - Consider Marketo if advanced features are critical
>
> **Conclusion:** HubSpot recommendation is robust under most reasonable weighting scenarios.
>
> ---
>
> ## Recommendation
>
> **Primary Recommendation: HubSpot Marketing Hub (Professional)**
>
> **Rationale:**
> 1. Highest overall score (4.2) with balanced performance across criteria
> 2. Best fit for team skill level and capacity
> 3. Reasonable TCO with predictable pricing
> 4. Strong vendor stability and product roadmap
> 5. Fastest implementation timeline (8-10 weeks)
>
> **Second Choice: ActiveCampaign**
> - Choose if: Budget is paramount and Salesforce integration requirements can be relaxed
> - TCO savings of ~$55K over 3 years
>
> **When to choose Marketo:** If we had a larger, more technical team and needed enterprise-grade ABM capabilities
>
> **When to choose Pardot:** If Sales leadership determines that native Salesforce integration is non-negotiable
>
> ---
>
> ## Next Steps
>
> 1. Present recommendation to steering committee (Week of [Date])
> 2. If approved, begin contract negotiation with HubSpot
> 3. Conduct reference calls with HubSpot customers of similar size
> 4. Finalize implementation timeline and resource plan
> 5. Develop change management and training plan

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Scores too close | Criteria not differentiating | Ask: "What criteria would actually differentiate these options?" |
| Stakeholder disagreement | Different priorities | Ask: "Let's run scenarios with different weightings to see impact" |
| Missing information | Incomplete research | Ask: "What questions do we need answered to score [criterion]?" |
| Analysis paralysis | Too many criteria | Ask: "Which criteria actually matter for the decision? Consolidate or eliminate others" |
| Biased toward incumbent | Familiarity bias | Ask: "Score the incumbent as if it were a new option we'd never used" |
| Cost dominates decision | Imbalanced weighting | Ask: "What's the cost of choosing wrong? Does that justify premium?" |

---

## Tips from Experience

1. **Get weight agreement BEFORE scoring.** Once people see scores, they'll want to change weights to get their preferred outcome.

2. **Distinguish must-haves from nice-to-haves.** Must-haves are pass/fail. Nice-to-haves are scored.

3. **Document evidence for scores.** "We scored them a 4 because..." prevents debates later.

4. **Run sensitivity analysis.** Know where your decision is robust vs. fragile.

5. **Include total cost of ownership.** License cost is rarely the whole story.

6. **Get sign-off on the process.** When stakeholders agree to the methodology upfront, they're more likely to accept the outcome.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Evaluation framework is accepted by stakeholders
- [ ] Scores are defensible with evidence
- [ ] Recommendation is clear and justified
- [ ] Stakeholders can explain why option was chosen
- [ ] Decision documentation is complete
- [ ] Post-implementation validates the decision

**Track over time:**
- Stakeholder satisfaction with process
- Time to decision vs. previous evaluations
- Post-selection vendor performance
- Whether predicted risks materialized
- Lessons for future evaluations

---

## Variations

### Technology Architecture Evaluation
For platform or architecture decisions:
```
Evaluate technology architecture options.

Options: [Architecture approaches]
Context: [What system is being built]

Criteria to evaluate:
- Scalability
- Maintainability
- Cost
- Team capability fit
- Time to implement
- Risk profile

Output: Architecture decision record (ADR)
```

### Service Provider RFP Evaluation
For professional services:
```
Evaluate service provider proposals.

RFP responses: [Paste proposals or summaries]
Project: [What we're hiring for]

Criteria:
- Relevant experience
- Proposed approach
- Team qualifications
- Cost/value
- Cultural fit
- References

Output: Scored evaluation with interview recommendations
```

### Build vs. Buy Analysis
For make/buy decisions:
```
Evaluate build vs. buy for [solution].

Build option: [Estimated effort, resources, timeline]
Buy options: [Vendor products to consider]

Compare on:
- Time to solution
- Total cost (including maintenance)
- Customization fit
- Strategic implications
- Risk profile

Output: Recommendation with decision factors
```

### Consolidation/Rationalization
For reducing vendor/tool sprawl:
```
Evaluate tools for consolidation.

Current tools: [List with purposes and costs]
Consolidation candidates: [Which could replace multiple]

Analyze:
- Coverage gaps if consolidated
- Cost savings potential
- Migration complexity
- User impact
- Risk of consolidation

Output: Rationalization roadmap
```

---

## Building Your Repeatable System

After several evaluations, build your system:

1. **Create evaluation template library** by category
2. **Document standard criteria and weights** by purchase type
3. **Maintain vendor intelligence** from past evaluations
4. **Track decision outcomes** for learning
5. **Refine methodology** based on results

**Sample Setup:**
```
vendor-evaluation/
├── templates/
│   ├── software-evaluation.md
│   ├── service-provider-evaluation.md
│   ├── hardware-evaluation.md
│   └── build-vs-buy-analysis.md
├── criteria-libraries/
│   ├── software-criteria.md
│   ├── security-criteria.md
│   └── vendor-stability-criteria.md
├── evaluations/
│   ├── 2024/
│   │   ├── marketing-automation/
│   │   │   ├── requirements.md
│   │   │   ├── vendor-info/
│   │   │   ├── evaluation-matrix.xlsx
│   │   │   ├── recommendation.md
│   │   │   └── decision-record.md
│   │   └── [other evaluations]/
└── reference/
    ├── past-decisions.md
    └── lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define criteria → gather information → score consistently → analyze and recommend**—applies broadly:

| Role | Application |
|------|-------------|
| **Procurement** | All vendor selection |
| **IT** | Technology decisions |
| **HR** | Benefits vendor selection |
| **Operations** | Equipment and service selection |
| **Project Managers** | Solution selection |
| **Product** | Build vs. buy decisions |

---

## Next Steps

1. **Define requirements:** What do you need?
2. **Identify options:** What are the candidates?
3. **Agree on criteria:** What matters and how much?
4. **Gather information:** Get what you need to score
5. **Generate evaluation:** Use this recipe
6. **Validate with stakeholders:** Confirm scores and weighting
7. **Make and document decision:** Capture rationale

---

*Recipe #44 of 100 in the Claude Code Knowledge Worker Recipe Collection*
