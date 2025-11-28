# Change Management Documentation

**Recipe #49: From Chaotic Changes to Controlled Improvements**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 4-6 hours per change | Intermediate | PMO, Operations, IT, Any Change Manager |

---

## The Problem

Changes happen constantly—new processes, system updates, organizational restructuring, policy revisions. But changes without management create chaos. People don't know what's changing, why, or how it affects them. Implementation stumbles because dependencies weren't identified. After rollout, nobody can explain what changed or roll back if needed. The result is failed initiatives, frustrated employees, and organizations that resist change because it's always painful.

**Pain Points:**
- Changes announced without preparation
- Stakeholders surprised by impacts
- Implementation issues from missed dependencies
- No rollback plan when things go wrong
- Can't track what changed when
- Resistance because change is always disruptive
- Same change management mistakes repeated

---

## The Outcome

Comprehensive change documentation that enables smooth implementation, clear communication, and successful adoption. A structured approach that reduces resistance and increases change success rates.

**What You'll Have When Done:**
- Complete change request documentation
- Stakeholder impact analysis
- Communication plan
- Implementation timeline
- Rollback procedures
- Success metrics
- Post-implementation review template

---

## When to Use This Recipe

**Good Fit:**
- Process changes affecting multiple teams
- Technology implementations
- Organizational restructuring
- Policy and procedure updates
- System migrations
- Workflow modifications
- Any change requiring coordination

**Not a Good Fit:**
- Minor adjustments within a team
- Emergency fixes (do it, document later)
- Changes requiring executive decision first
- Highly technical changes (need technical lead)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have a defined change to implement
- [ ] You understand who's affected
- [ ] You have authority or sponsorship for the change
- [ ] You have 2-3 hours for documentation development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures change request documents
- Identifies potential impacts and stakeholders
- Creates communication plan frameworks
- Develops rollback procedures
- Generates timeline templates
- Creates training outlines

**Where Human Judgment Is Essential:**
- Actual impact assessment
- Stakeholder relationship management
- Political considerations
- Timing decisions
- Resource allocation
- Go/no-go decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Change description | What's changing | Core documentation |
| Business rationale | Why this change | Justification |
| Affected parties | Who's impacted | Stakeholder analysis |
| Current state | How things work now | Impact comparison |
| Constraints | Timeline, budget, resources | Planning |

**Sample Input:**
```
Change Management Request

CHANGE DESCRIPTION:
Transitioning from the current expense reporting system (Concur) to a new system
(Expensify) across the entire organization.

BUSINESS RATIONALE:
- Current system contract expires in 6 months
- New system is 40% cheaper
- Mobile app is significantly better rated
- Integration with our new accounting system is native
- Current system has usability complaints (30+ support tickets/month)

SCOPE:
- All employees who submit expenses (~800 people)
- Finance team who processes/approves (~15 people)
- IT team who administers (~3 people)
- Accounting team who reconciles (~5 people)

CURRENT STATE:
- Concur in use for 7 years
- Deeply embedded in workflows
- Custom integration with legacy accounting (will be retired)
- Extensive user training materials exist for current system
- Some users have developed workarounds for current system issues

AFFECTED SYSTEMS:
- Expense reporting (primary)
- Accounting system integration
- Corporate card reconciliation
- Approval workflows in current system
- SSO/authentication
- Data migration (7 years of history)

PROPOSED TIMELINE:
- Planning: Months 1-2
- Configuration: Months 2-3
- Pilot: Month 3
- Training: Months 3-4
- Migration: Month 4
- Full cutover: Month 5
- Contract end: Month 6

CONSTRAINTS:
- Must be complete before current contract expires
- No additional IT headcount
- Budget: $50K implementation, $120K annual (down from $200K)
- Minimal business disruption during Q4 (Oct-Dec)

RISKS IDENTIFIED:
- User resistance to learning new system
- Data migration complexity
- Integration timing with accounting system project
- Q4 timing conflict with busy period
- Custom approvals may not transfer cleanly
```

---

## Step-by-Step Implementation

### Step 1: Define the Change
**Time: 10-15 minutes**

Document clearly:
- What is changing?
- Why is it changing?
- Who is affected?
- What's the scope?
- What's the timeline?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Change Management Prompt
**Time: 7-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Change Management Documentation**

```
Please help me create comprehensive change management documentation.

CHANGE OVERVIEW:
[What is changing]

BUSINESS RATIONALE:
[Why this change is being made]

SCOPE:
[Who and what is affected]

CURRENT STATE:
[How things work today]

PROPOSED TIMELINE:
[Key dates and milestones]

CONSTRAINTS:
[Timeline, budget, resource limitations]

KNOWN RISKS:
[Identified risks or concerns]

PLEASE CREATE:

1. CHANGE REQUEST DOCUMENT

   Change ID: [Placeholder]
   Change Name: [Name]

   A. CHANGE SUMMARY
      - Description (one paragraph)
      - Business justification
      - Sponsor/Owner
      - Requested implementation date

   B. DETAILED DESCRIPTION
      - What is changing (specific)
      - What is NOT changing
      - Relationship to other initiatives

   C. BUSINESS CASE
      - Problem being solved
      - Benefits expected
      - Costs and investment
      - ROI or payback period

2. IMPACT ASSESSMENT

   A. Stakeholder Impact Analysis
   | Stakeholder Group | # Affected | Impact Level | Key Concerns | Engagement Approach |

   Impact levels: High (significant change to daily work), Medium (moderate adjustment), Low (minimal change)

   B. System/Process Impact
   | System/Process | Current State | Future State | Gap/Change |

   C. Risk Assessment
   | Risk | Likelihood | Impact | Mitigation | Owner |

   D. Dependencies
   - Prerequisites: [What must happen first]
   - Parallel activities: [What's happening simultaneously]
   - Post-implementation: [What depends on this completing]

3. COMMUNICATION PLAN

   A. Communication Matrix
   | Audience | Message | Channel | Timing | Owner |

   B. Key Messages by Audience
   For each stakeholder group:
   - What they need to know
   - Why they should care
   - What's in it for them
   - What they need to do

   C. Communication Timeline
   | Phase | Activity | Audience | Date |

4. IMPLEMENTATION PLAN

   A. Phase Breakdown
   For each phase:
   - Objectives
   - Key activities
   - Deliverables
   - Timeline
   - Resources needed
   - Success criteria

   B. Detailed Timeline
   | Week | Activities | Milestones | Owner |

   C. Resource Requirements
   | Resource Type | Quantity | Duration | Cost |

5. TRAINING AND SUPPORT

   A. Training Plan
   | Audience | Training Type | Duration | Timing | Materials |

   B. Support Plan
   - During implementation: [Support approach]
   - Post-implementation: [Ongoing support]
   - Escalation path: [How to get help]

6. ROLLBACK PLAN

   A. Rollback Triggers
   - Conditions that would trigger rollback
   - Who makes the decision
   - Escalation process

   B. Rollback Procedure
   - Steps to reverse the change
   - Data recovery process
   - Communication if rolling back
   - Timeline for rollback

7. SUCCESS METRICS

   | Metric | Baseline | Target | Measurement Method | Timeline |

8. POST-IMPLEMENTATION REVIEW

   Template for after go-live:
   - What went well
   - What could improve
   - Issues encountered
   - Metrics vs. targets
   - Lessons learned
   - Open items

9. APPROVALS

   | Approver | Role | Date | Signature |

10. APPENDICES

    - Detailed project plan
    - Training materials outline
    - FAQ template
    - Communication templates
```

---

### Step 4: Validate Impact Assessment
**Time: 20-30 minutes**

Review with stakeholders:
- Did we identify all affected parties?
- Is the impact level accurate?
- Are there concerns we missed?
- Are dependencies correctly mapped?

---

### Step 5: Refine Implementation Plan
**Time: 15-20 minutes**

**To improve timeline:**
```
The timeline assumes [X]. Is this realistic given [constraints]? What are the critical path items? Where is there flexibility?
```

**To enhance communication plan:**
```
Add more detail to communications for [stakeholder group]. They're highly impacted and will need:
- More frequent updates
- Different messaging
- Different channels
```

**To strengthen rollback plan:**
```
The rollback plan needs more detail for [scenario]. What specifically would we do if [specific failure]? How long would rollback take?
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create the final change management package:

1. CHANGE REQUEST (Formal Document)
   For approval and governance

2. EXECUTIVE SUMMARY (1 page)
   For leadership briefing

3. STAKEHOLDER PRESENTATION
   Slide outline for announcing the change

4. FAQ DOCUMENT
   Anticipated questions and answers

5. TRAINING OUTLINE
   Structure for training materials

6. QUICK REFERENCE GUIDE
   For during and after implementation

7. TRACKING TEMPLATE
   For monitoring implementation progress
```

---

## Example Output

Below is an abbreviated change management example:

---

> **CHANGE REQUEST**
>
> ---
>
> | Change ID | CHG-2024-042 |
> |-----------|--------------|
> | Change Name | Expense System Migration (Concur → Expensify) |
> | Sponsor | CFO |
> | Change Manager | [Name] |
> | Requested Go-Live | April 1, 2025 |
>
> ---
>
> ## 1. Change Summary
>
> ### Description
>
> This change replaces the current expense reporting system (Concur) with a new platform (Expensify) for all employees. The change includes system configuration, data migration, integration with the new accounting system, user training, and parallel operation before full cutover.
>
> ### Business Justification
>
> - **Cost reduction:** Annual savings of $80,000 (40% reduction)
> - **Improved user experience:** Mobile app rated 4.7 vs. current 3.2
> - **Strategic alignment:** Native integration with new accounting system
> - **Support reduction:** Expected 50% reduction in expense-related support tickets
>
> ### What IS Changing
> - Expense submission interface and mobile app
> - Receipt capture and processing
> - Approval workflow system
> - Reporting and analytics
> - Integration with accounting
>
> ### What IS NOT Changing
> - Expense policy and reimbursement rules
> - Approval hierarchy and limits
> - Corporate card program
> - Reimbursement timing
>
> ---
>
> ## 2. Impact Assessment
>
> ### Stakeholder Impact
>
> | Group | # Affected | Impact | Key Concerns | Approach |
> |-------|------------|--------|--------------|----------|
> | All employees | 800 | Medium | Learning new system, losing familiar workflow | Training, champions, support |
> | Frequent travelers | 150 | High | Heavy system users, many custom workflows | Early pilot, dedicated training |
> | Finance approvers | 50 | High | New approval interface, workflow changes | Admin training, preview period |
> | Finance processing | 15 | High | New tools, integration testing | Deep training, parallel period |
> | IT administration | 3 | Medium | New system administration | Technical training, vendor support |
>
> ### System Impact
>
> | System | Change |
> |--------|--------|
> | Expense reporting | Full replacement |
> | Accounting integration | New integration (Expensify native) |
> | SSO | New SAML configuration required |
> | Data warehouse | New data feeds to configure |
> | Audit systems | Update for new data source |
>
> ### Risk Assessment
>
> | Risk | Likelihood | Impact | Mitigation |
> |------|------------|--------|------------|
> | User resistance | High | Medium | Early communication, champion network, responsive support |
> | Data migration errors | Medium | High | Thorough testing, validation period, fallback access to historical |
> | Q4 timing conflict | Medium | Medium | Complete training before Q4, enhanced support during Q4 |
> | Integration delays | Medium | High | Early integration testing, parallel operation period |
> | Approval workflow gaps | Low | Medium | Map all scenarios, test with approvers |
>
> ---
>
> ## 3. Communication Plan
>
> ### Key Messages by Audience
>
> **All Employees:**
> - We're upgrading to a better expense app that's faster and easier to use
> - The mobile app is significantly improved for receipt capture
> - Your expense history will be migrated—nothing is lost
> - Training will be provided before the switch
> - Support will be available throughout the transition
>
> **Finance Team:**
> - New system gives you better reporting and analytics
> - Approval workflows will be configured to match current process
> - You'll have preview access before full rollout
> - We need your input on workflow requirements
>
> **Leadership:**
> - This change saves $80K annually
> - Improves employee experience with expenses
> - Aligns with accounting system modernization
> - Timeline designed to minimize Q4 disruption
>
> ### Communication Timeline
>
> | When | What | Audience | Channel |
> |------|------|----------|---------|
> | Week 1 | Announcement | All employees | Email from CFO |
> | Week 2 | FAQ published | All | Intranet |
> | Week 4 | Pilot kickoff | Pilot group | Meeting + email |
> | Week 6 | Pilot results | All | Town hall |
> | Week 8 | Training schedule | All | Email |
> | Week 10 | Training begins | Groups | Per schedule |
> | Week 14 | Go-live announcement | All | Email + signage |
> | Week 16 | Go-live | All | All channels |
>
> ---
>
> ## 4. Implementation Plan
>
> ### Phase Overview
>
> | Phase | Duration | Dates | Focus |
> |-------|----------|-------|-------|
> | Planning | 4 weeks | Nov 1-30 | Requirements, configuration design |
> | Configuration | 4 weeks | Dec 1-31 | System setup, integrations |
> | Pilot | 3 weeks | Jan 1-21 | Test with select users |
> | Training | 4 weeks | Jan 22-Feb 18 | All users trained |
> | Migration | 2 weeks | Feb 19-Mar 4 | Data migration, validation |
> | Go-Live | 1 week | Mar 5-11 | Cutover and support |
> | Hypercare | 4 weeks | Mar 12-Apr 8 | Enhanced support |
>
> ### Detailed Timeline
>
> **Phase 1: Planning (Nov 1-30)**
> - [ ] Requirements documentation complete - Nov 8
> - [ ] Approval workflow mapping - Nov 15
> - [ ] Integration specifications - Nov 15
> - [ ] Configuration design - Nov 22
> - [ ] Training plan finalized - Nov 30
> - [ ] Communication plan approved - Nov 30
>
> **Phase 2: Configuration (Dec 1-31)**
> - [ ] Base system configured - Dec 15
> - [ ] SSO integration complete - Dec 15
> - [ ] Approval workflows configured - Dec 20
> - [ ] Accounting integration built - Dec 22
> - [ ] Test environment ready - Dec 31
>
> **Phase 3: Pilot (Jan 1-21)**
> - [ ] Pilot users identified and briefed - Jan 3
> - [ ] Pilot training complete - Jan 7
> - [ ] Pilot go-live - Jan 8
> - [ ] Pilot feedback collection - Jan 8-20
> - [ ] Pilot issues resolved - Jan 21
> - [ ] Pilot sign-off - Jan 21
>
> **Phase 4: Training (Jan 22-Feb 18)**
> - [ ] Training materials finalized - Jan 22
> - [ ] Wave 1 training (Finance) - Jan 22-28
> - [ ] Wave 2 training (Frequent travelers) - Jan 29-Feb 4
> - [ ] Wave 3 training (All others) - Feb 5-18
> - [ ] Training completion confirmed - Feb 18
>
> **Phase 5: Migration (Feb 19-Mar 4)**
> - [ ] Historical data migration - Feb 19-25
> - [ ] Migration validation - Feb 26-Mar 1
> - [ ] User acceptance testing - Mar 2-4
> - [ ] Migration sign-off - Mar 4
>
> **Phase 6: Go-Live (Mar 5-11)**
> - [ ] Final cutover - Mar 5
> - [ ] Concur access removed - Mar 8
> - [ ] All users on Expensify - Mar 8
> - [ ] First week issues resolved - Mar 11
>
> ---
>
> ## 5. Training Plan
>
> | Audience | Format | Duration | Content |
> |----------|--------|----------|---------|
> | Finance processing | In-person workshop | 4 hours | Admin functions, reporting, integration |
> | Finance approvers | In-person workshop | 2 hours | Approval workflow, exceptions |
> | Frequent travelers | Live webinar | 1 hour | Full submission process, mobile app |
> | All employees | Self-paced online + QRG | 30 min | Basic submission, receipt capture |
>
> ### Support During Transition
>
> - **Dedicated Slack channel:** #expense-help
> - **Drop-in office hours:** Daily 2-3 PM for first 2 weeks
> - **Champion network:** 1 champion per 50 employees for peer support
> - **Escalation:** expense-support@company.com monitored by Finance
>
> ---
>
> ## 6. Rollback Plan
>
> ### Rollback Decision Criteria
>
> Consider rollback if:
> - Data integrity issues affecting more than 10% of transactions
> - Critical integration failure not resolvable within 24 hours
> - Security vulnerability requiring immediate action
> - User-blocking bugs affecting majority of users
>
> **Decision maker:** CFO with input from IT Director
>
> ### Rollback Procedure
>
> If rollback is triggered:
>
> 1. **Immediate (0-2 hours)**
>    - Notify all users via email blast
>    - Re-enable Concur access
>    - Post notice on Expensify login page
>
> 2. **Short-term (2-24 hours)**
>    - Extract any transactions entered in Expensify
>    - Re-key into Concur or queue for later migration
>    - Communicate timeline for re-attempt
>
> 3. **Recovery (1-5 days)**
>    - Root cause analysis
>    - Fix identified issues
>    - New go-live date determination
>    - Updated communication
>
> ### Data Preservation
>
> - Concur data remains accessible (read-only) for 90 days post-cutover
> - Daily backups of Expensify for first 30 days
> - Manual extraction capability from both systems
>
> ---
>
> ## 7. Success Metrics
>
> | Metric | Baseline | Target | Measurement |
> |--------|----------|--------|-------------|
> | Support tickets | 30/month | 15/month | IT ticket system |
> | Submission time | 15 min avg | 8 min avg | System analytics |
> | Mobile usage | 20% | 60% | System analytics |
> | Training completion | N/A | 95% | LMS tracking |
> | User satisfaction | 3.2/5 | 4.0/5 | Survey at 30 days |
> | On-time implementation | N/A | Yes | Project tracking |
> | Budget adherence | N/A | ±10% | Finance tracking |
>
> ---
>
> ## 8. Approvals
>
> | Approver | Role | Date | Status |
> |----------|------|------|--------|
> | [Name] | CFO (Sponsor) | | Pending |
> | [Name] | IT Director | | Pending |
> | [Name] | Finance Director | | Pending |
> | [Name] | Change Advisory Board | | Pending |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Stakeholder resistance | Not involved early | Ask: "How can we engage [group] in design, not just announcement?" |
| Timeline unrealistic | Dependencies not mapped | Ask: "What must happen before this? Are we accounting for it?" |
| Communication gaps | Audiences missed | Ask: "Who else is affected that we haven't considered?" |
| Training inadequate | One-size-fits-all | Ask: "What's the right training for each audience based on impact?" |
| Rollback plan weak | Not enough detail | Ask: "If we had to roll back, what exactly would we do step by step?" |
| Success undefined | Vague objectives | Ask: "How will we know this succeeded? What specifically will be different?" |

---

## Tips from Experience

1. **Communicate early and often.** The surprise of change is worse than the change itself.

2. **Involve stakeholders in design.** People support what they help create.

3. **Plan for resistance.** It's not "if" but "who" and "why." Address concerns proactively.

4. **Build in buffer time.** Changes always take longer than planned.

5. **Train for real scenarios.** Generic training doesn't stick. Use actual workflows.

6. **Hypercare is not optional.** Enhanced support post-go-live is when you build trust.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Change is implemented on time and on budget
- [ ] Stakeholders feel informed, not surprised
- [ ] Adoption meets or exceeds targets
- [ ] Support tickets are within expected range
- [ ] Rollback was not needed
- [ ] Lessons learned captured for next change

**Track over time:**
- Change success rate
- Stakeholder satisfaction
- Time to full adoption
- Support burden during transition
- Lessons learned implementation

---

## Variations

### Technology Implementation
For system implementations:
```
Create change management for technology implementation.

System: [What's being implemented]
Scope: [Who uses it, what it does]
Integration: [What it connects to]

Additional focus:
- Technical readiness criteria
- User acceptance testing plan
- Data migration plan
- System cutover checklist
```

### Organizational Change
For restructuring or reorganization:
```
Create change management for organizational change.

Change: [What's restructuring]
Impact: [Positions, reporting, roles]
Timeline: [When changes take effect]

Additional focus:
- Role transition plans
- Knowledge transfer requirements
- Emotional impact considerations
- Leadership visibility
```

### Process Change
For workflow or process changes:
```
Create change management for process change.

Process: [What's changing]
Current state: [How it works now]
Future state: [How it will work]

Additional focus:
- Process documentation
- Handoff points
- Exception handling
- Metric changes
```

### Policy Change
For policy or rule changes:
```
Create change management for policy change.

Policy: [What policy is changing]
Impact: [Who's affected, how]
Effective date: [When it takes effect]

Additional focus:
- Compliance requirements
- Exception process
- Enforcement approach
- Documentation updates
```

---

## Building Your Repeatable System

After managing several changes, build your system:

1. **Create change templates** for different change types
2. **Establish change governance** (CAB, approval process)
3. **Track change history** for learning
4. **Build stakeholder engagement playbook**
5. **Document lessons learned** for reuse

**Sample Setup:**
```
change-management/
├── templates/
│   ├── change-request.md
│   ├── impact-assessment.md
│   ├── communication-plan.md
│   ├── rollback-plan.md
│   └── post-implementation-review.md
├── active-changes/
│   ├── CHG-2024-042-expense-system/
│   │   ├── change-request.md
│   │   ├── communications/
│   │   ├── training/
│   │   └── tracking/
│   └── [other changes]/
├── completed/
│   └── [archived changes]
├── governance/
│   ├── cab-schedule.md
│   ├── approval-matrix.md
│   └── change-categories.md
└── reference/
    ├── stakeholder-playbook.md
    └── lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define change → assess impact → plan communication → implement with support → review and learn**—applies broadly:

| Role | Application |
|------|-------------|
| **PMO** | All project changes |
| **IT** | Technology implementations |
| **HR** | Organizational changes |
| **Operations** | Process improvements |
| **Compliance** | Policy updates |
| **Any** | Managing transitions |

---

## Next Steps

1. **Define the change:** What exactly is changing?
2. **Assess impact:** Who's affected and how?
3. **Generate documentation:** Use this recipe
4. **Engage stakeholders:** Validate and refine
5. **Execute with communication:** Implement per plan
6. **Review and learn:** Capture what worked

---

*Recipe #49 of 100 in the Claude Code Knowledge Worker Recipe Collection*
