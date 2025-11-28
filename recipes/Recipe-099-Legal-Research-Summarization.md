# Legal Research Summarization

**Recipe #99: From Legal Research to Actionable Guidance**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 3-6 hours per research project | Intermediate | Legal Professionals, Compliance Officers, Business Leaders |

---

## The Problem

Legal research generates extensive information from multiple sources—statutes, regulations, case law, legal opinions, and commentary. Synthesizing this into actionable guidance is time-consuming, and non-lawyers often struggle to understand the implications. Legal teams spend hours researching issues only to deliver memos that don't clearly answer the business question, or business teams make decisions without fully understanding legal implications.

**Pain Points:**
- Legal research scattered across statutes, cases, regulations, and secondary sources
- Non-lawyers struggle to understand dense legal language and implications
- Difficult to distill complex multi-jurisdictional analysis into clear recommendations
- Business teams need answers quickly but legal analysis takes time
- Uncertainty about how to apply legal precedents to specific business situations
- Risk of missing critical details when summarizing extensive research
- Challenge of keeping research current as laws and regulations change

---

## The Outcome

Clear, well-organized legal research summaries that present findings in accessible language, highlight key implications, identify risks, and provide actionable recommendations—enabling informed decision-making by legal and business stakeholders alike.

**What You'll Have When Done:**
- Organized summary of legal research by jurisdiction and issue
- Plain language explanation of legal requirements and restrictions
- Clear identification of risks and uncertainty areas
- Actionable recommendations with risk assessment
- Decision framework for business stakeholders
- Documentation suitable for both legal review and business use

---

## When to Use This Recipe

**Good Fit:**
- Contract interpretation questions requiring legal analysis
- Regulatory compliance research for business operations
- Employment law inquiries affecting HR policies
- Intellectual property questions for product development
- Privacy and data protection compliance analysis
- Corporate governance matters
- Litigation risk assessment before taking action
- Policy and procedure legal review

**Not a Good Fit:**
- Matters requiring formal legal opinions from outside counsel
- Active litigation requiring attorney-client privileged analysis
- Highly specialized areas requiring expert legal practitioners
- Emergency situations with insufficient time for thorough research

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Clear legal question or issue defined
- [ ] Relevant jurisdiction(s) identified
- [ ] Applicable time period known
- [ ] Business context documented
- [ ] Relevant contracts or documents available
- [ ] Prior legal opinions accessible (if any)
- [ ] Risk tolerance level understood
- [ ] Decision timeline known
- [ ] You have 1-2 hours for research organization and summarization

**Important Note:** This recipe helps organize and summarize legal research. It does not replace professional legal advice. All legal matters should be reviewed by qualified legal counsel.

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Organizes legal research findings by jurisdiction, statute, and issue
- Translates complex legal language into business-friendly explanations
- Identifies key precedents, authorities, and their implications
- Highlights risks, uncertainties, and areas requiring additional research
- Creates structured summaries for different audiences
- Formats findings into actionable decision frameworks

**Where Human Judgment Is Essential:**
- Determining applicability of precedents to specific facts
- Assessing materiality of legal risks in business context
- Making strategic recommendations balancing legal and business considerations
- Evaluating need for outside counsel or specialized expertise
- Determining appropriate level of risk for the organization
- Identifying when laws may be changing or subject to different interpretations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Research Question | Specific legal question with business context | Framing analysis and determining scope |
| Legal Findings | Statutes, cases, regulations, legal opinions | Understanding legal landscape and requirements |
| Jurisdictions | States, countries, regulatory bodies | Organizing multi-jurisdictional analysis |
| Business Context | Why this question matters, what's at stake | Tailoring recommendations to business needs |

---

## Step-by-Step Implementation

### Step 1: Frame the Legal Question
**Time: 10-15 minutes**

Clearly articulate the legal question, relevant jurisdictions, business context, and what decision depends on the answer.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Question Framing Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Frame Legal Research Question**

```
Claude, I need help organizing legal research.

Research question:
[PASTE THE LEGAL QUESTION OR ISSUE]

Business context:
[PASTE WHY THIS MATTERS, WHAT'S AT STAKE, WHAT DECISION NEEDS TO BE MADE]

Jurisdictions: [LIST RELEVANT STATES/COUNTRIES]
Timeline: [WHEN ANSWER IS NEEDED]

Help me:
1. Break down the question into specific legal issues to research
2. Identify relevant jurisdictions and applicable laws
3. Determine what precedents or authorities to look for
4. Note any threshold questions to resolve first
5. Identify what facts matter most for the legal analysis
```

---

### Step 4: Organize Research Findings
**Time: 7-10 minutes for Claude to process**

**PROMPT: Organize Legal Findings**

```
Organize these legal research findings:

Research findings: [PASTE STATUTES, CASES, REGULATIONS, LEGAL OPINIONS]
Jurisdictions covered: [LIST]

Create:
1. Summary organized by jurisdiction
2. Key authorities (statutes, cases, regulations) with citations
3. Current legal landscape and requirements
4. Recent trends or pending changes (if any)
5. Areas of uncertainty or conflicting authority
6. Comparison table if multiple jurisdictions
```

---

### Step 5: Analyze Implications
**Time: 7-10 minutes for Claude to process**

**PROMPT: Analyze Legal Implications**

```
Analyze the implications of this legal research:

Organized research findings: [PASTE FROM STEP 4]
Business context: [PASTE SPECIFIC SITUATION]
Proposed action: [WHAT THE BUSINESS WANTS TO DO]

Assess:
1. What is legally permissible vs. prohibited?
2. What are the risks of different approaches?
3. What factors affect enforceability or compliance?
4. How might the law change or be interpreted differently?
5. What practical constraints exist beyond pure legality?
```

---

### Step 6: Develop Recommendations
**Time: 7-10 minutes for Claude to process**

**PROMPT: Create Recommendations**

```
Develop recommendations based on this legal analysis:

Legal analysis: [PASTE FROM STEP 5]
Business objectives: [WHAT THEY WANT TO ACHIEVE]
Risk tolerance: [CONSERVATIVE / MODERATE / AGGRESSIVE]
Constraints: [TIME, BUDGET, OPERATIONAL LIMITATIONS]

Provide:
1. Recommended approach with legal basis
2. Alternative options with pros and cons
3. Risk mitigation strategies
4. Implementation considerations
5. Monitoring or review triggers
```

---

### Step 7: Create Summary Memorandum
**Time: 10-15 minutes for Claude to process**

**PROMPT: Generate Legal Memo**

```
Create a legal research summary memo:

All research and analysis: [PASTE FROM PREVIOUS STEPS]
Audience: [BUSINESS LEADERS / LEGAL TEAM / BOTH]
Format: [FORMAL LEGAL MEMO / BUSINESS SUMMARY / EXECUTIVE BRIEF]

Include:
1. Executive summary (one paragraph bottom line)
2. Question presented
3. Short answer
4. Analysis organized by issue or jurisdiction
5. Recommendations with rationale
6. Next steps or open questions
7. Authorities cited
```

---

### Step 8: Review and Validate
**Time: 15-30 minutes**

**Check immediately:**
- Analysis addresses the actual business question
- All relevant jurisdictions are covered
- Recommendations are practical and actionable
- Risks are clearly identified

**Spot-check specifics:**
- Citations are accurate and complete
- Statutes and cases are current
- Multi-jurisdictional comparisons are accurate
- Plain language summaries preserve legal accuracy

---

### Step 9: Prepare for Review
**Time: 5-10 minutes**

**PROMPT: Create Review Checklist**

```
Create a checklist for legal counsel review:

Research summary: [PASTE]
Research question: [ORIGINAL QUESTION]

Include:
- Key assumptions made
- Areas requiring validation
- Facts that might change the analysis
- Issues requiring specialized expertise
- Recommendations requiring approval
```

---

## Example Output

Below is an abbreviated example of what a well-executed legal research summary looks like:

---

> **LEGAL RESEARCH MEMORANDUM**
>
> | Field | Value |
> |-------|-------|
> | To | VP of Human Resources |
> | From | Legal Department |
> | Date | January 15, 2024 |
> | Re | Non-Compete Agreement Feasibility - Multi-State Analysis |
>
> ---
>
> ## Executive Summary
>
> Non-compete agreements are **not feasible** for California employees due to statutory prohibition, but **may be implemented** with careful drafting for Texas and New York employees. However, given pending federal regulation that may ban non-competes nationwide, we recommend focusing on **enhanced confidentiality agreements and non-solicitation provisions** rather than traditional non-competes.
>
> ---
>
> ## Questions Presented
>
> 1. Can the company require employees to sign non-compete agreements?
> 2. If so, what restrictions apply in California, Texas, and New York?
> 3. What alternatives exist to protect company interests?
>
> ## Short Answers
>
> 1. **Depends on jurisdiction.** Prohibited in California, enforceable with limitations in Texas and New York.
> 2. **California:** Void by statute. **Texas:** Must be ancillary, reasonable scope. **New York:** Must protect legitimate interests, reasonable terms.
> 3. **Yes.** Confidentiality agreements, non-solicitation, and trade secret protections available in all jurisdictions.
>
> ---
>
> ## Analysis
>
> ### I. California Law Prohibits Non-Compete Agreements
>
> **Governing Law:** California Business & Professions Code § 16600
>
> **Key Principle:** "Every contract by which anyone is restrained from engaging in a lawful profession, trade, or business of any kind is to that extent void."
>
> **Application:** This prohibition is interpreted broadly. Even if agreement specifies non-California law, California courts will apply California law to protect California residents.
>
> **Practical Implication:** Cannot use non-competes for California employees regardless of where agreement is signed.
>
> ---
>
> ### II. Texas Permits Non-Competes with Limitations
>
> **Governing Law:** Texas Business & Commerce Code § 15.50
>
> **Requirements:**
> - Must be ancillary to enforceable agreement
> - Reasonable time, geography, and scope
> - Cannot impose greater restraint than necessary
>
> **Consideration Issue:** Continued employment alone is insufficient consideration. Must provide something additional (confidential information, training).
>
> **Typical Enforceable Terms:** 1-2 years duration, territory where employee worked, same/similar business activities.
>
> ---
>
> ### III. Federal Regulation May Preempt State Law
>
> **Pending:** FTC Proposed Rule on Non-Compete Clauses (2023)
>
> **If enacted:** Would ban non-competes nationwide, preempting state law.
>
> **Status:** Final rule expected 2024, though subject to legal challenge.
>
> **Implication:** Even if implemented now, may become unenforceable in 2024-2025.
>
> ---
>
> ## Recommendations
>
> ### Primary Recommendation
>
> **Implement enhanced confidentiality and non-solicitation agreements** for all employees rather than non-competes.
>
> **Rationale:**
> - Consistent protection across jurisdictions
> - Avoids California issues
> - Reduces risk if federal ban enacted
> - More acceptable to employees
> - Protects key interests (confidential information, customer relationships)
>
> ### Specific Actions
>
> 1. **Update confidentiality agreements** - comprehensive definitions, post-employment obligations
> 2. **Add non-solicitation provisions** - customers (12-24 months), employees (12 months)
> 3. **Strengthen trade secret program** - identify, document, control access
> 4. **Consider role-specific protections** - executives may warrant additional provisions
>
> ---
>
> ## Next Steps
>
> 1. Decision on approach (non-competes TX/NY or confidentiality/non-solicitation)
> 2. Legal drafting of agreements
> 3. Review with HR and business stakeholders
> 4. Implementation rollout
> 5. Monitor FTC rulemaking
>
> ---
>
> ## Authorities Cited
>
> - California Business & Professions Code § 16600
> - *Edwards v. Arthur Andersen LLP* (2008) 44 Cal.4th 937
> - Texas Business & Commerce Code § 15.50
> - *Marsh USA Inc. v. Cook* (2011) 354 S.W.3d 764 (Tex.)
> - *BDO Seidman v. Hirshberg* (1999) 93 N.Y.2d 382
> - FTC Non-Compete Clause Proposed Rule, 88 Fed. Reg. 3482 (Jan. 19, 2023)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Research is inconclusive | Law is unclear or conflicting authority | Acknowledge uncertainty; present range; recommend conservative approach or further research |
| Business wants simple yes/no | Legal reality is nuanced | Provide clear recommendation in executive summary while preserving nuance in analysis |
| Law is changing rapidly | Pending legislation or evolving case law | Note changes prominently; build in review triggers; recommend monitoring |
| Multi-jurisdictional complexity | Different rules in different places | Organize by jurisdiction; provide comparison table; recommend practical approach across all |
| Too technical for audience | Legal jargon in summary | Use plain language; define terms; create separate technical appendix |
| Missing critical facts | Incomplete fact pattern | Identify assumptions; note how different facts change analysis; request clarification |

---

## Tips from Experience

1. **Frame the question precisely.** Vague questions get vague answers. "Can we do X?" is better than "Tell me about Y law."

2. **Include business context always.** Law is applied to facts. Understanding why this matters helps tailor analysis and recommendations.

3. **Identify jurisdiction clearly.** Location matters immensely. State the relevant jurisdictions explicitly and research all that apply.

4. **Distinguish legal from business advice.** Lawyers advise on law and risk, not pure business judgment. Make clear what's legal analysis vs. business recommendation.

5. **Acknowledge uncertainty honestly.** Legal analysis is rarely black and white. Be explicit about areas of uncertainty and how confident you are in conclusions.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Research clearly answers the business question posed
- [ ] Recommendations are practical and actionable
- [ ] Stakeholders understand the legal implications
- [ ] Decisions are made with appropriate understanding of risk
- [ ] No critical legal issues are overlooked

**Track over time:**
- Time from request to delivery of useful guidance
- Clarity ratings from business stakeholders
- Instances where legal issues were caught early
- Successful risk mitigation

---

## Variations

### Variation 1: Contract Interpretation Memo
Focus on specific contract language:
```
Analyze this contract provision:

Contract language: [PASTE SPECIFIC CLAUSE]
Dispute or question: [WHAT'S UNCLEAR]
Parties' positions: [DIFFERENT INTERPRETATIONS]

Include:
- Plain meaning analysis
- Industry standard interpretation
- Case law on similar provisions
- Practical implications of each interpretation
```

### Variation 2: Regulatory Compliance Summary
Focus on compliance requirements:
```
Summarize compliance requirements for [REGULATION]:

Regulation: [CITE REGULATION]
Our activities: [DESCRIBE WHAT WE DO]
Industry: [SECTOR]

Include:
- Applicable requirements
- Compliance gaps we have
- Implementation steps
- Ongoing obligations
- Penalties for non-compliance
```

### Variation 3: Litigation Risk Assessment
Assess risk before taking action:
```
Assess litigation risk of [PROPOSED ACTION]:

Proposed action: [DESCRIBE]
Potential claims: [WHAT COULD WE BE SUED FOR]
Jurisdiction: [WHERE THIS WOULD BE LITIGATED]

Include:
- Probability analysis
- Exposure assessment
- Strength of defenses
- Cost-benefit of alternatives
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create research templates.** Standard formats for different types of legal questions (employment, contracts, compliance, IP).

2. **Build a research library.** Archive completed memos by topic. Reuse and update rather than starting from scratch.

3. **Develop standard positions.** For recurring questions, document the company's standard legal position and rationale.

4. **Implement matter tracking.** Track legal research requests, status, and outcomes. Identify patterns requiring policy updates.

**Sample Folder Structure:**
```
legal-research/
├── templates/
│   ├── employment-law-memo.md
│   ├── contract-interpretation.md
│   └── compliance-summary.md
├── by-topic/
│   ├── employment/
│   ├── ip/
│   └── privacy/
└── standard-positions/
    └── non-competes-policy.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**translating complex technical analysis into actionable guidance**—applies broadly:

| Role | Application |
|------|-------------|
| **Tax Planning** | Translating tax code into business planning recommendations |
| **Technical Standards** | Interpreting engineering standards for product development |
| **Medical Research** | Summarizing clinical research for treatment decisions |
| **Financial Regulations** | Explaining securities regulations for business operations |
| **Scientific Analysis** | Translating research findings into policy recommendations |

---

## Next Steps

1. **This week:** Use this recipe for your next legal research project. Practice translating legal analysis into plain language.

2. **Track your results:** Measure time saved and stakeholder satisfaction with clarity of guidance.

3. **Iterate:** Customize memo formats for your organization and common question types.

4. **Maintain:** Keep research summaries updated as laws change. Review and refresh annually.

---

*Recipe #99 of 100 in the Claude Code Knowledge Worker Recipe Collection*
