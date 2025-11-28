# Customer/Account Analysis Deep Dives

**Recipe #24: From Data Points to Account Intelligence**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 3-5 hours per analysis | Intermediate | Sales, Customer Success, Account Managers, Executives |

---

## The Problem

You're preparing for a QBR, executive briefing, or strategic account review and your customer data is scattered across CRM, support tickets, usage analytics, email threads, and meeting notes. Creating a comprehensive account picture takes hours of data gathering and synthesis. By the time you've assembled everything, you barely have time to actually strategize about the account.

**Pain Points:**
- Customer data scattered across multiple systems
- Time-consuming to compile account reviews
- Missing the strategic picture amid the details
- Risk signals hidden in data noise
- Opportunity identification is reactive
- QBR prep takes a full day or more

---

## The Outcome

Comprehensive account intelligence that surfaces health indicators, identifies risks and opportunities, and provides actionable strategy recommendations. Transform data gathering into strategic account management with clear next steps for every customer conversation.

**What You'll Have When Done:**
- Account health assessment
- Risk identification with severity
- Opportunity analysis
- Relationship mapping
- Strategic recommendations
- QBR-ready materials

---

## When to Use This Recipe

**Good Fit:**
- Quarterly Business Review preparation
- Account planning and strategy
- Executive briefing preparation
- Renewal and expansion planning
- At-risk account intervention
- New account manager onboarding

**Not a Good Fit:**
- Quick tactical questions (overkill)
- Accounts with minimal data
- Real-time support situations
- Transactional customer relationships

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have access to account data (CRM, usage, support, etc.)
- [ ] You've exported or gathered relevant data points
- [ ] You know the purpose of this analysis
- [ ] You have 1-2 hours for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Synthesizes data from multiple sources
- Identifies patterns and trends
- Surfaces risks and opportunities
- Creates comprehensive account profiles
- Generates strategic recommendations
- Produces presentation-ready materials

**Where Human Judgment Is Essential:**
- Understanding relationship nuances
- Political and organizational dynamics at customer
- Trust level and relationship history
- What's actually actionable in your context
- Validating data accuracy
- Final strategic decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| CRM data | Account details, contacts, activities | Baseline profile |
| Usage data | Product usage metrics, trends | Engagement health |
| Support tickets | Open/closed issues, satisfaction | Service health |
| Financial data | Revenue, growth, payment history | Commercial health |
| Communications | Email threads, meeting notes | Relationship context |
| External data | Company news, earnings, changes | Strategic context |

**Sample Input:**
```
Account Analysis: Meridian Health Systems

ACCOUNT BASICS (from CRM):
- Company: Meridian Health Systems
- Industry: Healthcare (hospital network)
- Employees: 12,000
- Contract: $180K ARR, renewed 8 months ago (2-year term)
- Products: Enterprise Platform, Analytics Module, Mobile Add-on
- Account Manager: Sarah Chen
- Executive Sponsor: David Park (VP of IT)

KEY CONTACTS:
- David Park (VP IT) - Executive sponsor, strong relationship
- Maria Santos (Director, Clinical Systems) - Day-to-day champion, engaged
- Robert Kim (CFO) - Limited engagement, questioned value last QBR
- Jennifer Wu (CIO) - New hire (3 months), haven't met yet

USAGE DATA (Last 90 days):
- Daily active users: 342 (down from 410 last quarter)
- Feature adoption: Core features 85%, Analytics 45%, Mobile 28%
- Login frequency: Down 15% vs. prior quarter
- API calls: Stable
- Admin logins: Decreased significantly

SUPPORT DATA (Last 90 days):
- Tickets opened: 23 (up from 12 prior quarter)
- Average resolution: 4.2 days (vs. 2.1 SLA target)
- CSAT score: 3.2/5 (down from 4.1)
- Open escalations: 2 (both >30 days old)

FINANCIAL:
- ARR: $180K
- Expansion opportunity: $60K (additional modules)
- Payment history: Always on time
- Last expansion: 18 months ago

RECENT COMMUNICATIONS:
- QBR 6 months ago: Positive, discussed expansion, CFO raised ROI questions
- Email from Maria (2 weeks ago): Asked about integration roadmap, mentioned "evaluating options"
- Support escalation (3 weeks ago): Critical feature request, no resolution yet

EXTERNAL CONTEXT:
- Meridian announced merger with Valley Health (3 months ago)
- Healthcare IT spending under pressure industry-wide
- David Park (our sponsor) may be affected by merger restructuring
```

---

## Step-by-Step Implementation

### Step 1: Gather Account Data
**Time: 15-20 minutes**

Export and organize data from:
- CRM (contacts, activities, history)
- Product usage/analytics
- Support system
- Finance/billing
- Meeting notes and communications
- External news/developments

Organize in a structured format for analysis.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Account Analysis Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Customer Account Analysis**

```
Please conduct a comprehensive analysis of this customer account.

ACCOUNT DATA:
"""
[PASTE ALL ACCOUNT DATA - CRM, usage, support, communications, etc.]
"""

ANALYSIS CONTEXT:
- My role: [Account Manager/CSM/Sales/etc.]
- Purpose: [QBR prep / Strategic review / Risk assessment / etc.]
- Upcoming event: [QBR date, renewal date, exec meeting, etc.]
- Key questions: [What specifically you need to know]

PLEASE PROVIDE:

1. ACCOUNT EXECUTIVE SUMMARY
   - One-paragraph account overview
   - Current health assessment (healthy/at-risk/critical)
   - Key relationship status
   - Single most important action needed

2. HEALTH SCORE ANALYSIS
   | Dimension | Score (1-10) | Trend | Key Indicators |

   Assess:
   - Engagement health (usage, adoption)
   - Relationship health (contacts, sentiment)
   - Service health (support satisfaction)
   - Commercial health (revenue, growth)
   - Strategic health (alignment, sponsorship)

   Overall health score with rationale

3. RISK ASSESSMENT
   | Risk | Severity | Likelihood | Evidence | Mitigation |

   Identify all risks with:
   - What could go wrong
   - How severe would it be
   - What's the evidence
   - How to mitigate

4. OPPORTUNITY ANALYSIS
   | Opportunity | Size | Timing | Next Step |

   Identify:
   - Expansion opportunities
   - Deepening engagement
   - New use cases
   - New stakeholders

5. RELATIONSHIP MAP
   - Key stakeholders with assessment
   - Relationship gaps
   - Champion health
   - Executive alignment
   - Power dynamics

6. TREND ANALYSIS
   - Usage trends (with interpretation)
   - Support trends (with interpretation)
   - Engagement trends
   - What trends suggest

7. STRATEGIC CONTEXT
   - External factors affecting customer
   - Industry/competitive pressures
   - Internal changes at customer
   - How this affects our position

8. RECOMMENDED ACTIONS
   Prioritized list:
   | Priority | Action | Owner | Timing | Expected Outcome |

   For each critical action:
   - Why this matters
   - How to execute
   - Success criteria

9. QBR/MEETING PREPARATION
   - Key messages to deliver
   - Questions to ask
   - Topics to avoid
   - Desired outcomes
   - Potential difficult questions and responses

10. 12-MONTH OUTLOOK
    - Best case scenario
    - Base case scenario
    - Worst case scenario
    - Key milestones and decision points
```

---

### Step 4: Review and Validate
**Time: 15-20 minutes**

Check the analysis:

**Validate health assessment:**
- Does the health score match your intuition?
- Are risks appropriately weighted?
- Any risks or opportunities missed?

**Check relationships:**
- Is the relationship map accurate?
- Any contacts missing?
- Power dynamics correct?

**Review recommendations:**
- Are actions realistic?
- Priorities correct?
- Timeline appropriate?

---

### Step 5: Enrich with Qualitative Context
**Time: 10-15 minutes**

Add what the data doesn't show:

```
Add this qualitative context to the analysis:

Recent conversations:
- [Summary of recent informal conversations]
- [Sentiment and concerns expressed]

Political dynamics:
- [What you know about internal politics]
- [Who's gaining/losing influence]

Relationship history:
- [How we've worked together over time]
- [Past issues and how they were resolved]

Gut feeling:
- [Your intuition about this account]

Revise the risk assessment and recommendations with this context.
```

---

### Step 6: Create Deliverables
**Time: 10 minutes**

```
Create these outputs:

1. ACCOUNT ONE-PAGER
   - Executive summary format
   - Health dashboard
   - Key risks and opportunities
   - Recommended actions

2. QBR PRESENTATION (10-12 slides)
   - Account performance review
   - Value delivered
   - Opportunities ahead
   - Strategic roadmap
   - Discussion topics

3. INTERNAL BRIEFING
   - Full analysis for internal team
   - Risk mitigation plan
   - Expansion strategy
   - Escalation items if any

4. MEETING PREP DOCUMENT
   - Agenda
   - Key messages
   - Questions to ask
   - Objection handling
   - Desired outcomes
```

---

## Example Output

Below is an abbreviated account analysis example:

---

> **ACCOUNT ANALYSIS: Meridian Health Systems**
> **Analysis Date: October 2024 | QBR Prep**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> Meridian Health Systems is showing early warning signs that require immediate attention. While the account has a strong foundation (solid ARR, engaged champion), multiple risk indicators have emerged: declining usage (-15%), deteriorating support satisfaction (CSAT dropped to 3.2), and the pending merger creates organizational uncertainty. Our executive sponsor may be affected by restructuring, and we haven't connected with the new CIO.
>
> **Health Assessment: ⚠️ AT-RISK (Score: 5.8/10)**
>
> **Most Important Action:** Secure executive-level meeting with new CIO before the merger restructuring solidifies. Our position is vulnerable without senior sponsorship.
>
> ---
>
> **HEALTH SCORE ANALYSIS**
>
> | Dimension | Score | Trend | Key Indicators |
> |-----------|-------|-------|----------------|
> | Engagement | 5/10 | ⬇️ Declining | DAU down 15%, Mobile adoption 28%, Admin logins dropped |
> | Relationship | 6/10 | ⬇️ At risk | Sponsor uncertain, CIO unknown, CFO skeptical |
> | Service | 4/10 | ⬇️ Declining | CSAT 3.2, 2 open escalations >30 days, resolution times 2x target |
> | Commercial | 7/10 | ➡️ Stable | Payments current, but no expansion in 18 months |
> | Strategic | 5/10 | ⬇️ Declining | Merger uncertainty, "evaluating options" mentioned |
>
> **Overall: 5.8/10 (AT-RISK)**
>
> Rationale: Multiple dimensions trending negatively simultaneously. The combination of declining engagement, poor service experience, and organizational uncertainty creates significant churn risk at renewal.
>
> ---
>
> **RISK ASSESSMENT**
>
> | Risk | Severity | Likelihood | Evidence | Mitigation |
> |------|----------|------------|----------|------------|
> | Churn at renewal | 🔴 High | Medium | Usage down, CSAT down, "evaluating options" | Immediate exec engagement, service recovery |
> | Sponsor loss | 🔴 High | Medium | Merger restructuring, David Park may be affected | Diversify relationships, engage Jennifer Wu |
> | Competitive displacement | 🟡 Medium | Medium | "Evaluating options" mention, merger as evaluation trigger | Demonstrate value, accelerate roadmap items |
> | Downsell pressure | 🟡 Medium | High | CFO skepticism, low feature adoption, cost pressure | Build ROI case, improve adoption |
> | Service relationship damage | 🟡 Medium | High | 2 long-standing escalations, CSAT declining | Resolve escalations immediately, exec attention |
>
> **Critical Risk:** The merger creates a natural evaluation point. Combined with service issues and declining engagement, this is a high-risk situation.
>
> ---
>
> **RELATIONSHIP MAP**
>
> | Contact | Role | Relationship | Influence | Status |
> |---------|------|--------------|-----------|--------|
> | David Park | VP IT | Strong | ⬇️ Uncertain post-merger | ⚠️ At risk |
> | Maria Santos | Director | Strong | Stable | ✅ Engaged champion |
> | Robert Kim | CFO | Weak | High | 🔴 Skeptical |
> | Jennifer Wu | CIO | None | Very High | ❓ Unknown |
>
> **Relationship Gaps:**
> 1. **No relationship with new CIO** — This is critical. Jennifer Wu likely has authority over IT direction post-merger.
> 2. **CFO skepticism unaddressed** — ROI questions from last QBR never fully resolved.
> 3. **Over-reliance on single sponsor** — David Park is our only executive relationship.
>
> ---
>
> **OPPORTUNITY ANALYSIS**
>
> | Opportunity | Size | Timing | Probability | Next Step |
> |-------------|------|--------|-------------|-----------|
> | Merger expansion | $100K+ | 6-12 months | Medium | Position for Valley Health rollout |
> | Analytics upsell | $60K | 3-6 months | Low now | Must fix service issues first |
> | Mobile deployment | $25K | Q1 | Medium | Low adoption—need success story |
> | Additional users | $40K | Post-merger | Medium | Depends on organizational clarity |
>
> **Key Insight:** Expansion opportunities exist but cannot be pursued until we stabilize the relationship. Focus on retention first.
>
> ---
>
> **RECOMMENDED ACTIONS**
>
> | Priority | Action | Owner | Timing | Expected Outcome |
> |----------|--------|-------|--------|------------------|
> | 🔴 P1 | Resolve open escalations | Support Lead | This week | CSAT recovery, service credibility |
> | 🔴 P1 | Request introduction to Jennifer Wu | Sarah Chen | Before QBR | Executive relationship, merger insight |
> | 🔴 P1 | Develop ROI analysis for CFO | Sarah + CSM | Before QBR | Address value skepticism |
> | 🟡 P2 | Engagement recovery plan | CSM | Next 30 days | Reverse usage decline |
> | 🟡 P2 | Integration roadmap response | Product | 2 weeks | Address Maria's question |
> | 🟢 P3 | Merger expansion positioning | Sales | 90 days | Seed future opportunity |
>
> **Action Detail: Resolve Open Escalations**
>
> Why: Two escalations open >30 days signals service failure. CSAT at 3.2 means the relationship is damaged.
>
> How:
> 1. Escalate internally to VP of Support
> 2. Provide direct update to Maria with timeline
> 3. Offer exec-to-exec apology if needed
> 4. Follow up with service recovery gesture
>
> Success criteria: Both escalations resolved with customer confirmation, follow-up CSAT survey showing improvement.
>
> ---
>
> **QBR PREPARATION**
>
> **Key Messages:**
> 1. Acknowledge service issues proactively—don't wait for them to raise it
> 2. Present concrete remediation plan
> 3. Show value delivered (quantify if possible)
> 4. Express commitment to partnership through merger transition
>
> **Questions to Ask:**
> 1. "How is the merger affecting your IT organization and priorities?"
> 2. "What does Jennifer Wu (new CIO) see as priorities?"
> 3. "What would success look like for you in the next 12 months?"
> 4. "What features from our roadmap matter most post-merger?"
>
> **Topics to Approach Carefully:**
> - Don't push expansion until service issues addressed
> - Don't assume David Park's future role
> - Don't ignore CFO's concerns
>
> **Desired Outcomes:**
> 1. Introduction to Jennifer Wu
> 2. Commitment to continue partnership
> 3. Clarity on merger impact and timeline
> 4. Agreement on 90-day priorities

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Health score doesn't match intuition | Missing qualitative data | Add: "Here's what the data doesn't show: [context]" |
| Recommendations too generic | Not enough account specifics | Add: "Given our history with this account: [details]" |
| Missing key risks | Data gaps | Ask: "What risks might exist that this data wouldn't show?" |
| Relationships incomplete | CRM data outdated | Add: "Here are contacts I know but aren't in the system: [list]" |
| Actions not actionable | Too high-level | Ask: "For the top 3 actions, provide specific execution steps" |
| External context missing | No external research | Ask: "Search for recent news about [company] and factor into analysis" |

---

## Tips from Experience

1. **Trust patterns over points.** Single data points can mislead. Look for patterns across multiple indicators.

2. **The relationship map is crucial.** Understanding who has power and influence is often more important than usage data.

3. **Decode "evaluating options."** When customers mention evaluating or exploring, they're already in a competitive process. Treat it as urgent.

4. **Service issues trump everything.** You cannot expand or deepen engagement while the customer is frustrated with support.

5. **New executives reset everything.** A new CIO or VP means your existing relationships and agreements may not matter. Act fast.

6. **Prepare for the conversation, not the presentation.** QBRs are dialogues, not monologues. The best prep enables great conversations.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Account health is clearly understood
- [ ] Risks are identified and mitigated
- [ ] QBR/meeting achieves desired outcomes
- [ ] Relationships are strengthened
- [ ] Retention/expansion targets are met

**Track over time:**
- Account health score trends
- QBR satisfaction scores
- Retention rates for analyzed accounts
- Expansion rates post-analysis
- Time spent on account prep (should decrease)

---

## Variations

### Portfolio Risk Assessment
For reviewing multiple accounts:
```
Analyze these accounts to identify portfolio risks.

Account data for: [List of accounts with key metrics]

Identify:
1. Accounts at highest risk (ranked)
2. Common risk patterns across portfolio
3. Resource prioritization recommendations
4. Early warning indicators to monitor
5. Aggregate portfolio health trend
```

### Expansion Planning
For growth-focused account analysis:
```
Analyze this account for expansion opportunities.

Account data: [Paste]
Current products: [What they have]
Expansion targets: [What could be sold]

Identify:
1. Most viable expansion opportunities
2. Decision makers for expansion
3. Business case for customer
4. Timing and approach
5. Competitive threats to expansion
```

### Renewal Preparation
For renewal-focused analysis:
```
Prepare for this account's upcoming renewal.

Account data: [Paste]
Renewal date: [Date]
Renewal value: [Amount]
Known issues: [What's been problematic]

Provide:
1. Renewal risk assessment
2. Value documentation
3. Objection anticipation
4. Negotiation preparation
5. Walk-away scenarios
```

### New Account Manager Onboarding
For transitioning accounts:
```
Create an onboarding document for a new account manager.

Account data: [Paste]
Transition date: [Date]

Provide:
1. Account history and context
2. Key relationship map
3. Current status and health
4. Open issues and commitments
5. 90-day recommended focus
6. Pitfalls to avoid
```

---

## Building Your Repeatable System

After several account analyses, establish your system:

1. **Create data export templates** for consistent gathering
2. **Build analysis templates** for different account tiers
3. **Establish review cadence** (quarterly for strategic accounts)
4. **Maintain account insights library** for institutional memory
5. **Connect to CRM** so insights persist

**Sample Setup:**
```
account-intelligence/
├── templates/
│   ├── analysis-prompt.txt
│   ├── data-export-checklist.md
│   └── qbr-template.pptx
├── accounts/
│   ├── meridian-health/
│   │   ├── 2024-Q4-analysis.md
│   │   ├── qbr-presentation.pptx
│   │   └── action-plan.md
│   └── [other accounts]/
├── portfolio/
│   ├── risk-dashboard.md
│   └── expansion-pipeline.md
└── playbooks/
    ├── at-risk-playbook.md
    └── expansion-playbook.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**aggregate data → analyze health → identify risks and opportunities → develop strategy → prepare for engagement**—applies broadly:

| Role | Application |
|------|-------------|
| **Sales** | Account planning and pursuit strategy |
| **Customer Success** | Renewal and expansion planning |
| **Account Management** | QBR and strategic account management |
| **Executives** | Key account reviews |
| **Partners** | Partner health and planning |
| **Investors** | Portfolio company assessment |

---

## Next Steps

1. **Pick a strategic account:** Choose one that matters and needs attention
2. **Gather the data:** Export from all relevant systems
3. **Run the analysis:** Use this recipe for comprehensive review
4. **Take action:** Execute on the top priorities
5. **Track results:** Monitor health score changes over time

---

*Recipe #24 of 100 in the Claude Code Knowledge Worker Recipe Collection*
