# Audit Preparation and Documentation

**Recipe #47: From Audit Anxiety to Organized Readiness**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 8-20 hours per audit | Intermediate | Finance, Compliance, IT, Operations |

---

## The Problem

Audit season strikes fear into organizations. Evidence is scattered across systems and people. Documentation is incomplete or outdated. Teams scramble to reconstruct what they did months ago. Simple requests take hours to fulfill because nobody knows where things are. The result is stressful, expensive audits that disrupt normal operations and often surface findings that better preparation would have prevented.

**Pain Points:**
- Evidence scattered and hard to find
- Documentation incomplete or outdated
- Last-minute scrambling for every request
- Same questions asked every audit cycle
- Findings that could have been prevented
- Business disruption during audit period
- Inconsistent response quality across teams

---

## The Outcome

Organized, audit-ready documentation with evidence mapped to requirements. Streamlined response processes that minimize disruption. Fewer findings because gaps are identified and addressed before auditors arrive.

**What You'll Have When Done:**
- Audit readiness checklist
- Evidence inventory mapped to requirements
- Gap identification and remediation tracking
- Response templates for common requests
- Organized evidence repository
- Efficient audit workflow

---

## When to Use This Recipe

**Good Fit:**
- Financial audits (annual, quarterly)
- SOC 2/SOC 1 examinations
- ISO certification audits
- Regulatory examinations
- Internal audit preparation
- Customer due diligence requests
- Compliance audits

**Not a Good Fit:**
- Fraud investigations (need specialized approach)
- Legal discovery (different requirements)
- First-time audits requiring scope definition (start there)
- Audits where control environment needs building first

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the audit scope/requirements
- [ ] You know what evidence is typically requested
- [ ] You have access to relevant systems and documentation
- [ ] You have 4-8 hours for preparation work

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Creates comprehensive checklists from requirements
- Maps evidence to control objectives
- Generates response templates
- Organizes documentation structure
- Identifies gaps in evidence
- Creates narratives from bullet points

**Where Human Judgment Is Essential:**
- Accuracy of evidence and documentation
- Control effectiveness assessment
- Materiality decisions
- Sensitive information handling
- Auditor relationship management
- Final response approval

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Audit scope | What's being examined | Requirements mapping |
| Prior audits | Previous requests and findings | Pattern identification |
| Control documentation | Policies, procedures | Completeness check |
| Evidence inventory | What exists where | Gap analysis |
| Timeline | Key dates and deadlines | Planning |

**Sample Input:**
```
Audit Preparation Request

AUDIT TYPE: SOC 2 Type II Examination

AUDIT PERIOD: January 1 - December 31, 2024
FIELDWORK: March 15-28, 2025
REPORT DUE: April 30, 2025

AUDIT SCOPE:
Trust Service Criteria:
- Security (CC)
- Availability (A)
- Confidentiality (C)

Systems in scope:
- Production cloud infrastructure (AWS)
- Customer data platform
- Internal IT systems
- Third-party integrations (list provided)

PRIOR AUDIT RESULTS:
- 2023 audit: 2 findings
  1. Incomplete access reviews (remediated)
  2. Missing change management evidence (partially remediated)
- Areas auditors focused on: access management, vendor management, incident response

CURRENT DOCUMENTATION:
- Information Security Policy (updated Jan 2024)
- Access Management Procedure (updated Mar 2024)
- Change Management Policy (updated Jun 2024)
- Incident Response Plan (updated Aug 2024)
- Vendor Management Policy (updated Nov 2023)
- Risk Assessment (completed Sep 2024)
- Business Continuity Plan (updated Feb 2024)

KNOWN GAPS/CONCERNS:
- Change management evidence still inconsistent
- New vendor onboarded without full due diligence
- Some quarterly access reviews were late
- Network diagram needs updating

TEAM RESOURCES:
- Compliance Manager (primary coordinator)
- IT Security (technical evidence)
- Engineering (change management)
- HR (personnel controls)
- Finance (billing/contract evidence)

AUDITOR: Big Four firm, same engagement team as prior year
```

---

## Step-by-Step Implementation

### Step 1: Understand Audit Requirements
**Time: 15-20 minutes**

Gather:
- Audit scope and objectives
- Trust criteria or control framework
- Prior audit requests and findings
- Timeline and key dates

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Audit Preparation Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Audit Preparation and Documentation**

```
Please help me prepare for an upcoming audit.

AUDIT INFORMATION:
- Type: [Audit type - SOC 2, Financial, ISO, etc.]
- Scope: [What's being examined]
- Period: [Audit period]
- Fieldwork dates: [When auditors will be on-site/working]
- Report deadline: [When final report is due]

AUDIT FRAMEWORK/CRITERIA:
[List specific criteria, controls, or standards being examined]

PRIOR AUDIT HISTORY:
- Findings: [Previous findings and status]
- Focus areas: [What auditors typically examine closely]

CURRENT DOCUMENTATION:
[List existing policies, procedures, evidence]

KNOWN GAPS OR CONCERNS:
[Issues you're already aware of]

TEAM RESOURCES:
[Who's available to support the audit]

PLEASE CREATE:

1. AUDIT READINESS CHECKLIST

   Pre-Audit (4+ weeks before):
   - [ ] [Task] - Owner - Due
   - [ ] [Task] - Owner - Due

   Preparation (2-4 weeks before):
   - [ ] [Task] - Owner - Due

   Final Prep (1-2 weeks before):
   - [ ] [Task] - Owner - Due

   During Fieldwork:
   - [ ] [Task] - Owner - Ongoing

   Post-Audit:
   - [ ] [Task] - Owner - Due

2. EVIDENCE MAPPING MATRIX

   | Control/Criteria | Evidence Required | Current Status | Location | Owner | Gap? |

   Organize by category:
   - [Category 1]
   - [Category 2]
   - etc.

3. GAP ANALYSIS AND REMEDIATION

   For each identified gap:
   | Gap | Risk | Remediation | Owner | Due | Status |

   Prioritize by:
   - Critical: Will result in finding if not addressed
   - High: Likely to be identified
   - Medium: May be identified
   - Low: Minor improvement opportunity

4. EVIDENCE REPOSITORY STRUCTURE

   Recommended folder structure:
   ```
   [Folder structure for organizing evidence]
   ```

   Naming conventions:
   - [Convention guidance]

5. COMMON REQUEST TEMPLATES

   For frequently requested items, create response templates:

   Request Type 1: [e.g., Population and samples]
   - What to provide
   - How to format
   - Common issues to avoid

   Request Type 2: [e.g., Policy documentation]
   - What to provide
   - How to format
   - Common issues to avoid

   [Continue for common request types]

6. PRIOR FINDING FOLLOW-UP

   For each prior finding:
   | Finding | Remediation Status | Evidence of Remediation | Risk if Not Complete |

7. WALKTHROUGH PREPARATION

   For each control requiring walkthrough:
   | Control | Process Owner | Key Steps to Demonstrate | Supporting Evidence |

8. SAMPLE TESTING PREPARATION

   For each control tested via sampling:
   | Control | Population | Sample Size Expected | How to Pull Sample | Common Exceptions |

9. COMMUNICATION PLAN

   - Kickoff meeting agenda
   - Status update cadence
   - Escalation process
   - Key contacts by area

10. RISK AREAS TO MONITOR

    Controls or areas where findings are most likely:
    | Area | Risk | Mitigation |

11. TIMELINE WITH MILESTONES

    Week-by-week preparation plan:
    | Week | Focus Areas | Key Deliverables | Owner |
```

---

### Step 4: Validate Evidence Inventory
**Time: 30-45 minutes**

For each required evidence item:
- Does it exist?
- Is it current?
- Does it cover the full audit period?
- Is it accessible?

---

### Step 5: Address Gaps
**Time: Varies based on gaps**

For each gap identified:

```
Help me develop a remediation plan for [specific gap].

Current state: [What exists or doesn't]
Audit criteria: [What's required]
Time available: [How long until audit]

What are my options:
1. Fully remediate before audit
2. Partially remediate and document plan
3. Prepare response if finding is issued

For each option, what would I need to do?
```

---

### Step 6: Organize and Package
**Time: 20-30 minutes**

```
Help me organize the audit evidence package:

1. CREATE EVIDENCE INDEX
   Master list of all evidence:
   | ID | Description | Criteria Addressed | Filename | Location |

2. EVIDENCE PACKAGE CHECKLIST
   For handoff to auditors:
   - [ ] Evidence organized by criteria
   - [ ] File naming consistent
   - [ ] Index complete and accurate
   - [ ] Sensitive items marked
   - [ ] Version control clear

3. RESPONSE PLAYBOOK
   Quick reference for common scenarios:
   - How to handle sample requests
   - How to handle additional documentation requests
   - How to handle clarification questions
   - How to escalate issues
```

---

## Example Output

Below is an abbreviated audit preparation example:

---

> **SOC 2 AUDIT PREPARATION**
>
> **Audit Period:** January 1 - December 31, 2024
> **Fieldwork:** March 15-28, 2025
>
> ---
>
> ## 1. Audit Readiness Checklist
>
> ### Pre-Audit (By February 15)
>
> - [ ] Confirm audit scope and timing with auditors - Compliance Mgr - Feb 1
> - [ ] Review prior year findings and remediation status - Compliance Mgr - Feb 5
> - [ ] Update control documentation for currency - All control owners - Feb 10
> - [ ] Complete evidence inventory - Compliance Mgr - Feb 12
> - [ ] Address identified gaps - Various - Feb 15
> - [ ] Conduct internal readiness assessment - Compliance Mgr - Feb 15
>
> ### Preparation (February 15 - March 7)
>
> - [ ] Organize evidence repository - Compliance Mgr - Feb 20
> - [ ] Prepare populations for sampling - IT/Engineering - Feb 25
> - [ ] Brief process owners on walkthrough expectations - Compliance Mgr - Feb 28
> - [ ] Confirm auditor logistical requirements - Admin - Mar 1
> - [ ] Distribute audit schedule internally - Compliance Mgr - Mar 5
> - [ ] Prepare kickoff presentation - Compliance Mgr - Mar 7
>
> ### Final Prep (March 8-14)
>
> - [ ] Final evidence completeness check - Compliance Mgr - Mar 10
> - [ ] Pre-position evidence in shared repository - All owners - Mar 12
> - [ ] Confirm walkthrough participants available - All owners - Mar 14
> - [ ] Set up auditor workspace/access - IT - Mar 14
>
> ### During Fieldwork (March 15-28)
>
> - [ ] Daily status check with engagement team - Compliance Mgr - Daily
> - [ ] Track open requests - Compliance Mgr - Ongoing
> - [ ] Escalate issues same-day - Compliance Mgr - As needed
> - [ ] Document any verbal discussions - All - Ongoing
>
> ### Post-Audit (March 29 - April 30)
>
> - [ ] Review draft findings - Compliance Mgr - Within 5 days
> - [ ] Prepare management responses - Control owners - Within 10 days
> - [ ] Review draft report - Executive team - Before final
> - [ ] Document lessons learned - Compliance Mgr - Within 2 weeks
>
> ---
>
> ## 2. Evidence Mapping Matrix
>
> ### Security (CC Series)
>
> | Criteria | Evidence Required | Status | Location | Owner | Gap? |
> |----------|-------------------|--------|----------|-------|------|
> | CC6.1 - Access Control | Access policy; provisioning procedure; access review evidence; terminated user evidence | ✅ | /Security/Access | IT Security | No |
> | CC6.2 - System Registration | Asset inventory; device management procedure | ✅ | /Security/Assets | IT | No |
> | CC6.3 - Provisioning | Role-based access matrix; approval evidence | ⚠️ | /Security/Access | IT Security | Partial |
> | CC6.6 - Logical Access | Access logs; PAM evidence; MFA enforcement | ✅ | /Security/Logs | IT Security | No |
> | CC6.7 - System Components | Network diagram; firewall configs; segmentation | ⚠️ | /Security/Network | Engineering | Yes - diagram outdated |
> | CC7.1 - Vulnerability Management | Scan reports; remediation evidence; pentest reports | ✅ | /Security/Vuln | IT Security | No |
> | CC7.2 - Incident Monitoring | SIEM alerts; incident tickets; response evidence | ✅ | /Security/Incidents | IT Security | No |
> | CC8.1 - Change Management | Change policy; change tickets; approval evidence | ⚠️ | /Engineering/Changes | Engineering | Partial - inconsistent |
>
> ### Availability (A Series)
>
> | Criteria | Evidence Required | Status | Location | Owner | Gap? |
> |----------|-------------------|--------|----------|-------|------|
> | A1.1 - Capacity Planning | Capacity reports; scaling evidence; thresholds | ✅ | /Operations/Capacity | Engineering | No |
> | A1.2 - Recovery | BCP/DR plans; test results; recovery procedures | ✅ | /Operations/DR | IT | No |
> | A1.3 - Environmental Controls | AWS infrastructure documentation; redundancy evidence | ✅ | /Operations/Infra | Engineering | No |
>
> ### Confidentiality (C Series)
>
> | Criteria | Evidence Required | Status | Location | Owner | Gap? |
> |----------|-------------------|--------|----------|-------|------|
> | C1.1 - Confidential Information | Classification policy; handling procedures | ✅ | /Compliance/Data | Compliance | No |
> | C1.2 - Disposal | Disposal procedure; destruction evidence | ✅ | /Compliance/Data | IT | No |
>
> ---
>
> ## 3. Gap Analysis and Remediation
>
> | # | Gap | Risk | Remediation | Owner | Due | Status |
> |---|-----|------|-------------|-------|-----|--------|
> | 1 | Network diagram outdated | High - Auditors will request current diagram | Update diagram to reflect current architecture | Engineering | Feb 15 | In progress |
> | 2 | Change management evidence inconsistent | High - Prior finding, auditors will scrutinize | Implement evidence collection checklist; backfill Q4 evidence | Engineering | Feb 20 | Not started |
> | 3 | New vendor missing due diligence | Medium - May be identified during vendor testing | Complete vendor assessment; document exception if time insufficient | Procurement | Feb 15 | Not started |
> | 4 | Q3 access reviews 2 weeks late | Medium - Will appear in sample if selected | Document reason for delay; ensure Q4 on time | IT Security | N/A - historical | Document ready |
> | 5 | Access matrix not fully documented | Low - Supporting evidence exists | Complete RBAC documentation | IT Security | Feb 10 | In progress |
>
> ---
>
> ## 4. Evidence Repository Structure
>
> ```
> SOC2-2024-Audit/
> ├── 00-Index/
> │   └── Evidence-Index.xlsx
> ├── 01-Security-CC/
> │   ├── CC6-Access/
> │   │   ├── Policies/
> │   │   ├── Procedures/
> │   │   ├── Access-Reviews/
> │   │   ├── Provisioning-Evidence/
> │   │   └── Termination-Evidence/
> │   ├── CC7-Vulnerability/
> │   │   ├── Scan-Reports/
> │   │   ├── Pentest/
> │   │   └── Remediation/
> │   └── CC8-Change/
> │       ├── Policies/
> │       └── Change-Tickets/
> ├── 02-Availability-A/
> │   ├── Capacity/
> │   ├── DR-Testing/
> │   └── Infrastructure/
> ├── 03-Confidentiality-C/
> │   ├── Classification/
> │   └── Disposal/
> ├── 04-Populations/
> │   ├── Employee-List.xlsx
> │   ├── Terminated-Users.xlsx
> │   ├── Change-Tickets.xlsx
> │   ├── Access-Changes.xlsx
> │   └── Vendors.xlsx
> └── 05-Samples/
>     └── [Auditor-provided samples]
> ```
>
> **Naming Convention:**
> `[CriteriaID]-[Description]-[Date or Period].ext`
> Example: `CC6.1-AccessReview-Q4-2024.xlsx`
>
> ---
>
> ## 5. Common Request Templates
>
> ### Request: Employee Population
>
> **What to provide:**
> - Complete list of employees as of period end
> - Include: Name, Title, Department, Start Date, End Date (if applicable), System Access Level
> - Format: Excel with column headers
>
> **How to prepare:**
> 1. Pull from HRIS as of December 31, 2024
> 2. Merge with access management system data
> 3. Verify completeness against payroll
>
> **Common issues:**
> - Contractors missing (include if they have system access)
> - Access levels not mapped to roles
> - Status not clear (active vs. terminated)
>
> ---
>
> ### Request: Change Ticket Sample
>
> **What to provide:**
> For each sampled change:
> - Change ticket with full details
> - Evidence of approval before implementation
> - Evidence of testing
> - Evidence of rollback plan
> - Post-implementation verification
>
> **How to prepare:**
> 1. Provide full population first
> 2. Wait for sample selection
> 3. Pull complete ticket record from Jira
> 4. Export approval workflow from Jira
> 5. Attach any referenced documents
>
> **Common issues:**
> - Emergency changes without pre-approval (document post-approval)
> - Testing evidence in different system (consolidate)
> - Approval via email not ticket (attach email to ticket)
>
> ---
>
> ### Request: Access Review Evidence
>
> **What to provide:**
> - Screenshot or report showing review completion
> - Reviewer name and date
> - Evidence of actions taken for exceptions
> - Management sign-off
>
> **How to prepare:**
> 1. Export from access review tool
> 2. Ensure reviewer and date visible
> 3. If exceptions found, show remediation
> 4. Include manager approval email/signature
>
> **Common issues:**
> - Review done but not documented
> - Exceptions identified but no follow-up evidence
> - Missing management sign-off
>
> ---
>
> ## 6. Prior Finding Follow-Up
>
> | Finding | Original Issue | Remediation | Status | Evidence |
> |---------|---------------|-------------|--------|----------|
> | 2023-01 | Access reviews incomplete for Q2 | Implemented calendar reminders, checklist, manager accountability | ✅ Remediated | All 4 quarters complete with evidence |
> | 2023-02 | Change management evidence missing for 3 of 15 samples | Created evidence collection checklist, implemented ticket template | ⚠️ Partial | Q1-Q3 improved; Q4 being validated |
>
> **Prior Finding Discussion Points:**
> - Prepare to walk through remediation steps
> - Have before/after evidence ready
> - Be prepared for additional testing of remediated areas
>
> ---
>
> ## 7. Walkthrough Preparation
>
> | Control | Process Owner | Key Steps | Supporting Evidence |
> |---------|--------------|-----------|---------------------|
> | User Provisioning | IT Security | Request → Manager approval → IT creates access → Confirmation | Sample request ticket, approval email, access grant screenshot |
> | User Termination | IT Security + HR | HR notification → IT disables same day → Access removal verified | Termination ticket, disable timestamp, access verification |
> | Change Management | Engineering | Request → Review → Approval → Testing → Deployment → Verification | Change ticket walkthrough with all artifacts |
> | Incident Response | IT Security | Detection → Triage → Response → Resolution → Post-mortem | Sample incident with full lifecycle |
> | Vendor Assessment | Procurement | Risk assessment → Due diligence → Approval → Contracting | Vendor file walkthrough |
>
> ---
>
> ## 8. Risk Areas to Monitor
>
> | Area | Risk Level | Concern | Mitigation |
> |------|------------|---------|------------|
> | Change Management | High | Prior finding; inconsistent evidence | Extra review of Q4 changes; be transparent about improvements |
> | New Vendor | Medium | Due diligence incomplete | Complete assessment; if not possible, document exception process |
> | Late Access Reviews | Medium | Q3 reviews were late | Document reason; show Q4 on-time |
> | Network Diagram | Medium | Outdated | Update before audit; be prepared to explain delta |
>
> ---
>
> ## 9. Communication Plan
>
> **Kickoff Meeting Agenda:**
> 1. Introductions (5 min)
> 2. Scope confirmation (10 min)
> 3. Timeline and logistics (10 min)
> 4. Prior year finding status (10 min)
> 5. Process for requests and questions (5 min)
> 6. Q&A (20 min)
>
> **Status Updates:**
> - Daily 15-minute check-in at 4 PM
> - Open request tracker shared daily
> - Escalation within 24 hours if blocked
>
> **Contacts:**
> | Area | Primary | Backup |
> |------|---------|--------|
> | Overall coordination | [Compliance Mgr] | [CFO] |
> | Access controls | [IT Security Lead] | [IT Director] |
> | Change management | [Engineering Mgr] | [CTO] |
> | Vendor management | [Procurement Mgr] | [CFO] |
> | HR controls | [HR Director] | [CEO] |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Evidence doesn't exist | Control not operating | Either implement quickly or prepare for finding |
| Evidence exists but scattered | No organization | Create index and organize now; document location |
| Prior finding not remediated | Remediation failed or incomplete | Be transparent; document plan to complete |
| Can't pull populations | System access issues | Resolve immediately; population delays cascade |
| Sample has exceptions | Control failures occurred | Document and explain; show they're exceptions not pattern |
| Auditor expanding scope | Concerns about control environment | Understand why; address underlying concerns |

---

## Tips from Experience

1. **Start earlier than you think.** Audit prep always takes longer than planned. Start 6-8 weeks ahead.

2. **Address prior findings first.** Auditors will look here closely. Unresolved findings multiply.

3. **Organize evidence before fieldwork.** Scrambling during fieldwork creates stress and delays.

4. **Populations are critical.** Many controls are tested via sampling. Accurate populations are foundational.

5. **Document exceptions proactively.** Known issues with documented explanations are better than surprises.

6. **Communicate, don't hide.** Auditors find issues. Being transparent builds trust and may reduce findings.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Evidence is organized before fieldwork
- [ ] Requests are fulfilled within 24-48 hours
- [ ] No surprises during audit
- [ ] Findings are limited to known issues
- [ ] Audit completes on schedule
- [ ] Clean opinion achieved (if applicable)

**Track over time:**
- Number of findings per audit
- Average request fulfillment time
- Auditor satisfaction feedback
- Preparation time vs. prior years
- Repeat findings rate

---

## Variations

### Financial Audit Preparation
For external financial audits:
```
Prepare for financial statement audit.

Audit type: [Annual financial audit]
Scope: [Financial statements and related disclosures]
Period: [Fiscal year]

Focus areas:
- Revenue recognition evidence
- Expense substantiation
- Account reconciliations
- Journal entry testing
- Related party transactions

Output: Financial audit evidence package
```

### ISO Certification Audit
For ISO standard audits:
```
Prepare for ISO [27001/9001/etc.] audit.

Certification: [New/Surveillance/Recertification]
Standard version: [Current version]
Scope: [What's in scope]

Focus areas:
- Management system documentation
- Policy compliance evidence
- Internal audit results
- Corrective action tracking
- Management review evidence

Output: ISO audit evidence package
```

### Regulatory Examination
For regulatory agency reviews:
```
Prepare for regulatory examination.

Regulator: [Agency name]
Type: [Scheduled/For cause]
Focus: [Examination scope]

Prepare:
- Regulatory compliance documentation
- Prior examination responses
- Corrective action evidence
- Current state documentation

Output: Examination readiness package
```

### Internal Audit Support
For internal audit department:
```
Prepare for internal audit.

Audit area: [Process or function]
Audit objectives: [What they're assessing]
Control framework: [What controls are relevant]

Prepare:
- Process documentation
- Control evidence
- Self-assessment results
- Known issues and remediation

Output: Internal audit response package
```

---

## Building Your Repeatable System

After several audit cycles, build your system:

1. **Maintain evergreen evidence** that's always current
2. **Create annual audit calendar** with prep milestones
3. **Build request response library** for efficiency
4. **Track findings over time** for pattern identification
5. **Document lessons learned** after each audit

**Sample Setup:**
```
audit-management/
├── current-year/
│   ├── soc2-2024/
│   │   ├── evidence/
│   │   ├── requests/
│   │   ├── findings/
│   │   └── final-report/
│   └── [other audits]/
├── evergreen-evidence/
│   ├── policies/
│   ├── procedures/
│   └── standing-populations/
├── templates/
│   ├── evidence-index.xlsx
│   ├── request-tracker.xlsx
│   ├── response-templates/
│   └── checklists/
├── prior-years/
│   └── [archived audit files]
└── reference/
    ├── audit-calendar.xlsx
    ├── lessons-learned.md
    └── finding-history.xlsx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**understand requirements → inventory evidence → address gaps → organize for delivery**—applies broadly:

| Role | Application |
|------|-------------|
| **Finance** | Financial audits, internal controls |
| **IT** | SOC audits, security assessments |
| **Compliance** | Regulatory examinations |
| **Quality** | ISO and quality audits |
| **Operations** | Process audits, certifications |
| **Legal** | Due diligence support |

---

## Next Steps

1. **Confirm audit scope:** Understand what's being examined
2. **Review prior audits:** Learn from history
3. **Inventory evidence:** Know what exists and where
4. **Identify gaps:** Find issues before auditors do
5. **Organize and prepare:** Structure for efficient delivery
6. **Execute and learn:** Track lessons for next time

---

*Recipe #47 of 100 in the Claude Code Knowledge Worker Recipe Collection*
