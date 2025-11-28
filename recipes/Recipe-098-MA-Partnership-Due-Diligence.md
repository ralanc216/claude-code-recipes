# M&A and Partnership Due Diligence Preparation

**Recipe #98: From Scattered Documents to Organized Due Diligence Package**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 30 minutes (first time) / 15 minutes (repeat) | 10-20 hours per deal | Advanced | Corporate Development, Legal, Finance, Executives |

---

## The Problem

Due diligence for mergers, acquisitions, and partnerships involves gathering and organizing massive amounts of information—financial records, contracts, IP documentation, org charts, customer data, and more. This information is scattered across systems, formats, and teams. Delays in due diligence can kill deals, and incomplete or poorly organized documentation raises red flags with potential partners or acquirers.

**Pain Points:**
- Critical documents scattered across multiple systems, folders, and team members
- Incomplete records create gaps that slow down or derail transactions
- Inconsistent organization makes it difficult for counterparties to find information
- Missing documentation discovered too late to remediate before closing
- Unclear which documents exist, which are missing, and who owns them
- Time pressure to organize years of records in weeks
- Sensitive information requires careful access control and presentation

---

## The Outcome

A well-organized due diligence package or data room with comprehensive documentation categorized by diligence area, clear summaries of key information, and supporting materials ready for review—accelerating deal timelines and building confidence with counterparties.

**What You'll Have When Done:**
- Structured data room with intuitive folder hierarchy matching diligence requests
- Gap analysis identifying missing documents with remediation plans
- Executive summaries for each diligence area (financial, legal, IP, customers)
- Disclosure schedule documenting known issues with context
- Response protocol for handling diligence questions systematically
- Follow-up tracking ensuring all action items are addressed

---

## When to Use This Recipe

**Good Fit:**
- Preparing to be acquired (sell-side due diligence preparation)
- Evaluating acquisition targets (buy-side due diligence)
- Partnership due diligence for strategic alliances
- Strategic investment preparation for Series funding
- Joint venture documentation
- IPO readiness preparation

**Not a Good Fit:**
- Routine vendor evaluations requiring limited documentation
- Internal audits where full deal preparation isn't needed
- Non-binding exploratory conversations without LOI
- Simple licensing agreements with limited scope

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Deal type and scope defined (acquisition, partnership, investment)
- [ ] Timeline and key dates identified
- [ ] Diligence request list obtained (if available)
- [ ] Access to financial records
- [ ] Contract repository accessible
- [ ] IP documentation available
- [ ] Corporate records accessible
- [ ] HR and employee information available
- [ ] Customer and sales data accessible
- [ ] Technical documentation on hand
- [ ] You have 1-2 days for initial organization and gap analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Organizes diligence materials into structured inventories and indexes
- Creates summaries and executive overviews for different diligence areas
- Identifies documentation gaps systematically
- Drafts responses to common diligence questions
- Ensures consistent presentation across materials
- Generates disclosure schedules from known issues

**Where Human Judgment Is Essential:**
- Determining materiality of issues and what must be disclosed
- Assessing risk levels of missing documentation
- Deciding remediation vs. disclosure approach for gaps
- Prioritizing which gaps to address first given time constraints
- Evaluating what level of detail to provide in responses
- Making strategic decisions about deal structure and timing

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Deal Context | LOI terms, timeline, focus areas, deal value | Understanding scope and priorities |
| Diligence Request List | Numbered requests by category | Mapping available materials to requests |
| Available Materials | Inventory of what exists and where | Gap analysis and organization planning |
| Known Issues | IP gaps, litigation, regulatory | Disclosure schedule preparation |

---

## Step-by-Step Implementation

### Step 1: Map Requests to Available Materials
**Time: 20-30 minutes**

Gather the diligence request list and inventory what materials you have. Identify which requests you can satisfy and which have gaps.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Gap Analysis Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Map and Identify Gaps**

```
Claude, I need to prepare for due diligence.

Deal context:
[PASTE DEAL TYPE, TIMELINE, COUNTERPARTY, FOCUS AREAS]

Diligence request list:
[PASTE THE REQUEST LIST WITH SECTION NUMBERS]

Available materials:
[PASTE INVENTORY OF WHAT YOU HAVE AND WHERE IT IS]

Help me:
1. Map each request item to available materials
2. Identify gaps where we don't have requested information
3. Prioritize gaps by risk/importance to the deal
4. Estimate effort to fill each gap
5. Recommend remediation vs. disclosure approach for each gap
```

---

### Step 4: Design Data Room Structure
**Time: 5-7 minutes for Claude to process**

**PROMPT: Create Data Room Organization**

```
Design the data room structure for this deal:

Request categories: [PASTE MAIN SECTIONS FROM REQUEST LIST]
Deal type: [ACQUISITION / PARTNERSHIP / INVESTMENT]
Total documents: [APPROXIMATE COUNT IF KNOWN]

Create:
1. Folder hierarchy that maps to request list
2. Naming conventions for files
3. Index document template for each section
4. Version control approach
5. Access control recommendations (if sensitive sections)
```

---

### Step 5: Draft Summary Documents
**Time: 10-15 minutes for Claude to process per area**

**PROMPT: Create Area Summary**

```
Create a summary document for [DILIGENCE AREA]:

Area: [E.G., CUSTOMER ANALYSIS / FINANCIAL PERFORMANCE / IP PORTFOLIO]
Raw data available: [PASTE WHAT YOU HAVE]
Questions they're likely asking: [LIST KEY QUESTIONS]
Business context: [RELEVANT BACKGROUND]

Create:
1. Executive summary (1 page)
2. Key metrics and trends
3. Notable items that may need explanation
4. Supporting documents list with file references
5. Recommendations for follow-up questions
```

---

### Step 6: Address Gaps and Prepare Disclosures
**Time: 10-15 minutes for Claude to process**

**PROMPT: Gap Remediation and Disclosure**

```
Help me address these due diligence gaps:

Gap description: [E.G., "5 EARLY EMPLOYEES MISSING IP ASSIGNMENTS"]
Risk level: [HIGH / MEDIUM / LOW]
Available remediation options: [WHAT WE COULD DO]
Timeline constraint: [DAYS UNTIL CLOSING]

Provide:
1. Recommended remediation approach with timeline
2. Draft disclosure language if can't be fully remediated
3. Talking points for counterparty questions
4. Assessment of deal impact if unresolved
```

---

### Step 7: Create Response Protocol
**Time: 5-7 minutes for Claude to process**

**PROMPT: Diligence Response Guide**

```
Create a guide for responding to diligence questions:

Deal context: [PASTE]
Key sensitivities: [WHAT WE'RE CONCERNED ABOUT]
Team structure: [WHO APPROVES WHAT]

Include:
1. Response SLA (how quickly we respond)
2. Approval requirements by question type
3. Standard responses for common questions
4. What to escalate before responding
5. Documentation requirements for all responses
```

---

### Step 8: Review and Validate
**Time: 30-60 minutes**

**Check immediately:**
- All diligence requests are mapped to materials or identified as gaps
- Data room structure is logical and easy to navigate
- Critical gaps have remediation plans
- Summaries accurately reflect underlying data

**Spot-check specifics:**
- File naming is consistent throughout
- All sensitive items are flagged appropriately
- Cross-references between documents work
- Statistics in summaries match source documents

---

### Step 9: Populate and Test
**Time: Variable (2-8 hours depending on volume)**

Upload materials to data room, create indexes, and test navigation:

**PROMPT: Create Section Index**
```
Create an index document for [SECTION NAME]:

Files in section: [LIST WITH DESCRIPTIONS]
Request items covered: [LIST REQUEST NUMBERS]

Format as table with:
- File name
- Description
- Request item(s) addressed
- Date
- Notes (if any context needed)
```

---

### Step 10: Final Preparation
**Time: 30-60 minutes**

**PROMPT: Pre-Launch Checklist**
```
Create a pre-launch checklist for our data room:

Data room structure: [PASTE]
Gap analysis: [PASTE SUMMARY]
Timeline: [DAYS UNTIL ACCESS GRANTED]

Include:
- Final document verification items
- Access control verification
- Team briefing requirements
- Monitoring and tracking setup
- Communication protocol
```

---

## Example Output

Below is an abbreviated example of what a well-executed due diligence package looks like:

---

> **DUE DILIGENCE PREPARATION PACKAGE**
> **TechStart Inc. / LargeCorp Acquisition**
> *Confidential*
>
> ---
>
> ## Data Room Index
>
> **Access:** DocSend (NDA required)
> **Last Updated:** January 15, 2024
>
> ### Folder Structure
>
> ```
> TechStart Due Diligence/
> ├── 1.0 Corporate/
> │   ├── 1.1 Formation Documents
> │   ├── 1.2 Governance
> │   └── 1.3 Capitalization
> ├── 2.0 Financial/
> │   ├── 2.1 Historical Financials
> │   ├── 2.2 Current Period
> │   └── 2.3 Projections
> ├── 3.0 Customers/
> │   ├── 3.1 Customer Analysis
> │   └── 3.2 Contracts
> ├── 4.0 Intellectual Property/
> │   ├── 4.1 Patents & Trademarks
> │   └── 4.2 IP Assignments
> └── 8.0 Summaries/
>     ├── Executive Summary
>     ├── Financial Summary
>     └── Customer Summary
> ```
>
> ---
>
> ## Gap Analysis and Remediation Plan
>
> ### Critical Gaps (Must Resolve Before Closing)
>
> | Item | Gap Description | Risk | Remediation | Owner | Due |
> |------|-----------------|------|-------------|-------|-----|
> | 4.2 | IP assignments missing for 5 early employees | High | Obtain retroactive assignments | Legal | Jan 25 |
> | 5.6 | Open source compliance audit never done | High | Engage vendor for audit | Engineering | Jan 30 |
>
> ---
>
> ## Financial Summary
>
> **Revenue Performance**
>
> | Metric | 2021 | 2022 | 2023 |
> |--------|------|------|------|
> | ARR ($M) | 2.1 | 4.8 | 8.2 |
> | Growth (%) | - | 129% | 71% |
> | Customers | 45 | 89 | 142 |
>
> **Notes for Discussion:**
> - Path to profitability in Q3 2024
> - $2.1M cash on hand as of Dec 31, 2023
>
> ---
>
> ## Customer Summary
>
> **Top 10 Concentration: 34.6% of ARR**
>
> **Churn Analysis**
> - 2023 logo churn: 6%
> - 2023 revenue churn: 4%
>
> ---
>
> ## Response Protocol
>
> **Response SLA:**
> - Standard questions: 48 hours
> - Complex/sensitive: 72 hours
>
> **Approval Requirements:**
> - Financial data: CFO
> - Legal/contracts: General Counsel
> - Technology: CTO

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Can't locate all requested documents | Records not centralized or lost over time | Acknowledge gaps; provide what's available; explain why missing; offer alternatives |
| Information is outdated | Documentation not maintained | Update critical documents; note dates clearly; provide verbal updates for recent changes |
| Overwhelming volume of requests | Broad due diligence scope | Prioritize by criticality; provide summaries first; detailed backup upon request |
| Sensitive information concerns | Legitimate confidentiality needs | Understand what they really need; provide aggregates first; use clean rooms if needed |
| Questions imply concerns | Buyer has identified issues | Address directly; don't be defensive; provide context proactively; escalate internally |
| Team can't keep up with questions | Insufficient staffing or process | Implement triage system; batch responses; set realistic SLAs; request extensions if needed |

---

## Tips from Experience

1. **Start early, even before LOI.** Maintain a "deal-ready" state with organized corporate records. Don't wait for a transaction to start organizing.

2. **Be organized and make it easy.** Clear structure and good indexes save everyone time. Confusion creates doubts about the business itself.

3. **Be responsive and transparent.** Slow responses or evasive answers kill deals. If something is missing, acknowledge it and explain why.

4. **Anticipate questions proactively.** Don't wait to be asked. If something looks unusual, provide context upfront in summaries.

5. **Track everything obsessively.** Know exactly what you've shared, when, and to whom. This becomes critical if deals fall through or in future negotiations.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] All diligence requests either satisfied or gaps documented with plans
- [ ] Data room is organized and counterparty provides positive feedback on accessibility
- [ ] Response time averages within your SLA
- [ ] Critical gaps are remediated before closing
- [ ] No major surprises discovered post-close

**Track over time:**
- Time from request to response (target: <48hrs for standard)
- Completeness percentage (documents provided vs. requested)
- Buyer/partner feedback on diligence process
- Deal timeline adherence

---

## Variations

### Variation 1: Buy-Side Due Diligence
Evaluating a target company:
```
Create a due diligence review framework for evaluating [TARGET COMPANY]:

Target information: [PASTE AVAILABLE INFO]
Our investment thesis: [WHY WE'RE INTERESTED]
Key risks to evaluate: [CONCERNS]

Include:
- Request list organized by priority
- Red flag checklist
- Valuation impact assessment framework
- Integration planning considerations
```

### Variation 2: Partnership Due Diligence
Mutual evaluation for partnerships:
```
Create a partnership due diligence package:

Partnership type: [STRATEGIC ALLIANCE / JOINT VENTURE / CO-DEVELOPMENT]
Mutual diligence areas: [WHAT BOTH PARTIES NEED TO SHARE]

Include:
- Capability documentation
- Cultural fit assessment
- Integration requirements
- Governance structure
```

### Variation 3: Investment/Fundraising Due Diligence
Preparing for investors:
```
Create an investor due diligence package for [SERIES X] round:

Round details: [SIZE, LEAD INVESTOR, TIMING]
Investor focus areas: [GROWTH, UNIT ECONOMICS, TEAM]

Include:
- Pitch-aligned metrics and narratives
- Growth story documentation
- Use of funds plan
- Risk mitigation strategies
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Maintain ongoing diligence readiness.** Keep corporate records organized continuously. Update data room quarterly even when not in a deal.

2. **Create standard templates.** Build templates for each diligence area. Pre-populate what you can so you're never starting from scratch.

3. **Implement document retention policies.** Ensure contracts, board minutes, and key records are consistently stored and easily retrievable.

4. **Conduct annual internal audits.** Review your own readiness. Identify and fix gaps before they become problems in a deal.

**Sample Folder Structure:**
```
corporate-records/
├── always-current/
│   ├── corporate/
│   ├── financial/
│   └── legal/
├── diligence-templates/
│   ├── ma-dataroom-structure.md
│   ├── summary-templates/
│   └── response-protocols/
└── deal-archive/
    └── 2024-largecorp-acquisition/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**organizing scattered information for systematic evaluation**—applies broadly:

| Role | Application |
|------|-------------|
| **Compliance Audits** | Preparing for SOC 2, ISO, or regulatory examinations |
| **Customer RFPs** | Responding to enterprise customer security and capabilities questionnaires |
| **Board Reporting** | Organizing business updates and materials for board meetings |
| **Fundraising** | Preparing data rooms for investor due diligence |
| **Litigation** | Organizing discovery materials for legal proceedings |

---

## Next Steps

1. **This week:** Even if not in a deal, audit your due diligence readiness. Identify where your gaps are.

2. **Track your results:** If in a transaction, measure response times and completeness. Get counterparty feedback.

3. **Iterate:** After each deal (successful or not), document lessons learned. Update templates and processes.

4. **Maintain:** Don't let organization lapse after deals close. Stay ready for the next opportunity.

---

*Recipe #98 of 100 in the Claude Code Knowledge Worker Recipe Collection*
