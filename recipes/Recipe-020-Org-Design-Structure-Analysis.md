# Org Design and Structure Analysis

**Recipe #20: From Org Chart Chaos to Strategic Structure**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 10 minutes (repeat) | 4-8 hours per analysis | Intermediate | HR Leaders, Executives, Managers, Consultants |

---

## The Problem

Your organization has grown, merged, or evolved, and the current structure doesn't match how work actually gets done. Reporting lines are unclear, spans of control vary wildly, there are obvious gaps and overlaps, but you can't articulate why it feels broken. When someone asks "should we reorganize?" you can describe symptoms but can't do structured analysis. Org design becomes political rather than strategic.

**Pain Points:**
- Org structure evolved organically without intentional design
- Spans of control inconsistent (some managers with 2, others with 15)
- Unclear where certain functions should sit
- Duplication of roles across teams
- Gaps in coverage for critical capabilities
- No framework for evaluating structural options
- Reorganization discussions driven by politics, not strategy

---

## The Outcome

A structured analysis of your current organization with clear identification of issues, comparison of structural options, and recommendations for improvement. You can have evidence-based conversations about org design, evaluate trade-offs between structures, and make intentional choices about reporting relationships and team composition.

**What You'll Have When Done:**
- Current state org analysis with identified issues
- Span of control and layer analysis
- Role clarity and duplication assessment
- Alternative structure options with trade-offs
- Recommendations with rationale
- Transition considerations

---

## When to Use This Recipe

**Good Fit:**
- Post-merger integration planning
- Rapid growth requiring structural adaptation
- Performance issues potentially linked to structure
- New leader evaluating their organization
- Annual strategic planning
- Preparing for significant change (new product, market, etc.)

**Not a Good Fit:**
- Small teams (<10 people) where informal works
- Very recent restructure (give it time to work)
- When the real issue is people, not structure
- Avoiding difficult personnel decisions by reorganizing
- Routine headcount planning

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have current org chart or structure data
- [ ] You understand the organization's strategy and priorities
- [ ] You know current pain points and symptoms
- [ ] You have context on how work flows across the org
- [ ] You have 1-2 hours for analysis and exploration

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes span of control and organizational layers
- Identifies structural patterns and anomalies
- Generates alternative structure options
- Evaluates trade-offs between designs
- Creates comparison frameworks
- Produces documentation for stakeholder discussion

**Where Human Judgment Is Essential:**
- Understanding the real issues (not just symptoms)
- Political and cultural considerations
- People and talent implications
- Historical context (what's been tried before)
- Implementation feasibility
- Final design decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Current org chart | Reporting relationships | Structure analysis |
| Role descriptions | What each role does | Duplication/gap finding |
| Strategy context | Company priorities | Alignment assessment |
| Pain points | Where it's not working | Problem diagnosis |
| Headcount data | Team sizes | Span of control analysis |

**Sample Input:**
```
Organization: Product Development Division
Headcount: 85 people
Context: Grew from 30 to 85 in 18 months; never intentionally redesigned

Current Structure:
VP Product Development
├── Director of Engineering (12 direct reports)
│   ├── 8 Senior Engineers (individual contributors)
│   ├── 2 Engineering Managers
│   │   ├── EM1: 6 engineers
│   │   └── EM2: 4 engineers
│   └── 2 Tech Leads (hybrid IC/management)
├── Director of Product (3 direct reports)
│   ├── Senior PM (2 PMs report to them)
│   ├── PM
│   └── Product Analyst
├── Director of Design (8 direct reports)
│   ├── Design Manager (3 designers)
│   ├── 4 Senior Designers
│   └── UX Researcher
├── Director of QA (4 direct reports)
│   └── 4 QA Engineers
└── Program Manager (dotted line reports unclear)

Known Issues:
- Engineering Director overwhelmed (12 DRs, plus all escalations)
- Unclear if Tech Leads manage or contribute
- Design and Engineering don't collaborate well
- QA feels siloed (brought in too late)
- Product team seems understaffed for the workload
- Nobody owns platform/infrastructure specifically
- Program Manager role unclear—is it strategic or admin?

Strategic Context:
- Need to launch 2 new products next year
- Platform stability is becoming critical
- Want to improve speed of delivery
- May acquire a small company (10-15 engineers)
```

---

## Step-by-Step Implementation

### Step 1: Document Current State
**Time: 10-15 minutes**

Gather:
- Current org chart with reporting lines
- Headcount by team/function
- Known pain points and symptoms
- Strategic context (where the org is headed)
- Any constraints (budget, key people, etc.)

Be honest about what's not working—that's what we're solving.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Org Analysis Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Org Design Analysis**

```
Please analyze this organization structure and provide design recommendations.

CURRENT ORGANIZATION:
"""
[PASTE YOUR ORG STRUCTURE - text format of reporting relationships]
"""

CONTEXT:
- Organization: [Name/function]
- Total headcount: [Number]
- Growth history: [How it got to current state]
- Strategic priorities: [Where the org is headed]

KNOWN ISSUES/SYMPTOMS:
"""
[PASTE YOUR LIST OF PAIN POINTS]
"""

CONSTRAINTS:
- [Budget constraints]
- [Key people who must stay in role]
- [Timeline pressures]
- [Political considerations]

PLEASE PROVIDE:

1. CURRENT STATE ANALYSIS
   - Organizational metrics (spans of control, layers, ratios)
   - Structural strengths (what's working)
   - Structural issues (what's not working)
   - Root causes (why it's not working)

2. SPAN OF CONTROL ANALYSIS
   | Role | Direct Reports | Assessment |
   Flag anyone over 10 or under 3 direct reports

3. ORGANIZATIONAL LAYERS
   - Count layers from top to bottom
   - Identify where layers add value vs. add bureaucracy
   - Compare to benchmarks

4. ROLE CLARITY ASSESSMENT
   - Roles with unclear accountability
   - Potential duplications
   - Gaps in coverage
   - Hybrid roles that may cause confusion

5. STRUCTURAL OPTIONS
   Present 2-3 alternative structures:

   Option A: [Name/Theme]
   - Description
   - Org chart (text format)
   - Pros
   - Cons
   - Best for: [when to choose this]

   Option B: [Name/Theme]
   ...

   Option C: [Name/Theme]
   ...

6. COMPARISON MATRIX
   | Criteria | Current | Option A | Option B | Option C |
   Rate: speed, clarity, scalability, talent development, etc.

7. RECOMMENDATION
   - Which option (or hybrid) do you recommend?
   - Rationale
   - Key risks
   - Phasing (how to get there)

8. TRANSITION CONSIDERATIONS
   - Change management needs
   - Communication approach
   - Timeline recommendation
   - Success metrics for new structure
```

---

### Step 4: Review the Analysis
**Time: 15-20 minutes**

Evaluate Claude's analysis:

**Check the numbers:**
- Are span of control calculations correct?
- Layer count accurate?
- Any roles or people missed?

**Check the logic:**
- Do the identified issues match your experience?
- Are root causes plausible?
- Do the structural options make sense?

**Check the fit:**
- Would these options work in your culture?
- Are there political realities not captured?
- Is the recommendation implementable?

---

### Step 5: Explore Options
**Time: 15-20 minutes**

**To dive deeper on an option:**
```
Expand on Option B (the cross-functional pod model). Show me specifically how this would work for a feature team—who reports to whom, how decisions get made, and how this addresses the Engineering-Design collaboration issue.
```

**To address a specific issue:**
```
The Engineering Director's span of control is the most urgent issue. Show me 3 ways to address this specifically, with minimal disruption to the rest of the org.
```

**To model a hybrid:**
```
I like elements of Option A and Option C. Can you create a hybrid that has the functional leadership structure of A but the cross-functional execution model of C?
```

**To add constraints:**
```
We need to do this without adding headcount. How does that change the recommendations?
```

**To plan the transition:**
```
Assuming we go with Option B, create a detailed transition plan including:
- What changes in Phase 1 (first 30 days)
- What changes in Phase 2 (days 30-60)
- Communication plan
- Risk mitigation
```

---

### Step 6: Prepare Stakeholder Materials
**Time: 10 minutes**

```
Create two outputs:
1. Executive briefing (2 pages max) summarizing the analysis and recommendation for leadership approval
2. Manager talking points for explaining the rationale to their teams (if/when we proceed)
```

---

## Example Output

Below is an abbreviated org analysis example:

---

> **CURRENT STATE ANALYSIS: Product Development Division**
>
> ---
>
> **Organizational Metrics**
>
> | Metric | Current | Benchmark | Assessment |
> |--------|---------|-----------|------------|
> | Total headcount | 85 | - | - |
> | Organizational layers | 4 | 3-4 | ✅ Appropriate |
> | Average span of control | 5.2 | 5-8 | ✅ Healthy average |
> | Max span of control | 12 | 8-10 | 🔴 Dir of Eng overloaded |
> | Min span of control | 2 | 3+ | ⚠️ Some too narrow |
> | Engineer:PM ratio | 14:1 | 6-10:1 | 🔴 PMs understaffed |
> | Engineer:Designer ratio | 5.7:1 | 4-6:1 | ✅ Appropriate |
>
> ---
>
> **SPAN OF CONTROL ANALYSIS**
>
> | Role | Direct Reports | Assessment |
> |------|---------------|------------|
> | VP Product Development | 5 | ✅ Appropriate |
> | Director of Engineering | 12 | 🔴 Overloaded |
> | Director of Product | 3 | ⚠️ Could be broader |
> | Director of Design | 8 | ✅ Appropriate |
> | Director of QA | 4 | ⚠️ Narrow for a Director |
> | Engineering Managers | 4-6 | ✅ Appropriate |
> | Design Manager | 3 | ⚠️ Narrow |
>
> **Critical Issue:** Director of Engineering with 12 DRs (8 ICs + 2 EMs + 2 Tech Leads) is unsustainable. This creates bottleneck for decisions, insufficient coaching for team, and burnout risk.
>
> ---
>
> **ROOT CAUSE ANALYSIS**
>
> | Symptom | Root Cause |
> |---------|------------|
> | Engineering Director overwhelmed | Structure didn't scale with growth; no intermediate layer added |
> | Design-Engineering collaboration poor | Functional silos; no shared accountability for outcomes |
> | QA brought in too late | Separate reporting line; not embedded in delivery flow |
> | Product understaffed | Headcount grew in Engineering but PM ratio not maintained |
> | Platform ownership unclear | No dedicated platform team; everyone owns infrastructure |
> | Tech Lead role confusion | Hybrid IC/management role without clear definition |
>
> ---
>
> **STRUCTURAL OPTIONS**
>
> **Option A: Strengthen Functional Model**
>
> ```
> VP Product Development
> ├── Sr. Director of Engineering (NEW)
> │   ├── Engineering Manager - Frontend (4 eng)
> │   ├── Engineering Manager - Backend (4 eng)
> │   ├── Engineering Manager - Platform (4 eng) (NEW TEAM)
> │   └── Engineering Manager - Mobile (3 eng)
> ├── Director of Product (add 2 PMs)
> ├── Director of Design
> ├── Director of QA (embed QA in teams)
> └── Program Manager (reports to VP)
> ```
>
> **Pros:**
> - Clear career paths within functions
> - Deep functional expertise development
> - Easier to manage compensation and growth
>
> **Cons:**
> - Doesn't solve cross-functional collaboration
> - Hand-offs between functions remain
> - Platform team still separate from product teams
>
> **Best for:** Organizations that value functional excellence over delivery speed
>
> ---
>
> **Option B: Cross-Functional Pods**
>
> ```
> VP Product Development
> ├── Pod Lead - Core Product (PM background)
> │   ├── 3 Engineers, 1 Designer, 1 QA (embedded)
> ├── Pod Lead - Growth (PM background)
> │   ├── 3 Engineers, 1 Designer, 1 QA (embedded)
> ├── Pod Lead - Platform (Eng background)
> │   ├── 4 Engineers, 1 DevOps
> ├── [Additional pods...]
> ├── Director of Engineering (functional home, dotted line)
> ├── Director of Design (functional home, dotted line)
> └── Director of QA (functional home, dotted line)
> ```
>
> **Pros:**
> - Teams own outcomes end-to-end
> - Collaboration built into structure
> - Faster delivery, fewer hand-offs
>
> **Cons:**
> - Career path complexity (matrix)
> - Potential for inconsistent practices across pods
> - Functional directors become coaches, not direct managers
>
> **Best for:** Organizations prioritizing delivery speed and cross-functional collaboration
>
> ---
>
> **COMPARISON MATRIX**
>
> | Criteria | Current | Option A | Option B |
> |----------|---------|----------|----------|
> | Clarity of accountability | 🔴 | ✅ | ✅ |
> | Cross-functional collaboration | 🔴 | ⚠️ | ✅ |
> | Delivery speed | ⚠️ | ⚠️ | ✅ |
> | Functional expertise depth | ✅ | ✅ | ⚠️ |
> | Scalability | 🔴 | ✅ | ✅ |
> | Change management effort | - | Low | High |
>
> ---
>
> **RECOMMENDATION: Modified Option B**
>
> Implement cross-functional pods for product delivery, with functional leadership retained for career development, hiring, and practices.
>
> **Rationale:**
> 1. Directly addresses collaboration issues (primary pain point)
> 2. Solves Engineering Director overload (distributes leadership)
> 3. Embeds QA into flow (fixes "brought in too late" issue)
> 4. Creates clear platform ownership
> 5. Positions org well for new product launches
>
> **Key Risks:**
> - Change management complexity (people used to functional reporting)
> - Pod Lead role needs strong definition
> - Risk of functional skill atrophy
>
> **Mitigation:**
> - Retain functional "chapters" for skill development
> - Define clear Pod Lead selection criteria and training
> - Establish functional communities of practice

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Analysis too superficial | Not enough context provided | Add: "Here's more context about [specific area]" |
| Options all look the same | Constraints too tight | Relax constraints: "Show me a more radical option, even if it requires headcount" |
| Recommendations too generic | Generic input | Add specific pain points: "The specific issue is X and we need to solve that" |
| Doesn't fit culture | Cultural context missing | Add: "Our culture is [description]. Factor this into recommendations" |
| Political realities ignored | Wasn't mentioned | Add: "There are political considerations: [X and Y]. How does that change things?" |
| Transition plan unrealistic | Underestimated change effort | Ask: "Assume this will be harder than typical. What's a more conservative transition plan?" |

---

## Tips from Experience

1. **Structure follows strategy.** Before reorganizing, be clear on what you're optimizing for. Different strategies need different structures.

2. **Don't reorganize to avoid people decisions.** If the issue is an underperformer or bad manager, restructuring won't fix it.

3. **Spans of control aren't one-size-fits-all.** A manager of experienced ICs can handle 10; a manager of new hires might struggle with 5. Context matters.

4. **Every structure has trade-offs.** There's no perfect org chart. Pick the trade-offs you can live with.

5. **Changes take 6-12 months to show results.** Don't reorganize too frequently. Give structures time to work.

6. **Involve the people affected.** The best structures are designed with input from those who'll work within them.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Structural issues are clearly articulated with evidence
- [ ] Options have clear trade-offs, not just pros
- [ ] Recommendation has rationale leadership can evaluate
- [ ] Transition plan is realistic and actionable
- [ ] Stakeholders can have informed discussion about structure

**Track after restructure:**
- Delivery speed (lead time, cycle time)
- Employee satisfaction with clarity
- Manager span of control sustainability
- Cross-functional collaboration effectiveness
- Time to fill new roles (structure clarity helps recruiting)

---

## Variations

### Post-Merger Integration
For combining two organizations:
```
I need to integrate two organizations post-merger.

Org A (acquiring company):
[Structure and headcount]

Org B (acquired company):
[Structure and headcount]

Constraints:
- Key people to retain from both
- Synergies expected (headcount reduction target if any)
- Cultural differences

Create integration options that:
1. Combine effectively while retaining key talent
2. Clarify leadership structure
3. Minimize disruption to ongoing work
4. Address cultural integration
```

### New Function/Team Design
For designing a new team:
```
I need to design a new [function/team] from scratch.

Purpose: [What this team will do]
Scope: [What's in/out of scope]
Headcount budget: [How many people]
Interfaces: [What other teams it connects to]

Design options for:
1. Team structure and roles
2. Reporting line (where it should sit)
3. Interaction model with other teams
4. Growth path as team scales
```

### Flattening Analysis
For reducing layers:
```
We want to flatten our organization. Current structure:

[Paste current org]

Goals:
- Reduce from X to Y layers
- Increase spans of control to 7-10
- Maintain clear accountability

Analyze:
1. Which layers can be removed with least disruption?
2. Which roles become unnecessary?
3. What new capabilities do remaining managers need?
4. Transition approach
```

### Scaling Planning
For future growth:
```
We're planning to grow from [X] to [Y] people over [timeframe].

Current structure: [paste]

Plan:
1. At what points does current structure break?
2. What structural changes should we plan for at each milestone?
3. Which roles should we hire proactively vs. reactively?
4. How do we maintain culture and coordination as we scale?
```

---

## Building Your Repeatable System

After several org analyses, establish your system:

1. **Create a standard org data template** for consistent input
2. **Maintain org design principles** for your company
3. **Document structural decisions** with rationale for future reference
4. **Build a change management playbook** for restructures
5. **Track structural metrics** over time (spans, layers, ratios)

**Sample Setup:**
```
org-design/
├── templates/
│   ├── org-analysis-prompt.txt
│   └── org-data-template.md
├── analyses/
│   ├── 2024-product-dev/
│   │   ├── current-state.md
│   │   ├── options.md
│   │   └── decision.md
│   └── 2024-engineering/
├── principles/
│   └── org-design-principles.md
└── playbooks/
    └── restructure-change-mgmt.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**document current state → identify structural issues → generate options → evaluate trade-offs → recommend**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Company-wide structure decisions |
| **HR Leaders** | Organization design consulting |
| **Managers** | Team structure optimization |
| **Consultants** | Client org assessments |
| **M&A Teams** | Integration planning |
| **Operations** | Process and workflow structure |

---

## Next Steps

1. **Next org question:** Use this recipe to structure your analysis
2. **Document current state:** Even if not changing, document your org for future reference
3. **Define principles:** What org design principles should guide your decisions?
4. **Plan proactively:** Identify when your structure will need to change before it breaks

---

*Recipe #20 of 100 in the Claude Code Knowledge Worker Recipe Collection*
