# Regulatory Change Impact Assessment

**Recipe #46: From New Regulations to Compliant Operations**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 10 minutes (repeat) | 6-12 hours per assessment | Advanced | Legal, Compliance, Operations, Regulated Industries |

---

## The Problem

Regulations change constantly—new laws, updated guidance, revised standards. For organizations in regulated industries, each change triggers a cascade of questions: Does this apply to us? What needs to change? How much will it cost? What's the deadline? Compliance teams drown in regulatory updates, struggling to assess which matter and what to do about them. The result is either over-reaction to everything or missed changes that lead to violations.

**Pain Points:**
- Volume of regulatory updates overwhelming
- Unclear which changes actually apply
- No systematic way to assess impact
- Multiple departments affected but siloed
- Timeline and resource estimation difficult
- Easy to miss compliance deadlines
- Hard to prioritize limited resources

---

## The Outcome

Structured impact assessments that clearly identify what changes, who's affected, and what actions are needed. A systematic approach to evaluating regulatory updates that prevents both over-reaction and dangerous omissions.

**What You'll Have When Done:**
- Applicability determination
- Gap analysis (current state vs. required)
- Impact assessment by function
- Required changes with timeline
- Resource and cost estimates
- Implementation roadmap
- Compliance tracking mechanism

---

## When to Use This Recipe

**Good Fit:**
- New legislation affecting your industry
- Regulatory guidance updates
- Standard revisions (ISO, SOC, etc.)
- Industry rule changes
- Privacy regulation updates (GDPR, CCPA)
- Financial regulation changes
- Healthcare compliance updates

**Not a Good Fit:**
- Minor clarifications with no material impact
- Regulations clearly not applicable to you
- Pending proposals (wait until final)
- Enforcement actions (need legal counsel)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the regulatory text or summary
- [ ] You understand current state of compliance
- [ ] You have access to relevant stakeholders
- [ ] Legal/compliance team is involved
- [ ] You have 4-6 hours for thorough assessment

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes regulatory text for key requirements
- Identifies applicability criteria
- Maps requirements to operational areas
- Structures gap analysis
- Generates action item frameworks
- Creates timeline templates

**Where Human Judgment Is Essential:**
- Legal interpretation
- Applicability determination
- Business impact assessment
- Resource allocation decisions
- Risk tolerance decisions
- Final compliance sign-off

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Regulatory text | New regulation or update | Requirements extraction |
| Guidance documents | Agency interpretations | Clarity on requirements |
| Current state | How you comply today | Gap identification |
| Organization context | Size, industry, operations | Applicability assessment |
| Timeline | Effective dates, deadlines | Implementation planning |

**Sample Input:**
```
Regulatory Impact Assessment Request

REGULATORY CHANGE:
New state privacy law: California Privacy Rights Act (CPRA) amendments
Effective date: January 1, 2025
Enforcement begins: July 1, 2025

REGULATORY TEXT SUMMARY:
[Paste the regulation text or detailed summary]

Key changes from current CCPA:
- New "sensitive personal information" category with opt-out rights
- Data minimization requirements
- Purpose limitation requirements
- Enhanced access/deletion rights
- New audit requirements for high-risk processing
- Increased penalties

OUR ORGANIZATION:
- Company: E-commerce retailer
- Size: 500 employees, $150M annual revenue
- California customers: ~2 million
- Data processed: Names, addresses, payment info, purchase history,
  browsing behavior, location data (sometimes)
- Current CCPA compliance: Yes, implemented 2020
- Current data practices documented: Yes, in privacy program docs

CURRENT STATE (Relevant to this regulation):
- Privacy policy: Updated for CCPA
- Consumer rights requests: Process in place (15 days)
- Data inventory: Exists but not comprehensive
- Consent management: Cookie banner, privacy preferences
- Vendor management: DPAs with major vendors
- Data security: SOC 2 certified
- Retention: No formal retention schedule
- Purpose tracking: Limited

KNOWN GAPS (preliminary):
- No sensitive data classification
- Data minimization not formally assessed
- No automated data retention
- Audit program not scoped for CPRA requirements

STAKEHOLDERS AFFECTED:
- Legal/Privacy
- IT/Engineering
- Marketing
- Customer Service
- HR (employee data)
- Procurement (vendor management)
```

---

## Step-by-Step Implementation

### Step 1: Gather Regulatory Materials
**Time: 20-30 minutes**

Collect:
- Full regulatory text
- Agency guidance or FAQ
- Industry interpretation (if available)
- Timeline and effective dates
- Your current compliance documentation

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Impact Assessment Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Regulatory Change Impact Assessment**

```
Please help me assess the impact of a regulatory change on our organization.

REGULATION INFORMATION:
- Name: [Regulation name]
- Effective Date: [When it takes effect]
- Enforcement Date: [When penalties begin]
- Jurisdiction: [Where it applies]

REGULATORY TEXT/SUMMARY:
"""
[Paste the regulatory text or detailed summary]
"""

OUR ORGANIZATION:
- Industry: [Your industry]
- Size: [Employees, revenue]
- Geographic presence: [Where you operate]
- Affected population: [Customers, employees, etc. under this regulation]

CURRENT COMPLIANCE STATE:
[Describe your current state relevant to this regulation]

PRELIMINARY GAPS IDENTIFIED:
[Any gaps you're already aware of]

PLEASE PROVIDE:

1. APPLICABILITY ASSESSMENT

   A. Does this regulation apply to us?
   - Threshold criteria (revenue, data volume, etc.)
   - Our status against each criterion
   - Determination: [Fully applies / Partially applies / Does not apply]

   B. What aspects apply?
   - Which requirements are relevant
   - Which have exemptions we qualify for
   - Which are unclear and need legal review

2. KEY REQUIREMENTS ANALYSIS

   For each major requirement:
   | Requirement | Description | Current State | Gap | Priority |

   Priority levels:
   - Critical: Must address immediately
   - High: Address within 90 days
   - Medium: Address by effective date
   - Low: Address within first year

3. IMPACT ASSESSMENT BY FUNCTION

   For each affected area:

   | Function | Impact Level | Key Changes Required | Resource Estimate |

   Functions to assess:
   - Legal/Compliance
   - IT/Technology
   - Operations
   - Marketing/Sales
   - HR
   - Finance
   - Customer Service
   - Vendor Management

4. GAP ANALYSIS

   Detailed gaps between current state and requirements:

   | # | Requirement | Current State | Gap | Remediation Approach |

5. RISK ASSESSMENT

   If we don't comply:
   - Regulatory penalties
   - Business consequences
   - Reputation risk
   - Competitive disadvantage

   If implementation is delayed:
   - Grace period risks
   - Enforcement likelihood
   - Mitigation options

6. IMPLEMENTATION ROADMAP

   Phase 1: Immediate (0-30 days)
   - Critical actions
   - Quick wins
   - Assessment completion

   Phase 2: Short-term (30-90 days)
   - High priority items
   - Process changes
   - Technology updates

   Phase 3: Pre-effective date
   - Remaining items
   - Testing and validation
   - Training

   Phase 4: Post-effective
   - Monitoring
   - Continuous compliance
   - Audit preparation

7. RESOURCE ESTIMATE

   | Category | Internal FTE | External Cost | Timeline |
   |----------|--------------|---------------|----------|
   | Legal/advisory | | | |
   | Technology | | | |
   | Process change | | | |
   | Training | | | |
   | Ongoing compliance | | | |
   | **Total** | | | |

8. DEPENDENCIES AND RISKS

   - What could delay implementation?
   - What decisions are blocking?
   - What external factors matter?

9. QUESTIONS REQUIRING LEGAL REVIEW

   Ambiguities or interpretive questions:
   - [Question 1]
   - [Question 2]

10. RECOMMENDED NEXT STEPS

    Immediate actions:
    1. [Action with owner]
    2. [Action with owner]
    3. [Action with owner]

NOTE: This assessment is for planning purposes. Legal/compliance review required for all interpretations and decisions.
```

---

### Step 4: Validate Applicability
**Time: 15-20 minutes**

Review the applicability assessment:
- Is our determination correct?
- Are there exemptions we missed?
- Do we need legal opinion on any criteria?

---

### Step 5: Deep Dive on Key Gaps
**Time: 20-30 minutes**

For significant gaps:

```
Let's analyze the gap in [specific requirement] more deeply:

Current state: [What we do today]
Requirement: [What the regulation requires]

Questions:
1. What specifically needs to change?
2. What are the options for addressing this?
3. What's the minimum viable compliance?
4. What's the gold standard approach?
5. What are the resource implications of each option?
```

---

### Step 6: Create Final Deliverables
**Time: 15 minutes**

```
Create the final impact assessment package:

1. EXECUTIVE SUMMARY (1-2 pages)
   For leadership:
   - What changed
   - Does it apply to us
   - Key impacts
   - Resource requirements
   - Recommended approach
   - Timeline

2. DETAILED IMPACT ASSESSMENT
   Complete analysis with all sections

3. IMPLEMENTATION PROJECT PLAN
   - Phases and milestones
   - Workstreams
   - Dependencies
   - Resource allocation

4. BOARD/COMMITTEE BRIEFING
   For governance reporting:
   - Regulatory change summary
   - Compliance posture
   - Risk assessment
   - Action plan

5. STAKEHOLDER COMMUNICATIONS
   Draft communications for:
   - Affected business units
   - IT and technology teams
   - Customer-facing teams

6. COMPLIANCE TRACKING TEMPLATE
   For ongoing monitoring:
   - Requirements checklist
   - Status tracking
   - Evidence documentation
```

---

## Example Output

Below is an abbreviated impact assessment example:

---

> **REGULATORY IMPACT ASSESSMENT**
>
> **California Privacy Rights Act (CPRA) Amendments**
>
> ---
>
> ## Executive Summary
>
> **Regulation:** California Privacy Rights Act (CPRA) 2025 amendments
> **Effective:** January 1, 2025 | **Enforcement:** July 1, 2025
>
> **Applicability:** ✅ **FULLY APPLIES** - We exceed all thresholds (2M California customers, $150M revenue, process significant personal information)
>
> **Overall Impact:** 🟡 **MEDIUM-HIGH**
>
> **Key Findings:**
> - 12 new or modified requirements identified
> - 6 gaps require remediation before effective date
> - Estimated implementation: $180K-$250K + 400-500 internal hours
> - Primary impacts: Data minimization, sensitive data handling, retention
>
> **Recommendation:** Initiate compliance project immediately. Engage external privacy counsel for interpretive questions. Budget approval needed by December 1.
>
> ---
>
> ## 1. Applicability Assessment
>
> ### Threshold Analysis
>
> | Criterion | Threshold | Our Status | Applies? |
> |-----------|-----------|------------|----------|
> | California consumer data | 100,000+ residents | 2,000,000 | ✅ Yes |
> | Revenue from CA data | 50%+ or $25M+ | ~35%, ~$15M | ⚠️ May not meet revenue alone |
> | Annual revenue | $25M+ gross | $150M | ✅ Yes |
> | Gross revenue trigger | Any business with PI | Yes | ✅ Yes |
>
> **Determination:** CPRA applies. We qualify as a "business" under multiple criteria.
>
> ### Exemptions Analysis
>
> | Exemption | Description | Do We Qualify? |
> |-----------|-------------|----------------|
> | Employee data | Limited exemption extended | ⚠️ Partial - reduced obligations |
> | B2B contact data | Limited exemption extended | ⚠️ Partial - reduced obligations |
> | Insurance data | CCPA insurance exemption | ❌ No - we're not insurance |
>
> **Exemption Status:** Limited exemptions for employee and B2B data; core consumer data protections fully apply.
>
> ---
>
> ## 2. Key Requirements Analysis
>
> | # | Requirement | Description | Current State | Gap | Priority |
> |---|-------------|-------------|---------------|-----|----------|
> | 1 | Sensitive personal information | Define, identify, provide opt-out | Not classified | 🔴 Major | Critical |
> | 2 | Data minimization | Collect only necessary data | Excess collection | 🔴 Major | High |
> | 3 | Purpose limitation | Use only for stated purposes | Informal tracking | 🟡 Moderate | High |
> | 4 | Retention limits | Delete when no longer needed | No formal policy | 🔴 Major | High |
> | 5 | Automated decision-making | Disclose, provide opt-out | Limited | 🟢 Minor | Medium |
> | 6 | Contractor requirements | Flow-down to service providers | Most DPAs current | 🟢 Minor | Medium |
> | 7 | Consumer right to correct | Process correction requests | Not implemented | 🟡 Moderate | High |
> | 8 | Consumer right to limit | Limit sensitive data use | Not implemented | 🟡 Moderate | High |
> | 9 | Risk assessments | Annual privacy risk assessments | Not conducted | 🟡 Moderate | Medium |
> | 10 | Cybersecurity audits | Annual security audits | SOC 2 exists | 🟢 Minor | Low |
> | 11 | Privacy notice updates | New disclosures required | Needs updates | 🟢 Minor | Medium |
> | 12 | Consumer preference signals | Honor Global Privacy Control | Not implemented | 🟡 Moderate | Medium |
>
> ---
>
> ## 3. Impact Assessment by Function
>
> | Function | Impact | Key Changes | Resource Est. |
> |----------|--------|-------------|---------------|
> | **Legal/Privacy** | High | Policy updates, contracts, interpretation | 150 hours + $40K external |
> | **IT/Engineering** | High | Data inventory, consent tooling, automation | 200 hours + $80K tools |
> | **Marketing** | Medium | Collection practices, purpose documentation | 40 hours |
> | **Customer Service** | Medium | New rights request handling | 30 hours + training |
> | **HR** | Low | Employee data compliance | 20 hours |
> | **Procurement** | Medium | Vendor assessments, DPA updates | 40 hours |
>
> ---
>
> ## 4. Gap Analysis
>
> ### Gap 1: Sensitive Personal Information Classification
>
> | Aspect | Detail |
> |--------|--------|
> | **Requirement** | Identify and classify sensitive PI; provide opt-out for use/disclosure |
> | **Current State** | No formal sensitive data classification; location data collected without special handling |
> | **Gap** | No inventory of sensitive data; no opt-out mechanism for sensitive data |
> | **Remediation** | 1) Complete data inventory with sensitive classification; 2) Implement sensitive data opt-out in preference center; 3) Update privacy notice |
> | **Estimated Effort** | 80 hours internal + $30K tooling |
>
> ### Gap 2: Data Minimization
>
> | Aspect | Detail |
> |--------|--------|
> | **Requirement** | Collect only personal information reasonably necessary for stated purpose |
> | **Current State** | Marketing collects extensive behavioral data; many fields "nice to have" |
> | **Gap** | No necessity assessment; likely over-collection |
> | **Remediation** | 1) Document purposes for each data element; 2) Conduct necessity review; 3) Reduce collection where not justified |
> | **Estimated Effort** | 60 hours internal |
>
> ### Gap 3: Retention Policy and Enforcement
>
> | Aspect | Detail |
> |--------|--------|
> | **Requirement** | Retain personal information only as long as reasonably necessary; inform consumers of retention |
> | **Current State** | No formal retention schedule; data retained indefinitely |
> | **Gap** | No retention periods defined; no automated deletion |
> | **Remediation** | 1) Define retention periods by data type; 2) Implement automated deletion; 3) Document in privacy notice |
> | **Estimated Effort** | 100 hours internal + $50K automation tooling |
>
> ### Gap 4: Right to Correction
>
> | Aspect | Detail |
> |--------|--------|
> | **Requirement** | Allow consumers to request correction of inaccurate personal information |
> | **Current State** | Not implemented |
> | **Gap** | No intake process; no workflow for corrections |
> | **Remediation** | 1) Add correction request to existing DSAR portal; 2) Create correction workflow; 3) Train customer service |
> | **Estimated Effort** | 30 hours internal |
>
> ---
>
> ## 5. Risk Assessment
>
> ### Non-Compliance Risk
>
> | Risk Type | Potential Impact |
> |-----------|-----------------|
> | **Regulatory penalties** | Up to $7,500 per intentional violation; $2,500 per unintentional violation |
> | **Private litigation** | $100-$750 per consumer per incident for data breaches |
> | **Enforcement actions** | California Privacy Protection Agency has direct enforcement authority |
> | **Business impact** | Potential loss of right to process CA data |
> | **Reputation** | Public enforcement actions; consumer trust erosion |
>
> ### Delay Risk Assessment
>
> | Scenario | Risk Level | Mitigation |
> |----------|------------|------------|
> | Full compliance by Jan 1 | 🟢 Low | Full protection |
> | Compliance by July 1 (enforcement) | 🟡 Medium | Document good faith efforts |
> | Compliance after July 1 | 🔴 High | Prioritize high-risk areas |
>
> ---
>
> ## 6. Implementation Roadmap
>
> ### Phase 1: Immediate (December 2024)
>
> | Action | Owner | Due |
> |--------|-------|-----|
> | Complete sensitive data inventory | Privacy Team | Dec 15 |
> | Legal review of ambiguous requirements | Outside Counsel | Dec 20 |
> | Budget approval for implementation | CFO | Dec 15 |
> | Project kickoff with stakeholders | Privacy Officer | Dec 10 |
>
> ### Phase 2: Short-term (January - February 2025)
>
> | Action | Owner | Due |
> |--------|-------|-----|
> | Implement sensitive data opt-out | IT | Jan 31 |
> | Complete data minimization review | Marketing/Privacy | Feb 15 |
> | Draft retention policy | Legal/Privacy | Jan 31 |
> | Add correction request capability | IT | Feb 28 |
> | Update privacy notice | Legal | Feb 28 |
>
> ### Phase 3: Pre-Enforcement (March - June 2025)
>
> | Action | Owner | Due |
> |--------|-------|-----|
> | Implement automated retention | IT | May 31 |
> | Complete vendor DPA updates | Procurement | Apr 30 |
> | Conduct privacy risk assessment | Privacy Team | May 31 |
> | Training rollout | HR/Privacy | Jun 15 |
> | Documentation and evidence collection | Compliance | Jun 30 |
>
> ### Phase 4: Post-Enforcement (July 2025+)
>
> | Action | Owner | Ongoing |
> |--------|-------|---------|
> | Monitor enforcement actions | Legal | Continuous |
> | Track consumer requests metrics | Privacy | Monthly |
> | Annual risk assessment | Privacy | Annually |
> | Audit readiness maintenance | Compliance | Continuous |
>
> ---
>
> ## 7. Resource Estimate
>
> | Category | Internal Hours | External Cost | Notes |
> |----------|---------------|---------------|-------|
> | Legal/Advisory | 50 | $40,000 | Interpretation, contracts |
> | Privacy Program | 100 | - | Policy, assessments |
> | Technology | 200 | $80,000 | Tooling, automation |
> | Operations | 40 | - | Process changes |
> | Training | 30 | $10,000 | Materials, delivery |
> | Ongoing (annual) | 100 | $30,000 | Monitoring, audit |
> | **Implementation Total** | **420** | **$130,000** | |
> | **First Year Total** | **520** | **$160,000** | |
>
> **Total Estimated Cost:** $180,000 - $250,000 (including contingency)
>
> ---
>
> ## 8. Questions for Legal Review
>
> 1. Does our current "location data" collection constitute "precise geolocation" under CPRA's sensitive data definition?
>
> 2. For data minimization, what standard applies—is "helpful for improving services" sufficient purpose, or must it be more specific?
>
> 3. Do our current SOC 2 audits satisfy the cybersecurity audit requirement, or is a separate privacy-focused audit needed?
>
> 4. What retention period is defensible for transaction history? Is there a safe harbor?
>
> ---
>
> ## 9. Recommended Next Steps
>
> **Immediate (This Week):**
>
> 1. **Schedule legal consultation** to resolve interpretive questions
>    - Owner: Privacy Officer
>
> 2. **Present to leadership** for budget approval
>    - Owner: Privacy Officer + CFO
>
> 3. **Initiate data inventory project** to classify sensitive data
>    - Owner: IT + Privacy
>
> **Next 30 Days:**
>
> 4. Launch cross-functional implementation team
> 5. Finalize project plan and resource allocation
> 6. Begin technology assessment for gaps
>
> ---
>
> **⚠️ DISCLAIMER**
>
> This assessment is for planning purposes only. It does not constitute legal advice. All regulatory interpretations and compliance decisions should be reviewed and approved by qualified legal counsel.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Unclear if regulation applies | Complex thresholds | Ask: "List every applicability criterion. Let's evaluate each separately" |
| Requirements too vague | Regulatory ambiguity | Ask: "What are the possible interpretations? What's the conservative approach?" |
| Impact underestimated | Not all functions considered | Ask: "Walk through every department. How does this touch their work?" |
| Timeline unrealistic | Scope not understood | Ask: "What are the dependencies? What's the critical path?" |
| Resources underestimated | Hidden complexity | Ask: "What are we not seeing? What similar projects have taught us?" |
| Stakeholders not aligned | Different interpretations | Ask: "Summarize in business terms. What decisions do stakeholders need to make?" |

---

## Tips from Experience

1. **Start with applicability.** Don't assume every regulation applies. Verify thresholds before deep analysis.

2. **Read the guidance.** Regulatory agencies often provide FAQ or implementation guides that clarify requirements.

3. **Engage legal early.** Complex interpretations need legal judgment, not AI analysis.

4. **Map to existing programs.** Often you're not starting from zero—existing compliance may cover parts of new requirements.

5. **Prioritize by risk.** Not all requirements carry equal penalty risk. Focus on high-consequence gaps.

6. **Build in buffer.** Regulatory timelines often slip, but so do implementation projects. Plan for both.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Applicability determination is validated
- [ ] All requirements are identified and assessed
- [ ] Gaps are quantified with remediation plans
- [ ] Resource estimates are approved
- [ ] Implementation is on track for deadlines
- [ ] No compliance surprises after effective date

**Track over time:**
- Regulatory change identification time
- Assessment completion time
- Implementation project success
- Compliance audit results
- Enforcement action avoidance

---

## Variations

### Multi-Regulation Comparison
For overlapping regulations:
```
Compare requirements across related regulations.

Regulations:
- [Regulation 1]
- [Regulation 2]
- [Regulation 3]

Create:
- Harmonized requirements matrix
- Where requirements conflict
- Single compliance approach where possible
- Gap analysis against current state
```

### Regulatory Monitoring Setup
For ongoing tracking:
```
Set up regulatory monitoring framework.

Industry: [Your industry]
Jurisdictions: [Where you operate]
Current regulations: [What you're already subject to]

Create:
- Sources to monitor
- Materiality criteria
- Assessment triggers
- Reporting cadence
- Escalation process
```

### Third-Party Impact Assessment
For vendor/customer implications:
```
Assess regulatory change impact on third parties.

Regulation: [Name]
Third parties: [Vendors, customers, partners]

Analyze:
- Contractual requirements
- Flow-down obligations
- Certification requirements
- Timeline for compliance demands
- Communication approach
```

### Board/Audit Committee Briefing
For governance reporting:
```
Create board briefing on regulatory change.

Regulation: [Name]
Full assessment: [Reference]

Create concise briefing:
- What changed and why it matters
- Our current compliance posture
- Risks if not addressed
- Resource request (if any)
- Timeline and milestones
- Management recommendation
```

---

## Building Your Repeatable System

After several assessments, build your system:

1. **Create assessment templates** by regulation type
2. **Maintain current state documentation** for faster gap analysis
3. **Build regulatory monitoring** for early awareness
4. **Track assessment history** for patterns
5. **Maintain stakeholder contacts** by compliance area

**Sample Setup:**
```
regulatory-compliance/
├── assessments/
│   ├── 2024/
│   │   ├── cpra-amendments/
│   │   │   ├── impact-assessment.md
│   │   │   ├── gap-analysis.xlsx
│   │   │   ├── implementation-plan.md
│   │   │   └── evidence/
│   │   └── [other assessments]/
├── current-state/
│   ├── data-inventory.xlsx
│   ├── privacy-program.md
│   ├── security-controls.md
│   └── vendor-compliance.xlsx
├── templates/
│   ├── impact-assessment.md
│   ├── gap-analysis.xlsx
│   └── board-briefing.md
├── monitoring/
│   ├── sources.md
│   ├── tracking.xlsx
│   └── alerts/
└── reference/
    ├── regulation-summaries/
    └── lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**determine applicability → analyze requirements → assess gaps → plan remediation**—applies broadly:

| Role | Application |
|------|-------------|
| **Legal/Compliance** | All regulatory changes |
| **Privacy** | Privacy law updates |
| **Security** | Security regulation and standards |
| **Finance** | Financial regulations |
| **Healthcare** | HIPAA, state health laws |
| **Operations** | Industry-specific regulations |

---

## Next Steps

1. **Get the regulation:** Obtain full text and guidance
2. **Assess applicability:** Determine if and how it applies
3. **Generate assessment:** Use this recipe for structured analysis
4. **Engage legal:** Validate interpretations
5. **Plan implementation:** Resource and timeline
6. **Execute and monitor:** Track to compliance

---

*Recipe #46 of 100 in the Claude Code Knowledge Worker Recipe Collection*
