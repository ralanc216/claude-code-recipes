# Contract Review and Risk Summarization

**Recipe #43: From Legal Documents to Actionable Insights**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 2-4 hours per contract | Intermediate | Legal, Procurement, Finance, Executives |

---

## The Problem

Contracts are critical business documents that nobody wants to read. They're long, dense, and written in legal language that obscures rather than clarifies. Business teams sign agreements without understanding key risks. Legal reviews take weeks while deals stall. When disputes arise, nobody knew about the problematic clause buried on page 47. The gap between what's signed and what's understood creates business risk.

**Pain Points:**
- Contracts too long and complex to read thoroughly
- Business teams don't understand legal language
- Legal review bottleneck delays deals
- Key risks hidden in dense language
- No standardized way to summarize terms
- Comparison to standard terms is manual and slow
- Due diligence overwhelmed with contract volume

---

## The Outcome

Clear, business-readable summaries of key contract terms with risks flagged and explained. Faster review cycles that don't sacrifice thoroughness. Executives and business teams who understand what they're signing.

**What You'll Have When Done:**
- Executive summary of key terms
- Risk assessment with severity ratings
- Comparison to standard terms
- Plain-language explanations
- Action items for negotiation
- Red flags clearly highlighted

---

## When to Use This Recipe

**Good Fit:**
- Vendor and supplier agreements
- Customer contracts before signing
- Partnership and collaboration agreements
- Lease and real estate contracts
- M&A due diligence contract review
- Insurance policy review
- Standard form contract analysis

**Not a Good Fit:**
- Replacing legal counsel (always have legal review)
- Highly regulated contracts (securities, healthcare)
- Litigation preparation (need specialized expertise)
- Contract drafting (different process)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the contract document (text extractable)
- [ ] You know your standard terms for comparison
- [ ] You understand the business context
- [ ] You have legal review planned (AI assists, not replaces)

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Extracts key terms from dense language
- Identifies unusual or risky clauses
- Creates structured summaries
- Compares against standard terms
- Translates legalese to plain language
- Highlights areas needing attention

**Where Human Judgment Is Essential:**
- Legal interpretation and advice
- Business impact assessment
- Risk tolerance decisions
- Negotiation strategy
- Final approval to sign
- Jurisdiction-specific analysis

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Contract text | The agreement to review | Core analysis |
| Standard terms | Your preferred terms | Comparison baseline |
| Deal context | What you're trying to achieve | Risk relevance |
| Priority areas | What matters most | Focus analysis |
| Past issues | Problems from similar contracts | Risk awareness |

**Sample Input:**
```
Contract Review Request

CONTRACT TYPE: Master Services Agreement (MSA)

CONTRACT PARTIES:
- Us: [Your Company Name] (Customer)
- Them: TechVendor Solutions, Inc. (Vendor)

DEAL CONTEXT:
- Engaging vendor for cloud data processing services
- 3-year term, ~$500K annual spend
- They'll have access to customer data (PII)
- Critical to our operations once implemented

PRIORITY REVIEW AREAS:
1. Data security and privacy obligations
2. Liability and indemnification
3. Term and termination rights
4. SLA and performance guarantees
5. IP ownership (of customizations)
6. Pricing and payment terms

OUR STANDARD POSITIONS:
- Unlimited liability for data breaches
- 30-day termination for convenience after Year 1
- 99.9% uptime SLA with service credits
- We own all customizations
- Annual price cap at 3% increase
- 60-day payment terms

KNOWN RED FLAGS (from past deals):
- Auto-renewal clauses
- Broad IP assignment clauses
- Limitation of liability caps that are too low
- Mandatory arbitration
- Unilateral amendment rights

CONTRACT TEXT:
[Paste full contract text here]
```

---

## Step-by-Step Implementation

### Step 1: Prepare the Contract
**Time: 5-10 minutes**

- Extract text from PDF or obtain clean document
- Note page numbers for reference
- Identify the contract type and parties
- Understand the business context

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Contract Review Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Contract Review and Risk Summarization**

```
Please help me review and summarize this contract.

CONTRACT INFORMATION:
- Type: [Contract type]
- Parties: [Who's involved]
- Value: [Financial terms if known]
- Context: [Why we're entering this agreement]

OUR STANDARD POSITIONS:
[List your preferred terms]

PRIORITY REVIEW AREAS:
[What matters most to you]

KNOWN CONCERNS:
[Any specific issues to watch for]

CONTRACT TEXT:
"""
[Paste the full contract text]
"""

PLEASE PROVIDE:

1. EXECUTIVE SUMMARY (1 page max)
   - Parties and effective date
   - What this agreement does
   - Key financial terms
   - Major obligations (ours and theirs)
   - Term and termination basics
   - Overall risk assessment (Low/Medium/High)

2. KEY TERMS EXTRACTION
   For each major area, extract and explain:

   | Area | Contract Says | Plain Language | Our Standard | Gap |

   Areas to cover:
   - Scope of services/deliverables
   - Pricing and payment
   - Term and renewal
   - Termination rights
   - Liability and indemnification
   - Intellectual property
   - Confidentiality
   - Data protection/privacy
   - Warranties
   - Insurance requirements
   - Dispute resolution
   - Assignment
   - Force majeure

3. RISK ASSESSMENT
   For each identified risk:

   | Risk | Severity | Contract Reference | Business Impact | Recommendation |

   Severity levels:
   - 🔴 High: Requires negotiation before signing
   - 🟡 Medium: Should try to negotiate, may accept
   - 🟢 Low: Note but likely acceptable

4. UNUSUAL OR NON-STANDARD CLAUSES
   - Clauses that deviate significantly from standard
   - Clauses that are unusually one-sided
   - Hidden obligations or landmines
   - Missing protections we should have

5. NEGOTIATION PRIORITIES
   Top 5-7 issues to negotiate, in priority order:
   - What to ask for
   - Why it matters
   - Fallback position
   - Walk-away point (if any)

6. QUESTIONS FOR THE OTHER PARTY
   Ambiguities or unclear terms that need clarification

7. COMPARISON TO STANDARD
   Summary of how this compares to our standard positions

8. RECOMMENDED ACTIONS
   - [ ] Must negotiate before signing
   - [ ] Should discuss with [stakeholder]
   - [ ] Acceptable to sign as-is
   - [ ] Other actions needed

IMPORTANT: This is for business review purposes. Final decisions require legal counsel.
```

---

### Step 4: Review the Analysis
**Time: 15-20 minutes**

Check the summary:
- Does the executive summary capture the essence?
- Are the key terms accurately extracted?
- Are the risks appropriately flagged?
- Is anything missing that matters?

---

### Step 5: Deep Dive on Concerns
**Time: 10-15 minutes**

For flagged risks or areas of concern:

```
Let's dive deeper into [specific clause/issue].

Questions:
1. What exactly does this clause obligate us to do?
2. What are the worst-case scenarios under this language?
3. How does this compare to market standard?
4. What alternative language would be more favorable?
5. If they won't change it, what's our exposure?
```

---

### Step 6: Prepare Negotiation Materials
**Time: 10 minutes**

```
Based on your analysis, create:

1. REDLINE SUMMARY
   For each issue to negotiate:
   - Current language (quote exactly)
   - Proposed language (our preferred revision)
   - Justification (why reasonable)

2. INTERNAL BRIEFING
   For our business team:
   - What this contract covers
   - Key risks in plain language
   - What we need to push back on
   - What we can accept

3. NEGOTIATION SCRIPT
   For the discussion with the other party:
   - Opening position
   - Key talking points
   - Potential compromises
```

---

## Example Output

Below is an abbreviated contract review example:

---

> **EXECUTIVE SUMMARY**
>
> ---
>
> **Parties:** [Your Company] (Customer) and TechVendor Solutions, Inc. (Vendor)
> **Contract Type:** Master Services Agreement
> **Effective Date:** Upon signature
> **Value:** ~$500,000/year; 3-year term = ~$1.5M total
>
> **What This Agreement Does:**
> TechVendor will provide cloud-based data processing services, including data storage, analytics, and reporting. They will have access to our customer data, including PII, and will process it according to our instructions.
>
> **Major Obligations:**
> - **Ours:** Pay invoices within 30 days; provide data in specified formats; designate admin contacts; comply with acceptable use policy
> - **Theirs:** Provide services per specifications; maintain 99.5% uptime; implement security measures; comply with data protection laws
>
> **Term:** 3 years, auto-renews for 1-year periods
>
> **Overall Risk Assessment:** 🟡 **MEDIUM**
>
> Several key terms require negotiation before signing, particularly around liability caps, data breach obligations, and termination rights. However, this is a workable contract with reasonable terms in most areas.
>
> ---
>
> **KEY TERMS EXTRACTION**
>
> | Area | Contract Says | Plain Language | Our Standard | Gap |
> |------|---------------|----------------|--------------|-----|
> | **Uptime SLA** | 99.5%, 5% service credits max | They guarantee 99.5% uptime; if they miss it, we get up to 5% off next month's bill | 99.9%, unlimited credits | 🟡 Lower SLA, capped credits |
> | **Termination for Convenience** | 90 days notice, only at renewal | We can't exit without cause until the 3-year term ends, except at renewal | 30 days after Year 1 | 🔴 Significant lock-in |
> | **Liability Cap** | Greater of 12 months fees or $500K | If they mess up, max we can recover is ~$500K | Unlimited for data breaches | 🔴 Major gap on data breach |
> | **Indemnification** | Mutual for IP infringement; Vendor for data breach (capped) | They'll cover us for IP lawsuits; data breach coverage is limited to the liability cap | Unlimited data breach indemnity | 🔴 Insufficient coverage |
> | **IP Ownership** | All customizations owned by Vendor | They own everything they build, even if we paid for it | We own customizations | 🟡 Should negotiate |
> | **Data Location** | US and "approved" locations | They can move our data, but "approved" isn't defined | US only, named facilities | 🟡 Need specificity |
> | **Price Increases** | Up to 7% annually with 60-day notice | They can raise prices significantly each year | 3% cap | 🟡 Higher than we like |
> | **Auto-Renewal** | 60-day written notice to prevent | We must remember to send notice or we're locked in another year | 90-day notice, email acceptable | 🟢 Slight gap, manageable |
> | **Payment Terms** | Net 30 | Standard | Net 60 | 🟢 We prefer longer, but acceptable |
>
> ---
>
> **RISK ASSESSMENT**
>
> | Risk | Severity | Contract Reference | Business Impact | Recommendation |
> |------|----------|-------------------|-----------------|----------------|
> | **Capped Liability for Data Breach** | 🔴 High | Section 9.2 | If they breach and expose customer PII, our potential liability to customers could far exceed $500K recovery from vendor | Must negotiate unlimited or significantly higher cap for data incidents |
> | **No Termination for Convenience** | 🔴 High | Section 12.1 | We're locked in for 3 years. If service is poor but not "material breach," we have no exit | Negotiate 30-day termination right after Year 1 |
> | **Vendor Owns Customizations** | 🟡 Medium | Section 7.3 | Work we pay for (custom reports, integrations) belongs to them; we can't take it if we leave | Negotiate ownership or perpetual license to customizations |
> | **Low SLA (99.5%)** | 🟡 Medium | Schedule B | 99.5% = up to 44 hours downtime/year. If this is mission-critical, that's significant | Push for 99.9%; increase service credits |
> | **Vague Data Location** | 🟡 Medium | Section 6.4 | "Approved locations" undefined; could include jurisdictions with different privacy laws | Require named data center locations or US-only commitment |
> | **Price Increase Cap (7%)** | 🟡 Medium | Section 4.3 | Over 3 years, 7% annual increases = potential 22.5% total increase | Negotiate down to 3-5% |
> | **Auto-Renewal Terms** | 🟢 Low | Section 12.4 | 60-day written notice is short; easy to miss and get locked in | Set internal reminder; possibly negotiate to 90 days |
>
> ---
>
> **UNUSUAL OR NON-STANDARD CLAUSES**
>
> 1. **Section 5.6 - Unilateral Policy Changes**
>    - Vendor can modify their security policies with 30-day notice
>    - We have no approval right; only remedy is termination
>    - This is unusual and concerning for critical services
>
> 2. **Section 14.2 - Audit Rights (Limited)**
>    - We can only audit once per year with 45-day notice
>    - Industry standard is more flexible audit rights
>    - Given the data sensitivity, we should push for better terms
>
> 3. **Section 8.4 - Marketing Rights**
>    - Hidden in "Miscellaneous": They can use our logo in marketing
>    - We didn't agree to this; should remove or require approval
>
> 4. **Missing: Data Breach Notification Timeline**
>    - No specific timeframe for breach notification
>    - Industry standard is 24-72 hours
>    - Must add specific notification requirements
>
> ---
>
> **NEGOTIATION PRIORITIES**
>
> | Priority | Issue | Ask | Why It Matters | Fallback | Walk-Away |
> |----------|-------|-----|----------------|----------|-----------|
> | 1 | Data Breach Liability | Unlimited or $5M minimum | Our regulatory exposure exceeds their cap | $2M cap for data incidents | Below $1M cap |
> | 2 | Termination Rights | 30-day termination after Year 1 | Need exit if service doesn't meet needs | 60-day, penalty fee | No termination right |
> | 3 | IP Ownership | We own customizations paid for | Protect our investment | Perpetual, transferable license | License that survives termination |
> | 4 | SLA | 99.9% with meaningful credits | Mission-critical system | 99.7%, 15% credit cap | Below 99.5% |
> | 5 | Data Location | US only, named facilities | Compliance and security | US and EU only, pre-approved | Undefined "approved" locations |
> | 6 | Breach Notification | 24-hour notification | Regulatory requirements | 48-hour notification | No specific timeline |
> | 7 | Price Cap | 3% annual | Budget predictability | 5% annual | Above 7% |
>
> ---
>
> **QUESTIONS FOR THE OTHER PARTY**
>
> 1. Section 6.4: What are the "approved" data processing locations? Please provide a complete list.
> 2. Section 5.6: Can we have approval rights over security policy changes that affect our data?
> 3. Section 9.2: Is there flexibility on the liability cap specifically for data security incidents?
> 4. Schedule B: What has been your actual uptime over the past 12 months?
> 5. Section 7.3: Will you agree to our ownership of custom development we fund?
>
> ---
>
> **RECOMMENDED ACTIONS**
>
> - [x] Review complete - issues identified
> - [ ] **Must negotiate** Sections 9.2 (liability), 12.1 (termination), 7.3 (IP ownership) before signing
> - [ ] **Should discuss** with Privacy/Security team re: Sections 6.4 and 5.6
> - [ ] **Should discuss** with Finance re: pricing terms and payment schedule
> - [ ] Prepare redlined version for negotiation call
> - [ ] Schedule legal review of final negotiated version before signature
>
> ---
>
> **⚠️ DISCLAIMER**
>
> This summary is for business review purposes only. It does not constitute legal advice. All contracts should be reviewed by qualified legal counsel before execution.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Missing key terms | Contract poorly organized | Ask: "Search for clauses related to [topic] throughout the document" |
| Risk assessment too conservative | Default caution | Ask: "Calibrate risks to [industry/deal size]. What's actually standard?" |
| Summary too long | Over-detailed | Ask: "Condense to what's genuinely important for a business decision" |
| Legal jargon not translated | Complex language | Ask: "Explain [clause] in plain language. What does this mean practically?" |
| Comparison baseline unclear | Standards not provided | Provide: "Our standard position is [X]. How does this compare?" |
| Missed hidden clauses | Buried in long document | Ask: "Check for any clauses in 'Miscellaneous' or 'General' that create obligations" |

---

## Tips from Experience

1. **AI assists, doesn't replace legal review.** Use this for efficiency, not to skip lawyers on important contracts.

2. **Context matters for risk assessment.** A $50K vendor contract has different risk tolerance than a $5M strategic partnership.

3. **Focus on what's non-standard.** If terms match market standard, spend less time there. Unusual clauses need attention.

4. **Business impact trumps legal language.** Translate every risk into business terms: "This could cost us $X" or "This means we can't do Y."

5. **Check the "boring" sections.** Miscellaneous, General Terms, and Definitions often hide important provisions.

6. **Document your analysis.** Keep contract summaries for reference in disputes or renewals.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Contract summaries are accurate and complete
- [ ] Business teams understand what they're signing
- [ ] Key risks are identified before signing
- [ ] Review turnaround time decreases
- [ ] Negotiation is focused on what matters
- [ ] No surprises from signed contracts

**Track over time:**
- Contract review cycle time
- Issues identified vs. missed
- Negotiation success rate on flagged issues
- Post-signature disputes or surprises
- Stakeholder satisfaction with summaries

---

## Variations

### Due Diligence Contract Review
For M&A or investment:
```
Review these contracts for due diligence purposes.

Context: [Acquisition, investment, partnership]
Material threshold: [Contract value threshold]

For each contract, identify:
- Key terms and obligations
- Change of control provisions
- Assignment restrictions
- Unusual or concerning terms
- Upcoming renewals or terminations
- Potential liabilities

Output: Due diligence summary matrix
```

### Vendor Contract Comparison
For evaluating multiple vendors:
```
Compare these vendor contracts.

Vendor A: [Paste contract]
Vendor B: [Paste contract]

Compare on:
- Pricing structure and total cost
- Service levels and guarantees
- Liability and risk allocation
- Term and flexibility
- Data protection

Output: Side-by-side comparison with recommendation
```

### Contract Renewal Analysis
For existing contracts up for renewal:
```
Analyze this contract for renewal negotiation.

Current contract: [Paste contract]
Our experience: [Any issues during the term]
Market changes: [What's different now]

Identify:
- Terms to improve
- Terms that worked well
- New protections to add
- Leverage points for negotiation
```

### Policy/Terms of Service Review
For standard form agreements:
```
Review this terms of service/privacy policy.

Document: [Paste terms]
Our role: [Customer/user]

Identify:
- What rights we're giving up
- What obligations we're accepting
- Unusual or one-sided terms
- Data collection and use provisions
- Arbitration or class action waivers

Output: Plain-language summary for decision-makers
```

---

## Building Your Repeatable System

After reviewing several contracts, build your system:

1. **Create standard comparison templates** for your common contract types
2. **Document your standard positions** for each term category
3. **Build a clause library** of preferred language
4. **Track negotiation outcomes** to improve leverage
5. **Archive summaries** for reference

**Sample Setup:**
```
contract-review/
├── templates/
│   ├── msa-review-template.md
│   ├── nda-review-template.md
│   ├── lease-review-template.md
│   └── saas-review-template.md
├── standards/
│   ├── our-standard-positions.md
│   ├── preferred-language/
│   │   ├── liability-clauses.md
│   │   ├── termination-clauses.md
│   │   └── ip-clauses.md
│   └── red-flag-checklist.md
├── reviews/
│   ├── 2024/
│   │   ├── techvendor-msa/
│   │   │   ├── original-contract.pdf
│   │   │   ├── review-summary.md
│   │   │   ├── redline.docx
│   │   │   └── final-signed.pdf
│   │   └── [other contracts]/
└── reference/
    ├── negotiation-outcomes.md
    └── lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**extract key information → identify risks → compare to baseline → create actionable summary**—applies broadly:

| Role | Application |
|------|-------------|
| **Legal** | All contract review |
| **Procurement** | Vendor agreements |
| **Sales** | Customer contracts |
| **Real Estate** | Leases and purchase agreements |
| **HR** | Employment agreements |
| **IT** | SaaS and technology contracts |

---

## Next Steps

1. **Get the contract:** Obtain clean text version
2. **Define your standards:** Know your preferred terms
3. **Generate review:** Use this recipe for analysis
4. **Identify priorities:** Focus on what matters most
5. **Prepare for negotiation:** Create redlines and talking points
6. **Get legal sign-off:** Have counsel review final version

---

*Recipe #43 of 100 in the Claude Code Knowledge Worker Recipe Collection*
