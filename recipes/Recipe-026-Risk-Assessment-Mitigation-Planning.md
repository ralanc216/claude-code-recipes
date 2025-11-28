# Risk Assessment and Mitigation Planning

**Recipe #26: From Uncertainty to Managed Risk**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 3-6 hours per assessment | Intermediate | Project Managers, Risk Managers, Executives, Operations |

---

## The Problem

Every project, initiative, and business decision carries risk, but risk assessment often happens superficially or not at all. You know things could go wrong, but you haven't systematically identified what, how likely, or how severe. When stakeholders ask "what could derail this?" you give generic answers. When things do go wrong, it feels like it should have been anticipated.

**Pain Points:**
- Risk identification is inconsistent and incomplete
- Likelihood and impact assessments are gut-feel
- Mitigation plans are vague or missing
- Risk registers become checkbox exercises
- Risks aren't monitored after identification
- Post-mortems reveal "obvious" risks that weren't captured

---

## The Outcome

Comprehensive risk assessments with structured identification, objective likelihood/impact ratings, concrete mitigation strategies, and monitoring approaches. Risk management becomes a value-adding discipline rather than compliance theater. You can make informed decisions about what risks to accept, mitigate, or avoid.

**What You'll Have When Done:**
- Complete risk register with all identified risks
- Likelihood and impact ratings with rationale
- Prioritized risk heat map
- Mitigation strategies for top risks
- Contingency plans
- Monitoring and early warning indicators
- Risk communication materials

---

## When to Use This Recipe

**Good Fit:**
- Project kickoff risk assessment
- Major initiative planning
- Strategic decision support
- Regulatory and compliance risk review
- Annual risk assessment refresh
- Pre-mortem analysis

**Not a Good Fit:**
- Real-time incident response (too slow)
- Highly technical security risks (need specialists)
- Insurance actuarial analysis (specialized)
- When you've already committed with no flexibility

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You understand the project/initiative/decision being assessed
- [ ] You know the stakeholders and their risk tolerances
- [ ] You have context on similar past initiatives
- [ ] You have 2-3 hours for comprehensive assessment

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Systematic risk identification across categories
- Consistent rating frameworks
- Mitigation strategy generation
- Risk register creation
- Pattern recognition from described context
- Documentation production

**Where Human Judgment Is Essential:**
- Organizational and political risks
- Likelihood estimates for your specific context
- What's actually acceptable to stakeholders
- Resource availability for mitigation
- Knowing what risks you've seen before
- Final risk acceptance decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Project/Initiative description | What you're doing | Risk identification context |
| Stakeholders | Who's affected | Impact assessment |
| Timeline | Key dates and milestones | Timeline risks |
| Dependencies | What relies on what | Dependency risks |
| Past issues | Similar project problems | Pattern recognition |
| Constraints | Budget, resources, etc. | Constraint-related risks |

**Sample Input:**
```
Risk Assessment Request

PROJECT: Customer Data Platform Migration
Duration: 6 months (March - August)
Budget: $2.5M
Team: 12 people (8 internal, 4 contractors)

DESCRIPTION:
Migrating from legacy on-premise customer data platform to cloud-based CDP. Involves:
- Moving 50M customer records
- Integrating with 15 downstream systems
- Retraining 200+ users
- Maintaining operations during transition
- Meeting GDPR and CCPA compliance requirements

KEY MILESTONES:
- March: Planning and architecture
- April-May: Development and testing
- June: Pilot migration (10% of data)
- July: Full migration
- August: Cutover and stabilization

STAKEHOLDERS:
- Marketing (primary users, 150 people)
- Sales (secondary users, 40 people)
- IT Security (compliance oversight)
- Finance (customer billing integration)
- Executive sponsor: CMO

DEPENDENCIES:
- Cloud vendor (new relationship)
- Data quality from legacy system
- Marketing team availability for testing
- IT Security approval gates

KNOWN CONCERNS:
- Legacy system has undocumented data transformations
- Cloud vendor is relatively new/small
- CMO has competing priorities and may not be available
- Similar migration failed at competitor last year
- Team has limited cloud migration experience
```

---

## Step-by-Step Implementation

### Step 1: Define Scope and Context
**Time: 10 minutes**

Document:
- What is being assessed (project, initiative, decision)
- Who the stakeholders are
- Timeline and key milestones
- Known constraints and dependencies
- Historical context (similar past efforts)

Comprehensive context leads to better risk identification.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Risk Assessment Prompt
**Time: 7-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Risk Assessment and Mitigation Planning**

```
Please conduct a comprehensive risk assessment for this initiative.

INITIATIVE OVERVIEW:
- Name: [Project/Initiative name]
- Description: [What you're doing]
- Duration: [Timeline]
- Budget: [If relevant]
- Team: [Size and composition]

DETAILED CONTEXT:
"""
[PASTE YOUR PROJECT DETAILS, MILESTONES, DEPENDENCIES, ETC.]
"""

STAKEHOLDERS:
- [Stakeholder 1]: [Their interest/role]
- [Stakeholder 2]: [Their interest/role]

KNOWN CONCERNS:
- [Concern 1]
- [Concern 2]

RISK TOLERANCE CONTEXT:
- Schedule flexibility: [Rigid/Some/Flexible]
- Budget flexibility: [Rigid/Some/Flexible]
- Scope flexibility: [Rigid/Some/Flexible]
- Quality tolerance: [Must be perfect/Good enough is OK]

PLEASE PROVIDE:

1. RISK IDENTIFICATION
   Systematically identify risks across categories:
   - Technical risks
   - Resource/People risks
   - Schedule risks
   - Budget/Financial risks
   - Dependency/Vendor risks
   - Organizational/Political risks
   - Compliance/Legal risks
   - External/Market risks

   For each risk:
   - Risk ID and name
   - Category
   - Description (what could happen)
   - Root cause (why it might happen)
   - Impact (what would be affected)

2. RISK REGISTER
   | ID | Risk | Category | Likelihood (1-5) | Impact (1-5) | Risk Score | Priority |

   Rating definitions:
   - Likelihood: 1=Rare, 2=Unlikely, 3=Possible, 4=Likely, 5=Almost certain
   - Impact: 1=Negligible, 2=Minor, 3=Moderate, 4=Major, 5=Severe

3. RISK HEAT MAP
   Create a visual representation:
   ```
   Impact ↑
   5 | [  ] [  ] [  ] [  ] [  ]
   4 | [  ] [  ] [  ] [  ] [  ]
   3 | [  ] [  ] [  ] [  ] [  ]
   2 | [  ] [  ] [  ] [  ] [  ]
   1 | [  ] [  ] [  ] [  ] [  ]
       1    2    3    4    5  → Likelihood
   ```
   Place risk IDs in appropriate cells

4. TOP RISKS DEEP DIVE
   For the top 5-7 highest-priority risks:
   - Detailed analysis
   - Early warning signs
   - Trigger events
   - Consequences if materialized
   - Mitigation strategy options
   - Recommended mitigation approach
   - Residual risk after mitigation
   - Contingency plan if risk materializes

5. MITIGATION PLAN
   | Risk | Mitigation Action | Owner | Timing | Cost | Effectiveness |

6. CONTINGENCY PLANS
   For high-impact risks:
   - Trigger for activating contingency
   - Contingency actions
   - Resources required
   - Decision authority

7. RISK MONITORING
   - Key risk indicators (KRIs) to track
   - Monitoring frequency
   - Escalation criteria
   - Review schedule

8. RISK INTERDEPENDENCIES
   - Which risks are connected
   - Cascading risk scenarios
   - Combined probability considerations

9. EXECUTIVE SUMMARY
   - Overall risk profile (Low/Medium/High/Critical)
   - Top 3 risks requiring attention
   - Recommended immediate actions
   - Go/No-Go recommendation with conditions

10. COMMUNICATION APPROACH
    - What to communicate to stakeholders
    - How to frame risks appropriately
    - Escalation path
```

---

### Step 4: Review and Validate
**Time: 20-30 minutes**

Evaluate the assessment:

**Check completeness:**
- Any obvious risks missing?
- Categories adequately covered?
- Your known concerns addressed?

**Validate ratings:**
- Do likelihood ratings match your experience?
- Are impact assessments realistic?
- Any under/over-rated risks?

**Test mitigations:**
- Are mitigation strategies feasible?
- Do you have resources to implement?
- Will they actually reduce risk?

---

### Step 5: Refine and Customize
**Time: 15-20 minutes**

**To add missing risks:**
```
Add these additional risks to the assessment:
1. [Risk you identified]
2. [Risk from past experience]

Rate them consistently with the existing framework.
```

**To adjust ratings:**
```
Risk #3 (vendor dependency) is higher likelihood in our context because [reason]. Adjust to likelihood 4 and update the analysis accordingly.
```

**To strengthen mitigation:**
```
The mitigation for data quality risk is too passive. Suggest more aggressive mitigation options that reduce the risk earlier in the project.
```

**To add pre-mortem perspective:**
```
Imagine the project failed. What's the most likely failure story? Work backward to identify risks and early warnings we might have missed.
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create these final outputs:

1. RISK REGISTER (formal document)
   - Complete risk listing
   - Ratings and justifications
   - Mitigation assignments

2. EXECUTIVE RISK SUMMARY (1 page)
   - Overall assessment
   - Top risks
   - Key mitigations
   - Recommendations

3. RISK DASHBOARD
   - Visual heat map
   - Key metrics
   - Status indicators

4. MONITORING CHECKLIST
   - What to track
   - When to review
   - Escalation triggers

5. STAKEHOLDER COMMUNICATION
   - Risk summary by audience
   - Talking points for concerns
```

---

## Example Output

Below is an abbreviated risk assessment example:

---

> **RISK ASSESSMENT: Customer Data Platform Migration**
> **Assessment Date: February 2024**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> **Overall Risk Profile: 🟡 MEDIUM-HIGH**
>
> This migration carries significant risk due to data complexity, vendor dependency, and organizational readiness factors. With proper mitigation, the project is achievable, but several high-priority risks require immediate attention and active management.
>
> **Top 3 Risks Requiring Attention:**
> 1. **Data quality and transformation issues** (Score: 20) — Legacy system undocumented transformations create significant data integrity risk
> 2. **Vendor stability** (Score: 16) — New, smaller vendor creates dependency risk
> 3. **Executive sponsor availability** (Score: 15) — Competing priorities may leave project without air cover
>
> **Recommendation:** Proceed with project, but implement all high-priority mitigations before beginning development phase. Establish weekly risk reviews and executive escalation path.
>
> ---
>
> **RISK REGISTER**
>
> | ID | Risk | Category | L | I | Score | Priority |
> |----|------|----------|---|---|-------|----------|
> | R1 | Data quality issues discovered during migration | Technical | 5 | 4 | 20 | 🔴 Critical |
> | R2 | Vendor stability/capability issues | Vendor | 4 | 4 | 16 | 🔴 Critical |
> | R3 | Executive sponsor unavailable for decisions | Organizational | 5 | 3 | 15 | 🟠 High |
> | R4 | Cloud migration skills gap | Resource | 4 | 3 | 12 | 🟠 High |
> | R5 | Downstream system integration failures | Technical | 3 | 4 | 12 | 🟠 High |
> | R6 | User adoption resistance | Organizational | 4 | 3 | 12 | 🟠 High |
> | R7 | Compliance/GDPR issues discovered | Compliance | 3 | 4 | 12 | 🟠 High |
> | R8 | Schedule overrun | Schedule | 4 | 3 | 12 | 🟠 High |
> | R9 | Budget overrun | Financial | 3 | 3 | 9 | 🟡 Medium |
> | R10 | Contractor turnover | Resource | 3 | 2 | 6 | 🟡 Medium |
>
> ---
>
> **RISK HEAT MAP**
>
> ```
> Impact ↑
>    5 |      |      |      |      |      |
>    4 |      |      | R5,R7|  R2  |  R1  |
>    3 |      |      |  R9  |R4,R6 |  R3  |
>      |      |      |      | R8   |      |
>    2 |      |      | R10  |      |      |
>    1 |      |      |      |      |      |
>        1      2      3      4      5   → Likelihood
> ```
>
> ---
>
> **TOP RISK DEEP DIVE**
>
> **R1: Data Quality Issues (Score: 20)**
>
> **Description:** Legacy system contains undocumented data transformations, business rules embedded in code, and potentially inconsistent data. Discovery of these issues during migration could cause significant rework, data integrity problems, and downstream failures.
>
> **Root Cause:** Technical debt in legacy system; original developers no longer with company; documentation not maintained.
>
> **Early Warning Signs:**
> - High volume of data validation errors in pilot
> - Downstream systems producing unexpected results
> - Users reporting data discrepancies
> - Extended time required for data mapping
>
> **Consequences if Materialized:**
> - Schedule delay (2-4 months)
> - Budget overrun ($300-500K)
> - Loss of stakeholder confidence
> - Potential data integrity issues affecting business decisions
> - Possible compliance violations
>
> **Mitigation Options:**
>
> | Option | Cost | Effectiveness | Recommendation |
> |--------|------|---------------|----------------|
> | A: Extended discovery phase | $150K | High | ✅ Recommend |
> | B: Data profiling tools | $50K | Medium | ✅ Recommend |
> | C: Legacy developer consulting | $80K | Medium | Consider |
> | D: Accept and address in testing | $0 | Low | Not recommended |
>
> **Recommended Mitigation:**
> - Extend discovery phase by 3 weeks ($150K)
> - Deploy data profiling tools immediately
> - Interview remaining long-tenure staff about undocumented rules
> - Create data quality dashboard before migration begins
>
> **Residual Risk After Mitigation:** Likelihood 3, Impact 3, Score 9 (reduced from 20)
>
> **Contingency Plan:**
> - Trigger: >10% data validation failures in pilot
> - Action: Halt migration, conduct deep-dive analysis, revise data mapping
> - Resources: Additional 2 data engineers, extended timeline
> - Decision: Project steering committee authorization required
>
> ---
>
> **R2: Vendor Stability Issues (Score: 16)**
>
> **Description:** Cloud CDP vendor is relatively new (3 years) and smaller (200 employees). Risk of vendor financial issues, capability gaps, or support failures during critical phases.
>
> **Early Warning Signs:**
> - Delayed responses to support tickets
> - Key vendor contacts leaving
> - Missing feature commitments
> - Negative industry press
>
> **Mitigation Strategy:**
> - Conduct vendor financial due diligence before contract finalization
> - Negotiate source code escrow agreement
> - Establish SLAs with penalties for support response
> - Identify backup vendor option
> - Require dedicated support contact
>
> **Contingency Plan:**
> - Trigger: Vendor misses 3+ SLA commitments OR significant negative news
> - Action: Activate backup vendor evaluation, escalate to vendor executive
> - Exit Strategy: Data portability plan, transition timeline
>
> ---
>
> **MITIGATION PLAN SUMMARY**
>
> | Risk | Mitigation Action | Owner | Timing | Status |
> |------|------------------|-------|--------|--------|
> | R1 | Extended discovery phase | PM | Before Phase 2 | Not started |
> | R1 | Data profiling deployment | Tech Lead | Week 1 | Not started |
> | R2 | Vendor due diligence | PM | Week 2 | Not started |
> | R2 | Escrow agreement | Legal | Week 3 | Not started |
> | R3 | Backup exec sponsor identified | PMO | Week 1 | Not started |
> | R4 | Cloud training for team | Tech Lead | Weeks 1-4 | Not started |
> | R5 | Integration testing plan | Tech Lead | Week 3 | Not started |
> | R6 | Change management plan | CMO | Week 2 | Not started |
>
> ---
>
> **RISK MONITORING**
>
> | Key Risk Indicator | Frequency | Green | Yellow | Red |
> |--------------------|-----------|-------|--------|-----|
> | Data validation error rate | Daily during migration | <2% | 2-5% | >5% |
> | Vendor support response time | Weekly | <4 hrs | 4-8 hrs | >8 hrs |
> | Schedule variance | Weekly | On track | <1 week slip | >1 week slip |
> | User training completion | Weekly | >90% | 70-90% | <70% |
> | Integration test pass rate | Per sprint | >95% | 85-95% | <85% |
>
> **Review Schedule:**
> - Weekly: Project team risk review
> - Bi-weekly: Steering committee risk update
> - Monthly: Executive sponsor risk briefing

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Risks too generic | Not enough project context | Add: "Here are specifics about our situation: [details]" |
| Missing obvious risks | Category not explored | Ask: "What [political/technical/etc.] risks might we be missing?" |
| All risks seem high priority | Rating calibration issue | Ask: "Apply stricter criteria—what are truly the top 5?" |
| Mitigations too expensive | Over-engineering solutions | Ask: "What's the minimum viable mitigation for each risk?" |
| Stakeholders dismissive | Poor communication | Ask: "How do I present these risks to skeptical stakeholders?" |
| Risk register becomes stale | No maintenance plan | Build in: "Create quarterly refresh protocol" |

---

## Tips from Experience

1. **The biggest risks are often not on the list.** Organizational and political risks are frequently underweighted because they're uncomfortable to document.

2. **Pre-mortems work better than risk lists.** Ask "imagine we failed—why?" to surface risks that structured identification misses.

3. **Likelihood × Impact is a start, not an answer.** Use the formula to prioritize, but don't ignore high-impact, low-likelihood risks that could be catastrophic.

4. **Mitigation has a cost.** Risk reduction isn't free. Make sure mitigation cost is proportionate to risk reduction.

5. **Monitor leading indicators, not lagging.** By the time the risk materializes, it's too late. Find early warning signs.

6. **Risk registers that aren't updated are worse than useless.** They create false confidence. Either maintain them or don't create them.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Risks are identified before they materialize
- [ ] Stakeholders make informed decisions about risk acceptance
- [ ] Mitigation plans are actually implemented
- [ ] Surprises decrease over time
- [ ] Post-mortems validate risk identification

**Track over time:**
- Percentage of identified risks that materialize
- Time from early warning to response
- Mitigation effectiveness
- Unidentified risks that occurred

---

## Variations

### Pre-Mortem Analysis
For imagining failure:
```
Conduct a pre-mortem for this initiative.

Initiative: [Description]

Imagine it's 12 months from now and the initiative has failed.

1. Write the failure story (what went wrong, how it unfolded)
2. Identify the root causes that led to failure
3. Work backward to early warning signs
4. Determine what we should do now to prevent this

Focus on realistic failure modes, not unlikely disasters.
```

### Strategic Risk Assessment
For organizational/business risks:
```
Assess strategic risks for [organization/business unit].

Context: [Business situation]

Identify risks across:
- Market and competitive risks
- Technology disruption risks
- Regulatory and compliance risks
- Talent and capability risks
- Financial and economic risks
- Reputation and brand risks

Provide 3-5 year risk horizon with recommended strategic responses.
```

### Decision Risk Analysis
For evaluating a specific decision:
```
Analyze risks of this decision:

Decision: [What you're deciding]
Options: [Option A, B, C]

For each option:
1. Risks introduced by choosing this option
2. Risks of NOT choosing this option
3. Risk comparison across options
4. Risk-adjusted recommendation
```

### Vendor/Partner Risk Assessment
For third-party risks:
```
Assess risks of engaging [Vendor/Partner].

Context: [What we'd use them for]
Information: [What we know about them]

Evaluate:
1. Financial stability risk
2. Operational capability risk
3. Dependency/concentration risk
4. Compliance and legal risk
5. Transition/exit risk
6. Reputation risk

Provide due diligence recommendations.
```

---

## Building Your Repeatable System

After several assessments, establish your system:

1. **Create risk category checklists** for thorough identification
2. **Build a risk library** of recurring risks in your domain
3. **Establish rating standards** for consistent assessment
4. **Maintain mitigation playbooks** for common risks
5. **Document lessons learned** from materialized risks

**Sample Setup:**
```
risk-management/
├── templates/
│   ├── risk-assessment-prompt.txt
│   ├── risk-register-template.xlsx
│   └── monitoring-dashboard.xlsx
├── assessments/
│   ├── cdp-migration/
│   │   ├── initial-assessment.md
│   │   ├── risk-register.xlsx
│   │   └── monitoring-log.md
│   └── archive/
├── reference/
│   ├── risk-category-checklists.md
│   ├── common-risks-library.md
│   └── mitigation-playbooks.md
└── lessons-learned/
    └── risk-retrospectives.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**systematic identification → structured rating → prioritization → mitigation planning → monitoring**—applies broadly:

| Role | Application |
|------|-------------|
| **Project Managers** | Project risk management |
| **Executives** | Strategic risk oversight |
| **Operations** | Operational risk management |
| **Finance** | Financial risk assessment |
| **IT/Security** | Technology risk management |
| **Compliance** | Regulatory risk assessment |

---

## Next Steps

1. **Pick a current project:** Apply this to something active
2. **Conduct the assessment:** Follow the full process
3. **Implement top mitigations:** Don't let it sit on paper
4. **Set up monitoring:** Track the key indicators
5. **Review and learn:** After the project, evaluate accuracy

---

*Recipe #26 of 100 in the Claude Code Knowledge Worker Recipe Collection*
