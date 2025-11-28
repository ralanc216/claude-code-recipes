# Service Level Agreement Development

**Recipe #50: From Vague Promises to Enforceable Commitments**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 4-8 hours per SLA | Intermediate | Operations, IT, Customer Success, Service Management |

---

## The Problem

Service expectations live in people's heads, not in documented agreements. Customers expect one thing, providers deliver another, and nobody has a clear reference point. When disputes arise, there's no objective standard. Internal teams blame each other for service failures without clear accountability. Performance can't be measured because metrics aren't defined. The result is frustration on all sides, unmet expectations, and an inability to improve because "good" was never defined.

**Pain Points:**
- Undefined service expectations
- No clear metrics or targets
- Disputes over service quality
- No accountability for performance
- Can't measure improvement
- Internal finger-pointing
- Customer dissatisfaction despite effort

---

## The Outcome

Comprehensive service level agreements with clear metrics, measurable targets, and defined accountability. Documents that both parties can reference to assess performance and drive improvement.

**What You'll Have When Done:**
- Complete SLA document
- Defined service metrics and targets
- Measurement methodology
- Escalation procedures
- Review cadence
- Credit or remedy provisions
- Continuous improvement framework

---

## When to Use This Recipe

**Good Fit:**
- Customer-facing service commitments
- Internal service agreements between teams
- Vendor/supplier agreements
- IT service management
- Operational support functions
- Shared services arrangements

**Not a Good Fit:**
- One-off transactions
- Highly variable scope services
- Early-stage relationships without baselines
- Services without measurable outputs

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have clear understanding of the service
- [ ] You know stakeholder expectations
- [ ] You have historical performance data (if available)
- [ ] You have 2-3 hours for SLA development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures SLA documents comprehensively
- Identifies appropriate metrics
- Develops measurement methodologies
- Creates escalation frameworks
- Defines service credits/remedies
- Generates reporting templates

**Where Human Judgment Is Essential:**
- Setting realistic targets
- Balancing commitments with capabilities
- Pricing service credits
- Political considerations
- Final agreement negotiations
- Exception handling decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Service description | What's being provided | Scope definition |
| Current performance | How service performs today | Baseline setting |
| Expectations | What customers/users need | Target setting |
| Constraints | Capacity, cost, capability | Realistic commitments |
| Past issues | What's gone wrong | Focus areas |

**Sample Input:**
```
SLA Development Request

SERVICE: IT Help Desk Support

SERVICE DESCRIPTION:
Provide technical support for all employees covering:
- Hardware issues (laptops, monitors, peripherals)
- Software issues (standard applications, OS problems)
- Access issues (password resets, account lockouts)
- Network and connectivity problems
- General IT questions and how-to assistance

SERVICE PROVIDER: Internal IT Team (5 support staff)
SERVICE RECIPIENT: All employees (~500 users)

CURRENT PERFORMANCE (if known):
- Average ticket volume: 150/week
- Average first response: ~4 hours
- Average resolution: ~18 hours
- No formal priority system
- User satisfaction: Unknown (not measured)

STAKEHOLDER EXPECTATIONS:
- IT Management: Measurable performance, clear accountability
- Users: Fast response to urgent issues, reliable resolution
- Executive team: Cost-effective support, minimal business disruption
- HR: Employee satisfaction with IT support

SERVICE HOURS:
- Primary support: Monday-Friday, 8 AM - 6 PM
- Limited after-hours: Critical issues only via on-call

CONSTRAINTS:
- Current staffing cannot increase
- Budget for tools/automation: $20K
- Must support both office and remote workers
- Some issues require vendor involvement (out of our control)

KNOWN ISSUES:
- No priority differentiation (all treated equally)
- Some tickets fall through cracks
- Users don't know what to expect
- Difficult issues take too long
- No proactive communication to users
```

---

## Step-by-Step Implementation

### Step 1: Define the Service
**Time: 10-15 minutes**

Document clearly:
- What service is being provided?
- Who is the provider? Who is the recipient?
- What's in scope vs. out of scope?
- What are the current capabilities and constraints?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the SLA Development Prompt
**Time: 7-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Service Level Agreement Development**

```
Please help me develop a Service Level Agreement.

SERVICE OVERVIEW:
[What service is being provided]

PROVIDER: [Who provides the service]
RECIPIENT: [Who receives the service]

CURRENT STATE:
[Current performance levels if known]

EXPECTATIONS:
[What stakeholders expect]

CONSTRAINTS:
[Limitations on what can be committed]

SERVICE HOURS:
[When service is available]

KNOWN ISSUES:
[Current problems to address]

PLEASE CREATE A COMPREHENSIVE SLA:

1. SLA DOCUMENT HEADER

   - Agreement name
   - Version
   - Effective date
   - Review date
   - Parties
   - Document owner
   - Approval signatures

2. SERVICE DESCRIPTION

   A. Service Overview
      - Purpose and scope
      - Service components
      - Key features

   B. In-Scope Services
      [Detailed list of what's covered]

   C. Out-of-Scope Services
      [What's NOT covered]

   D. Service Hours
      - Standard hours
      - Extended/on-call hours
      - Holiday schedule

3. SERVICE LEVEL METRICS

   For each metric:

   | Metric | Definition | Target | Measurement | Reporting |

   Include metrics for:
   - Availability
   - Response time
   - Resolution time
   - Quality (accuracy, satisfaction)
   - Volume handling

4. PRIORITY CLASSIFICATION

   | Priority | Definition | Examples | Response Target | Resolution Target |

   P1 (Critical): [Definition and targets]
   P2 (High): [Definition and targets]
   P3 (Medium): [Definition and targets]
   P4 (Low): [Definition and targets]

5. MEASUREMENT METHODOLOGY

   For each metric:
   - How it's calculated
   - Data source
   - Exclusions (what doesn't count)
   - Reporting frequency

6. ROLES AND RESPONSIBILITIES

   Service Provider:
   - [Responsibility 1]
   - [Responsibility 2]

   Service Recipient:
   - [Responsibility 1]
   - [Responsibility 2]

7. ESCALATION PROCEDURES

   | Level | Trigger | Contact | Response Expectation |

   Escalation path for:
   - SLA breaches
   - Service complaints
   - Emergency situations

8. SERVICE CREDITS/REMEDIES

   When targets are missed:
   | SLA Breach | Remedy |

   - What triggers a credit
   - How credits are calculated
   - Credit caps or limits
   - How credits are applied

9. EXCLUSIONS AND EXCEPTIONS

   SLA does NOT apply when:
   - [Exception 1]
   - [Exception 2]

   Planned maintenance windows:
   - [Schedule]

   Force majeure provisions

10. REPORTING AND REVIEW

    A. Regular Reporting
       - Report contents
       - Frequency
       - Distribution
       - Format

    B. Service Reviews
       - Review meeting frequency
       - Attendees
       - Agenda
       - Action item tracking

11. CONTINUOUS IMPROVEMENT

    - Improvement targets
    - Review process
    - Change management
    - Feedback mechanism

12. TERMS AND CONDITIONS

    - Agreement term
    - Amendment process
    - Termination provisions
    - Dispute resolution

13. APPENDICES

    - Contact information
    - Service catalog
    - Glossary of terms
    - Historical baselines
```

---

### Step 4: Validate Targets
**Time: 15-20 minutes**

Review proposed targets:
- Are targets achievable with current resources?
- Are targets meaningful to recipients?
- Do targets balance all stakeholder needs?
- Can targets be measured accurately?

---

### Step 5: Refine Specifics
**Time: 15-20 minutes**

**To adjust targets:**
```
The proposed response time target of [X] isn't achievable with current staffing. What's a realistic target given:
- 5 support staff
- 150 tickets/week average
- Current average of 4 hours

What would need to change to achieve [better target]?
```

**To add specificity:**
```
The priority definitions are still vague. Add specific examples for each priority level that users would recognize:
- P1: Examples like...
- P2: Examples like...
```

**To improve measurement:**
```
How exactly will we measure [metric]? What's the data source? What are the edge cases?
```

---

### Step 6: Create Final Package
**Time: 10 minutes**

```
Create the final SLA package:

1. FORMAL SLA DOCUMENT
   Complete agreement ready for approval

2. EXECUTIVE SUMMARY (1 page)
   Key commitments and metrics

3. USER GUIDE
   What service recipients need to know:
   - How to request service
   - What to expect
   - How to escalate

4. PROVIDER QUICK REFERENCE
   For service team:
   - Priority criteria
   - Response targets
   - Escalation triggers

5. REPORTING TEMPLATE
   Format for regular SLA reports

6. REVIEW AGENDA TEMPLATE
   For periodic service reviews
```

---

## Example Output

Below is an abbreviated SLA example:

---

> **SERVICE LEVEL AGREEMENT**
>
> **IT Help Desk Support Services**
>
> ---
>
> | Attribute | Value |
> |-----------|-------|
> | Agreement ID | SLA-IT-2024-001 |
> | Version | 1.0 |
> | Effective Date | [Date] |
> | Review Date | [Date + 6 months] |
> | Provider | IT Support Team |
> | Recipient | All Employees |
>
> ---
>
> ## 1. Service Description
>
> ### 1.1 Service Overview
>
> The IT Help Desk provides technical support to all employees for hardware, software, access, and connectivity issues. The service ensures employees can effectively use technology to perform their job functions with minimal disruption.
>
> ### 1.2 In-Scope Services
>
> - **Hardware Support:** Laptops, desktops, monitors, keyboards, mice, webcams, headsets, printers
> - **Software Support:** Standard applications (Office 365, Chrome, Zoom, Slack), operating system issues
> - **Access Management:** Password resets, account lockouts, access requests, MFA issues
> - **Network/Connectivity:** VPN issues, WiFi problems, network drive access
> - **General IT Assistance:** How-to questions, training referrals, new equipment requests
>
> ### 1.3 Out-of-Scope Services
>
> - Personal device support (unless BYOD enrolled)
> - Third-party SaaS applications (handled by app owners)
> - Facilities issues (desks, chairs, lighting)
> - Phone/mobile service (handled by mobile team)
> - Development or custom software support
>
> ### 1.4 Service Hours
>
> | Type | Hours | Coverage |
> |------|-------|----------|
> | Standard Support | Mon-Fri 8 AM - 6 PM ET | Full IT team |
> | Extended Support | Mon-Fri 6 PM - 10 PM ET | On-call (limited) |
> | Critical Only | Weekends and holidays | On-call (P1 only) |
>
> ---
>
> ## 2. Service Level Metrics
>
> ### 2.1 Key Performance Indicators
>
> | Metric | Definition | Target | Measurement |
> |--------|------------|--------|-------------|
> | **First Response Time** | Time from ticket creation to first IT response | See priority table | Ticketing system timestamps |
> | **Resolution Time** | Time from ticket creation to resolution | See priority table | Ticketing system timestamps |
> | **First Contact Resolution** | % of tickets resolved on first contact | 60% | Monthly calculation |
> | **User Satisfaction** | Post-resolution survey rating | 4.0/5.0 | Survey results |
> | **Abandonment Rate** | % of phone calls abandoned | <10% | Phone system reports |
>
> ### 2.2 Priority Classification
>
> | Priority | Definition | Examples | First Response | Resolution |
> |----------|------------|----------|----------------|------------|
> | **P1 - Critical** | Business-stopping issue affecting multiple users or executives | Server down, network outage, all-hands meeting tech failure | 15 minutes | 4 hours |
> | **P2 - High** | Significant impact to user productivity, no workaround | Laptop won't boot, primary application crash, cannot access critical system | 1 hour | 8 hours |
> | **P3 - Medium** | Moderate impact with workaround available | Secondary application issue, non-critical hardware problem, minor performance issues | 4 hours | 24 hours |
> | **P4 - Low** | Minimal impact, inconvenience | How-to questions, feature requests, non-urgent changes | 8 hours | 72 hours |
>
> **Priority Assignment:**
> - Priority is determined by IT based on impact and urgency
> - Users may request higher priority with business justification
> - Priority may be escalated or downgraded as situation evolves
>
> ---
>
> ## 3. Measurement Methodology
>
> ### 3.1 Response Time Calculation
>
> **Definition:** Time elapsed from ticket creation to first meaningful response from IT
>
> **Calculation:**
> - Clock starts: Ticket created (via portal, email, phone, or chat)
> - Clock stops: IT agent adds first response (acknowledgment alone does not count)
> - Clock pauses: Outside service hours, pending user response
>
> **Exclusions:**
> - Time waiting for user response (status: "Pending User")
> - Time outside service hours
> - Tickets created during system outages
>
> ### 3.2 Resolution Time Calculation
>
> **Definition:** Time elapsed from ticket creation to resolution confirmed
>
> **Calculation:**
> - Clock starts: Ticket created
> - Clock stops: Ticket status changed to "Resolved"
> - Clock pauses: Pending user, pending vendor, outside hours
>
> **Exclusions:**
> - Time waiting for vendor (documented)
> - Time waiting for user action
> - Time waiting for parts/hardware
> - Tickets reopened count as new tickets
>
> ---
>
> ## 4. Roles and Responsibilities
>
> ### 4.1 IT Support Team (Provider)
>
> - Respond to all tickets within defined SLA targets
> - Accurately classify and prioritize tickets
> - Communicate status updates proactively
> - Escalate appropriately when needed
> - Document all work in ticketing system
> - Conduct post-incident reviews for P1 incidents
> - Provide monthly SLA reporting
> - Continuously improve service quality
>
> ### 4.2 All Employees (Recipient)
>
> - Submit tickets via approved channels (portal, email, phone)
> - Provide accurate and complete issue descriptions
> - Respond to IT inquiries within 24 hours
> - Test solutions and confirm resolution
> - Complete satisfaction surveys
> - Report new issues separately (not on resolved tickets)
>
> ---
>
> ## 5. Escalation Procedures
>
> ### 5.1 Technical Escalation
>
> | Situation | Escalation To | Contact |
> |-----------|---------------|---------|
> | Issue beyond L1 skills | L2 Support | Internal escalation |
> | Issue beyond L2 skills | L3/Engineering | Internal escalation |
> | Vendor involvement needed | Vendor Support | IT initiates |
> | Security incident | Security Team | security@company.com |
>
> ### 5.2 Management Escalation
>
> | Trigger | Escalation To | Timeline |
> |---------|---------------|----------|
> | P1 not resolved in 4 hours | IT Manager | Immediate |
> | P2 not resolved in 8 hours | IT Manager | At 8-hour mark |
> | Repeated user complaints | IT Director | Within 24 hours |
> | SLA breach pattern | VP Technology | Monthly review |
>
> ### 5.3 User Escalation Path
>
> If users need to escalate:
>
> 1. **First:** Comment on ticket requesting escalation with reason
> 2. **Second:** Contact IT Manager ([email], [phone])
> 3. **Third:** Contact IT Director ([email])
>
> ---
>
> ## 6. Service Credits
>
> ### 6.1 When Credits Apply
>
> Service credits apply when SLA targets are missed due to IT performance, not due to exclusions or user-caused delays.
>
> | Metric | Threshold | Credit |
> |--------|-----------|--------|
> | P1 Resolution | >4 hours | 1 day support extension |
> | Monthly First Response SLA | <90% compliance | Report to IT Director |
> | Monthly Resolution SLA | <85% compliance | Corrective action plan |
> | User Satisfaction | <3.5/5.0 (3-month trend) | Service review initiated |
>
> ### 6.2 Credit Limitations
>
> - Credits do not apply for planned maintenance windows
> - Credits do not apply during force majeure events
> - Maximum credit in any month: 5 support days
> - Credits are goodwill; not for financial value
>
> ---
>
> ## 7. Reporting and Review
>
> ### 7.1 Regular Reporting
>
> **Monthly SLA Report (by 5th of following month):**
> - Ticket volume by category and priority
> - First response SLA compliance by priority
> - Resolution SLA compliance by priority
> - User satisfaction scores
> - Escalation summary
> - Notable incidents and resolutions
>
> **Distribution:** IT Leadership, Department Heads
>
> ### 7.2 Service Reviews
>
> **Monthly Review:**
> - Attendees: IT Manager, key stakeholders
> - Review: Previous month's SLA performance
> - Discussion: Trends, issues, feedback
> - Output: Action items, improvements
>
> **Quarterly Review:**
> - Attendees: IT Director, VP Technology, business leaders
> - Review: Quarterly trends, strategic issues
> - Discussion: SLA target adjustments, investment needs
> - Output: SLA amendments if needed
>
> ---
>
> ## 8. Continuous Improvement
>
> ### 8.1 Improvement Commitments
>
> IT Support commits to:
> - Review and improve processes quarterly
> - Implement user feedback where feasible
> - Increase first contact resolution by 5% annually
> - Reduce average resolution time by 10% annually
>
> ### 8.2 Feedback Mechanism
>
> - Post-ticket surveys (automated)
> - Quarterly user focus groups
> - Suggestion channel: it-feedback@company.com
> - Service review meetings
>
> ---
>
> ## 9. Terms
>
> ### 9.1 Agreement Term
>
> This SLA is effective from [date] and continues until superseded by a new version or terminated by either party with 30 days written notice.
>
> ### 9.2 Amendment Process
>
> - Either party may propose amendments
> - Proposals reviewed in quarterly service review
> - Changes require written approval from both parties
> - New version issued with changelog
>
> ### 9.3 Dispute Resolution
>
> 1. First level: IT Manager and complaining party
> 2. Second level: IT Director and department head
> 3. Third level: VP Technology (final decision)
>
> ---
>
> ## 10. Approvals
>
> | Role | Name | Signature | Date |
> |------|------|-----------|------|
> | IT Manager | | | |
> | IT Director | | | |
> | Business Representative | | | |
>
> ---
>
> ## Appendix A: Contact Information
>
> | Channel | Contact |
> |---------|---------|
> | Help Desk Portal | helpdesk.company.com |
> | Help Desk Email | helpdesk@company.com |
> | Help Desk Phone | ext. 1234 |
> | IT Manager | [Name], [email] |
> | IT Director | [Name], [email] |
> | Emergency (after hours P1) | [On-call number] |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Targets too aggressive | Not based on reality | Ask: "What's actually achievable today? Set targets 10-20% better than current" |
| Targets too easy | Aiming low to avoid misses | Ask: "Do these targets represent good service? Would customers be satisfied?" |
| Measurement unclear | Ambiguous definitions | Ask: "Walk through exactly how this is calculated with example scenarios" |
| Exclusions too broad | Avoiding accountability | Ask: "Are these legitimate exclusions or loopholes? What would the customer say?" |
| No enforcement mechanism | SLA is just words | Ask: "What happens if we miss? What are the consequences that create accountability?" |
| Stakeholders disagree | Different expectations | Ask: "Facilitate discussion on priorities. What tradeoffs are acceptable?" |

---

## Tips from Experience

1. **Set targets you can hit.** Missed SLAs damage trust more than conservative targets. Start achievable, then improve.

2. **Measure what matters.** Don't measure everything. Focus on metrics that drive behavior and matter to customers.

3. **Exclude what you can't control.** Legitimate exclusions (vendor delays, user delays) prevent unfair measurement.

4. **Make priorities clear.** Vague priority definitions lead to arguments. Use specific examples everyone recognizes.

5. **Review regularly.** SLAs get stale. Quarterly reviews keep them relevant and drive improvement.

6. **Communicate performance.** Share SLA results broadly. Transparency drives accountability and trust.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] SLA targets are met consistently (>90%)
- [ ] Stakeholders understand expectations
- [ ] Disputes are resolved by reference to SLA
- [ ] Service improves over time
- [ ] Reviews happen on schedule
- [ ] Both parties value the agreement

**Track over time:**
- SLA compliance rates
- User satisfaction trends
- Escalation frequency
- Dispute occurrence
- Improvement rate

---

## Variations

### Customer SLA
For external customer agreements:
```
Develop customer-facing SLA.

Service: [What's provided]
Customer: [Customer type]
Contract context: [Part of larger agreement]

Additional focus:
- Legally binding language
- Financial service credits
- Termination rights if SLA missed
- Limitation of liability
```

### Internal OLA
For operational level agreements between teams:
```
Develop internal OLA.

Service: [Internal service]
Provider team: [Who provides]
Consumer team: [Who receives]

Additional focus:
- Integration with upstream/downstream SLAs
- Internal escalation paths
- Collaboration expectations
- Shared accountability
```

### Vendor SLA Requirements
For requirements in vendor contracts:
```
Define SLA requirements for vendor selection.

Service being procured: [What vendor will provide]
Our requirements: [What we need]
Risk tolerance: [How critical is this]

Create:
- Required SLA terms
- Acceptable target ranges
- Measurement requirements
- Penalty/credit expectations
- Evaluation criteria
```

### SLA Review and Update
For existing SLA revision:
```
Review and update existing SLA.

Current SLA: [Paste current SLA]
Performance data: [How we've performed]
Feedback: [What stakeholders say]

Analyze:
- Where current SLA is working
- Where targets are wrong
- What's missing
- Recommended changes
```

---

## Building Your Repeatable System

After developing several SLAs, build your system:

1. **Create SLA template library** by service type
2. **Establish standard metrics catalog**
3. **Build review schedule** for all SLAs
4. **Track compliance** across services
5. **Maintain lessons learned** for improvement

**Sample Setup:**
```
sla-management/
├── templates/
│   ├── it-service-sla.md
│   ├── customer-sla.md
│   ├── vendor-sla-requirements.md
│   └── internal-ola.md
├── active-slas/
│   ├── it-helpdesk/
│   │   ├── sla-document.md
│   │   ├── monthly-reports/
│   │   └── review-notes/
│   └── [other services]/
├── metrics-catalog/
│   ├── standard-metrics.md
│   └── measurement-definitions.md
├── reporting/
│   ├── templates/
│   └── dashboards/
└── governance/
    ├── review-schedule.md
    └── amendment-process.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define service → set measurable targets → establish accountability → review and improve**—applies broadly:

| Role | Application |
|------|-------------|
| **IT** | All IT services |
| **Operations** | Internal service functions |
| **Customer Success** | Customer service commitments |
| **HR** | Shared services |
| **Finance** | Internal service delivery |
| **Any** | Any service with consumers |

---

## Next Steps

1. **Define the service:** What exactly is being provided?
2. **Gather expectations:** What do recipients need?
3. **Understand capabilities:** What can you deliver?
4. **Generate SLA:** Use this recipe
5. **Negotiate and agree:** Align stakeholders
6. **Implement and monitor:** Track from day one

---

*Recipe #50 of 100 in the Claude Code Knowledge Worker Recipe Collection*
