# Policy and Procedure Documentation

**Recipe #41: From Requirements to Compliant, Actionable Policies**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 8-15 hours per policy | Intermediate | Operations, HR, Compliance, Legal |

---

## The Problem

Creating policy documents is tedious but critical. Every policy needs to address regulatory requirements, operational reality, exception handling, and enforcement—while being clear enough that people actually follow it. Most policies are either too vague to be useful or so detailed they're never read. And when regulations change, updating policies becomes a major project. The gap between "having a policy" and "having an effective policy" is where compliance failures happen.

**Pain Points:**
- Time-consuming drafting and review cycles
- Inconsistent format across policies
- Policies that don't reflect operational reality
- Unclear exception handling procedures
- Missing compliance language
- Hard to update when requirements change
- Nobody reads or follows them anyway

---

## The Outcome

Professional, comprehensive policy documents that meet compliance requirements while being operationally practical. Clear structure that enables understanding and enforcement. Living documents that can be efficiently updated as requirements evolve.

**What You'll Have When Done:**
- Complete policy document with all required sections
- Clear purpose and scope definitions
- Specific procedures and responsibilities
- Exception handling framework
- Compliance mapping to requirements
- Implementation and enforcement guidance
- Audit-ready documentation

---

## When to Use This Recipe

**Good Fit:**
- New policy development
- Policy modernization and rewrites
- Compliance-driven policy updates
- Standardizing informal practices
- Merger/acquisition policy harmonization
- Gap remediation from audits

**Not a Good Fit:**
- Quick guidance memos (overkill)
- Technical specifications (different format)
- Emergency procedures requiring legal review (start there first)
- Policies for heavily litigated areas without legal input

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the policy topic and objectives
- [ ] You know relevant regulatory requirements
- [ ] You understand operational context
- [ ] You have stakeholder input on key points
- [ ] You have 2-4 hours for initial development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Creates comprehensive policy structures
- Ensures all required sections included
- Generates appropriate compliance language
- Develops exception handling frameworks
- Maintains consistent formatting
- Creates procedure details from high-level requirements

**Where Human Judgment Is Essential:**
- Regulatory interpretation
- Operational feasibility assessment
- Exception thresholds and approvals
- Enforcement decisions
- Legal review and approval
- Stakeholder sign-off

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Policy objective | What behavior to govern | Core requirements |
| Regulations | Applicable laws/standards | Compliance mapping |
| Current practices | How things work today | Operational grounding |
| Pain points | What's not working | Problem resolution |
| Stakeholder needs | Different requirements | Balanced approach |

**Sample Input:**
```
Policy Documentation Request

POLICY TOPIC: Remote Work and Hybrid Workplace Policy

POLICY OBJECTIVE:
Establish clear guidelines for remote and hybrid work arrangements that:
- Support employee flexibility while maintaining productivity
- Ensure data security and confidentiality
- Meet legal and compliance requirements
- Provide fair and consistent treatment
- Enable effective collaboration

APPLICABLE REQUIREMENTS:
- Data Protection: Company handles sensitive customer data (financial services)
- Employment law: Multiple states with different requirements
- Tax implications: Nexus considerations for remote workers
- Security: SOC 2 Type II compliance required
- Insurance: Workers' compensation coverage considerations

CURRENT SITUATION:
- ~60% of employees work hybrid (2-3 days in office)
- ~25% fully remote (approved during COVID, grandfathered)
- ~15% fully in-office (by role requirement)
- Manager discretion currently drives decisions (inconsistent)
- No formal policy document exists

KEY DECISIONS TO ENCODE:
- Who is eligible for remote work (by role, not tenure)
- Manager vs. HR vs. executive approval authority
- Equipment and expense provisions
- Performance and communication expectations
- Office day requirements for hybrid workers
- Process to request remote work changes
- Grounds for denying or revoking remote work

STAKEHOLDER CONCERNS:
- HR: Consistency, legal compliance, fairness
- Legal: Employment law, tax nexus, liability
- IT/Security: Data protection, secure access
- Managers: Flexibility to manage teams, performance
- Employees: Clarity, fairness, flexibility
- Finance: Cost control, tax implications

POLICY FORMAT REQUIREMENTS:
- Must include revision history
- Needs clear effective date
- Requires exception process
- Should map to compliance requirements
- Needs acknowledgment/signature component
```

---

## Step-by-Step Implementation

### Step 1: Define Policy Scope and Requirements
**Time: 15-20 minutes**

Document clearly:
- What is this policy governing?
- What regulations/requirements apply?
- Who does this policy affect?
- What behaviors are you trying to enable or prevent?
- What's the operational reality to work within?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Policy Documentation Prompt
**Time: 7-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Policy and Procedure Documentation**

```
Please help me create a comprehensive policy document.

POLICY TOPIC: [What this policy covers]

POLICY OBJECTIVES:
[What outcomes should this policy achieve?]

REGULATORY/COMPLIANCE REQUIREMENTS:
- [Regulation 1]: [How it applies]
- [Regulation 2]: [How it applies]
(etc.)

CURRENT STATE:
[How things work today, if relevant]

KEY DECISIONS TO ENCODE:
[Specific requirements the policy must establish]

STAKEHOLDER REQUIREMENTS:
- [Stakeholder 1]: [Their needs/concerns]
- [Stakeholder 2]: [Their needs/concerns]
(etc.)

PLEASE CREATE A COMPLETE POLICY DOCUMENT:

1. POLICY STRUCTURE
   Include these sections:

   HEADER:
   - Policy title
   - Policy number (placeholder)
   - Effective date (placeholder)
   - Version/revision number
   - Approval authority
   - Next review date

   SECTION 1: PURPOSE
   - Clear statement of why this policy exists
   - Problems it addresses
   - Goals it achieves

   SECTION 2: SCOPE
   - Who is covered by this policy
   - What situations it applies to
   - Exclusions (what's not covered)

   SECTION 3: DEFINITIONS
   - Key terms used in the policy
   - Clear, unambiguous definitions

   SECTION 4: POLICY STATEMENT
   - The core policy requirements
   - What is required, permitted, prohibited
   - Organized logically by topic

   SECTION 5: ROLES AND RESPONSIBILITIES
   - Who does what
   - Clear accountability for each role
   - Escalation paths

   SECTION 6: PROCEDURES
   - Step-by-step processes
   - How to request, approve, implement
   - Timelines and deadlines

   SECTION 7: EXCEPTIONS
   - When exceptions may be granted
   - Who can approve exceptions
   - Documentation requirements
   - Time limits on exceptions

   SECTION 8: NON-COMPLIANCE
   - Consequences of violation
   - Progressive discipline if applicable
   - Reporting mechanisms

   SECTION 9: RELATED POLICIES
   - Connected policies to reference
   - How they interact

   SECTION 10: REVISION HISTORY
   - Version tracking table
   - Change summary format

   APPENDICES (as needed):
   - Forms
   - Checklists
   - Quick reference guides

2. COMPLIANCE MAPPING
   Table showing how each requirement maps to the policy:
   | Requirement | Policy Section | How Addressed |

3. IMPLEMENTATION GUIDE
   - Rollout recommendations
   - Communication plan outline
   - Training needs
   - Timeline considerations

4. FAQ DRAFT
   - Anticipated questions from affected parties
   - Clear answers

Write in clear, professional language. Be specific enough to be enforceable but flexible enough to accommodate reasonable situations.
```

---

### Step 4: Review for Completeness and Practicality
**Time: 20-30 minutes**

Check the draft policy:

**Completeness:**
- Are all required elements present?
- Does it address all stakeholder concerns?
- Are compliance requirements mapped?

**Practicality:**
- Can this actually be implemented?
- Are the procedures realistic?
- Will people be able to follow this?

**Clarity:**
- Are terms defined clearly?
- Is the language accessible?
- Are responsibilities unambiguous?

---

### Step 5: Refine and Strengthen
**Time: 20-30 minutes**

**To add specificity:**
```
The approval process is too vague. Specify exact timelines, required documentation, and escalation paths if decisions aren't made in time.
```

**To improve exception handling:**
```
The exception process needs more detail. Who can approve what level of exception? What documentation is required? How long can exceptions last?
```

**To ensure enforceability:**
```
Make the non-compliance section more specific. What are the actual consequences at each level? How does this connect to the performance management process?
```

**To address gaps:**
```
The policy doesn't address [specific situation]. Add a section covering this scenario and how it should be handled.
```

**To improve usability:**
```
This is too long to read easily. Create an executive summary or quick reference guide that captures the key points for day-to-day use.
```

---

### Step 6: Create Final Package
**Time: 15 minutes**

```
Create the final policy documentation package:

1. MAIN POLICY DOCUMENT
   - Complete, formatted policy
   - All sections finalized
   - Ready for legal/compliance review

2. EXECUTIVE SUMMARY
   - One-page overview of key points
   - Who needs to know what

3. QUICK REFERENCE GUIDE
   - Simplified version for daily use
   - Key procedures at a glance
   - Where to go for help

4. MANAGER GUIDE
   - What managers need to know
   - How to apply the policy
   - Decision-making guidance

5. COMMUNICATION DRAFT
   - Email announcement text
   - Key messages for rollout
   - FAQ for common questions

6. ACKNOWLEDGMENT FORM
   - Employee acknowledgment template
   - What they're confirming

7. REVIEW CHECKLIST
   For legal/compliance review:
   - [ ] Regulatory requirements addressed
   - [ ] Employment law considered
   - [ ] Consistent with other policies
   - [ ] Enforceable as written
   - [ ] Exception process appropriate
```

---

## Example Output

Below is an abbreviated policy document example:

---

> **REMOTE AND HYBRID WORK POLICY**
>
> ---
>
> | Policy Number | HRP-2024-012 |
> |---------------|--------------|
> | Effective Date | [Date] |
> | Version | 1.0 |
> | Approved By | Chief Human Resources Officer |
> | Next Review | [Date + 12 months] |
>
> ---
>
> ## 1. Purpose
>
> This policy establishes guidelines for remote and hybrid work arrangements at [Company Name]. It aims to:
>
> - Provide employees with flexible work options that support work-life balance
> - Maintain productivity, collaboration, and business continuity
> - Ensure security and confidentiality of company and customer data
> - Comply with employment, tax, and regulatory requirements
> - Create fair, consistent processes across the organization
>
> This policy replaces all prior informal remote work arrangements and provides a standardized framework for work location decisions.
>
> ---
>
> ## 2. Scope
>
> **This policy applies to:**
> - All regular full-time and part-time employees
> - All business units and departments
> - Work performed from any location other than the employee's assigned office
>
> **This policy does not apply to:**
> - Independent contractors (governed by contract terms)
> - Temporary business travel
> - Short-term illness-related work from home (under 5 consecutive days)
> - Employees on approved leave status
>
> ---
>
> ## 3. Definitions
>
> **Remote Work:** Working from a location other than a company office on a regular, ongoing basis (more than 50% of scheduled work time).
>
> **Hybrid Work:** A scheduled arrangement where an employee works from both a company office and a remote location on a regular basis.
>
> **Primary Work Location:** The address designated as the employee's official work location for tax, employment law, and administrative purposes.
>
> **Eligible Role:** A position that can be effectively performed remotely based on job responsibilities, security requirements, and business needs.
>
> **In-Office Required Role:** A position requiring physical presence due to equipment, customer interaction, or operational requirements.
>
> ---
>
> ## 4. Policy Statement
>
> ### 4.1 Work Arrangement Types
>
> [Company Name] offers three work arrangement types:
>
> | Arrangement | Description | Requirements |
> |-------------|-------------|--------------|
> | Fully Remote | Works remotely 100% of scheduled time | Approved remote role; quarterly office visits may be required |
> | Hybrid | Works in-office minimum 2 days per week | In-office days include [Tuesday] and [Thursday] |
> | In-Office | Works in-office 100% of scheduled time | Required for designated roles |
>
> ### 4.2 Eligibility
>
> Work arrangement eligibility is determined by role, not tenure or individual preference.
>
> **Roles eligible for remote or hybrid work must:**
> - Not require physical presence for daily duties
> - Not require regular access to secured physical areas
> - Not require equipment that cannot be secured remotely
> - Be compatible with remote collaboration tools
>
> **Employees in eligible roles must:**
> - Have successfully completed their probationary period
> - Have satisfactory or better performance ratings
> - Have no active performance improvement plans
> - Have manager recommendation
>
> ### 4.3 Remote Work Location Requirements
>
> All remote work locations must:
>
> - Be within the United States (international remote work requires separate approval)
> - Have reliable, secure internet connectivity (minimum 25 Mbps download)
> - Provide a private workspace suitable for confidential work
> - Comply with home office safety requirements (see Appendix A)
> - Be disclosed to HR for employment law and tax purposes
>
> **State Restrictions:** Due to employment law and tax considerations, remote work from the following states requires executive approval: [List states with complications]
>
> ### 4.4 Equipment and Expenses
>
> The company provides:
> - Laptop computer meeting security standards
> - Required software and security tools
> - VPN access
>
> The employee is responsible for:
> - Reliable internet service
> - Appropriate workspace furniture
> - Home office utilities
>
> One-time home office stipend of $[500] available for approved remote/hybrid employees.
>
> ### 4.5 Performance and Communication Expectations
>
> Remote and hybrid employees must:
>
> - Maintain equivalent productivity to in-office performance
> - Be available during core hours (9 AM - 3 PM local time, unless otherwise agreed)
> - Respond to communications within [2 hours] during work hours
> - Attend required in-person meetings and events
> - Maintain updated calendar reflecting availability
> - Participate in scheduled check-ins with manager
>
> ### 4.6 Security Requirements
>
> Remote work must comply with the Information Security Policy (ISP-2024-001). Specifically:
>
> - Work on company-provided or approved devices only
> - Use VPN for all company network access
> - Do not store sensitive data on personal devices or cloud services
> - Ensure screens are not visible to others in shared spaces
> - Report any security incidents immediately
>
> ---
>
> ## 5. Roles and Responsibilities
>
> **Employees:**
> - Submit work arrangement requests through HR system
> - Maintain eligibility requirements
> - Comply with policy requirements
> - Report changes in remote work location
>
> **Managers:**
> - Assess role eligibility for remote/hybrid work
> - Approve/deny requests based on business needs and eligibility
> - Monitor performance and compliance
> - Address issues promptly
>
> **Human Resources:**
> - Maintain policy and procedures
> - Process employment documentation for work locations
> - Track work arrangement approvals
> - Provide guidance on policy interpretation
>
> **IT Security:**
> - Ensure remote access security compliance
> - Provide technical support for remote work tools
> - Monitor for security incidents
>
> **Legal/Finance:**
> - Advise on state-specific requirements
> - Monitor tax nexus implications
> - Address employment law considerations
>
> ---
>
> ## 6. Procedures
>
> ### 6.1 Requesting a Work Arrangement Change
>
> 1. Employee submits request through [HR System] with:
>    - Proposed arrangement type
>    - Remote work location address
>    - Start date
>    - Justification
>
> 2. Manager reviews within 5 business days:
>    - Assesses role eligibility
>    - Reviews employee performance
>    - Considers team/business needs
>    - Approves, denies, or modifies request
>
> 3. If approved, HR reviews for:
>    - State employment law compliance
>    - Tax implications
>    - Documentation requirements
>
> 4. Final approval communicated within 10 business days of submission
>
> 5. Work arrangement becomes effective on agreed start date
>
> ### 6.2 Changing Remote Work Location
>
> Permanent changes to remote work location require:
> - 30 days advance notice to HR
> - Updated address in HR system
> - Review of state-specific requirements
> - Manager acknowledgment
>
> Temporary location changes (less than 30 days):
> - Manager notification required
> - Security requirements must be maintained
>
> ### 6.3 Revoking Remote Work Privileges
>
> Remote work arrangements may be modified or revoked for:
> - Performance issues (below satisfactory rating)
> - Security violations
> - Compliance concerns
> - Business needs changes
> - Role changes
>
> Revocation process:
> 1. Manager documents reason
> 2. HR reviews for consistency
> 3. Employee notified with 30 days to transition (except for cause)
> 4. Appeal available through HR
>
> ---
>
> ## 7. Exceptions
>
> ### 7.1 Exception Types
>
> | Exception Type | Approver | Duration |
> |----------------|----------|----------|
> | Temporary schedule change | Manager | Up to 30 days |
> | Extended remote work | HR Director | Up to 90 days |
> | Out-of-state remote work | VP HR + Legal | Case by case |
> | International remote work | CHRO + Legal | Maximum 30 days |
>
> ### 7.2 Exception Process
>
> 1. Submit exception request with:
>    - Specific exception requested
>    - Business justification
>    - Duration requested
>    - Risk mitigation plan (if applicable)
>
> 2. Appropriate approver reviews within 5 business days
>
> 3. Approved exceptions are:
>    - Documented in HR system
>    - Time-limited
>    - Subject to conditions
>    - Reviewed for extension if needed
>
> ---
>
> ## 8. Non-Compliance
>
> Violations of this policy may result in:
>
> | Violation | First Occurrence | Repeated Occurrence |
> |-----------|------------------|---------------------|
> | Minor (e.g., missing in-office day) | Verbal warning | Written warning |
> | Moderate (e.g., unreported location change) | Written warning | Arrangement revocation |
> | Serious (e.g., security violation) | Arrangement revocation | Disciplinary action |
>
> Employees should report suspected violations to their manager or HR.
>
> ---
>
> ## 9. Related Policies
>
> - Information Security Policy (ISP-2024-001)
> - Code of Conduct (CMP-2024-001)
> - Performance Management Policy (HRP-2024-003)
> - Expense Reimbursement Policy (FIN-2024-007)
> - Health and Safety Policy (OPS-2024-002)
>
> ---
>
> ## 10. Revision History
>
> | Version | Date | Changes | Approved By |
> |---------|------|---------|-------------|
> | 1.0 | [Date] | Initial policy | CHRO |
>
> ---
>
> ## APPENDICES
>
> **Appendix A:** Home Office Safety Checklist
> **Appendix B:** Remote Work Request Form
> **Appendix C:** Work Arrangement Agreement Template
> **Appendix D:** State-Specific Requirements Summary

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Too vague to enforce | Over-generalization | Ask: "Add specific criteria, timelines, and measurable requirements" |
| Too complex to follow | Over-engineering | Ask: "Simplify while keeping core requirements. What's minimum viable policy?" |
| Doesn't reflect reality | Disconnected from operations | Ask: "How do we make this work given [operational constraint]?" |
| Missing compliance elements | Requirements not specified | Ask: "Add sections addressing [specific regulation] requirements" |
| Exception process unclear | Insufficient detail | Ask: "Specify who approves what, required documentation, and time limits" |
| Roles and responsibilities vague | Generic assignment | Ask: "Name specific roles and their exact accountabilities" |

---

## Tips from Experience

1. **Start with purpose, not rules.** If people understand why, they're more likely to comply even in situations not explicitly covered.

2. **Define terms precisely.** Many policy disputes come from undefined or ambiguous terms.

3. **Make it scannable.** Use tables, bullets, and clear headers. Nobody reads wall-of-text policies.

4. **Include the "how," not just the "what."** Procedures matter as much as requirements.

5. **Plan for exceptions.** No policy covers every situation. A clear exception process prevents workarounds.

6. **Test with real scenarios.** Before finalizing, run common scenarios through the policy to ensure it works.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Policy passes legal and compliance review
- [ ] Stakeholders approve the document
- [ ] Employees can understand and follow it
- [ ] Common questions are answered by the policy
- [ ] Exceptions are rare and handled consistently
- [ ] Auditors find documentation adequate

**Track over time:**
- Policy-related questions to HR
- Exception requests and approvals
- Compliance audit findings
- Employee feedback on clarity
- Policy update frequency

---

## Variations

### Compliance-Heavy Policy
For highly regulated areas:
```
Create a compliance-focused policy.

Policy area: [Topic]
Regulations: [List applicable regulations with citations]
Audit requirements: [What auditors will look for]

Emphasize:
- Specific regulatory citations
- Control documentation
- Evidence requirements
- Audit trail provisions
- Regulatory change monitoring
```

### Quick Policy Update
For revising existing policies:
```
Update an existing policy.

Current policy:
[Paste current policy]

Changes needed:
[What needs to change and why]

Requirements:
- Maintain document structure
- Show changes clearly
- Update revision history
- Flag sections affected
```

### Policy Harmonization
For merging multiple policies:
```
Harmonize these policies into one:

Policy A: [Summary or full text]
Policy B: [Summary or full text]

Requirements:
- Identify conflicts
- Recommend resolution
- Create unified policy
- Note significant changes for communication
```

### Emergency/Interim Policy
For rapid policy development:
```
Create an interim policy for immediate implementation.

Situation: [What triggered the need]
Time constraint: [When needed]

Create:
- Essential policy elements only
- Clear effective period
- Path to permanent policy
- Communication urgency
```

---

## Building Your Repeatable System

After creating several policies, build your system:

1. **Establish policy template** for consistency
2. **Create review workflow** with stakeholders
3. **Maintain policy register** tracking all policies
4. **Set review schedule** for periodic updates
5. **Track compliance** and questions

**Sample Setup:**
```
policies/
├── active/
│   ├── human-resources/
│   │   ├── HRP-2024-012-remote-work.md
│   │   ├── HRP-2024-003-performance.md
│   │   └── [other HR policies]
│   ├── information-security/
│   ├── finance/
│   └── operations/
├── drafts/
│   └── [policies under development]
├── archived/
│   └── [superseded policies]
├── templates/
│   ├── policy-template.md
│   ├── procedure-template.md
│   └── review-checklist.md
├── register/
│   └── policy-register.xlsx
└── guidance/
    ├── style-guide.md
    └── review-process.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define requirements → structure comprehensively → include procedures and exceptions → make enforceable and usable**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | Employment policies, benefits, conduct |
| **Operations** | Operating procedures, standards |
| **IT** | Security policies, acceptable use |
| **Compliance** | Regulatory policies, controls |
| **Finance** | Financial controls, expense policies |
| **Legal** | Corporate governance, contracts |

---

## Next Steps

1. **Identify policy need:** What requires formal documentation?
2. **Gather requirements:** Regulatory, operational, stakeholder
3. **Generate draft:** Use this recipe for comprehensive first draft
4. **Review with stakeholders:** Legal, compliance, affected parties
5. **Finalize and approve:** Get required sign-offs
6. **Communicate and implement:** Roll out with training

---

*Recipe #41 of 100 in the Claude Code Knowledge Worker Recipe Collection*
