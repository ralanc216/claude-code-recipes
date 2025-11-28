# Requirements Documentation

**Recipe #82: From Meeting Notes to Testable Requirements**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 20 minutes (first time) / 10 minutes (repeat) | 4-8 hours per document | Intermediate | Product Managers, Business Analysts, Project Teams |

---

## The Problem

Requirements documentation is the bridge between stakeholder needs and technical implementation, yet it's often poorly done. Requirements gathered in meetings, scattered across emails, and captured in notes must be synthesized into clear, complete, and testable documentation. Poor requirements lead to rework, scope creep, missed expectations, and project failure. Creating comprehensive requirements documents takes significant time and requires balancing multiple perspectives.

**Pain Points:**
- Synthesizing fragmented information from multiple sources (meetings, emails, Slack, documents)
- Translating stakeholder desires into specific, testable acceptance criteria
- Identifying edge cases and error scenarios that stakeholders don't mention
- Ensuring requirements are complete without being overly prescriptive
- Balancing functional requirements, non-functional requirements, and constraints
- Creating user stories that are truly independent and valuable
- Maintaining traceability between business objectives and detailed requirements

---

## The Outcome

A comprehensive requirements document with user stories, functional specifications, acceptance criteria, edge cases, and dependencies—providing clear direction for development teams and a solid foundation for testing and validation.

**What You'll Have When Done:**
- User stories with Given/When/Then acceptance criteria for all functionality
- Functional specifications documenting business rules and data requirements
- Non-functional requirements covering performance, security, and compliance
- Traceability matrix linking requirements to business objectives
- Identified dependencies on systems, teams, and data
- Ready-to-estimate stories for sprint planning

---

## When to Use This Recipe

**Good Fit:**
- New feature or product development with clear user needs
- System enhancement projects building on existing functionality
- Integration requirements where systems need to communicate
- Business process automation with defined workflows
- RFP/RFI requirements development for vendor selection
- User story refinement sessions before sprint planning
- Sprint preparation to ensure stories are well-defined
- Test case derivation to guide QA efforts

**Not a Good Fit:**
- Exploratory research where requirements are intentionally vague
- Prototyping exercises focused on learning, not building
- Projects where requirements are changing daily (use lightweight stories instead)
- Internal tool development where users and developers are the same people

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have meeting notes and discovery outputs from stakeholders
- [ ] Stakeholder interviews or feedback have been gathered
- [ ] Existing system documentation is available (if applicable)
- [ ] User personas or user profiles are defined
- [ ] Business process context is understood
- [ ] Technical constraints or guidelines are documented
- [ ] Regulatory or compliance requirements are identified
- [ ] You have 3-4 hours for requirements development and review

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforming unstructured meeting notes into organized user stories
- Generating comprehensive acceptance criteria in Given/When/Then format
- Identifying edge cases and error scenarios stakeholders might miss
- Creating functional specifications with business rules and validations
- Organizing requirements by priority, user type, or feature area
- Ensuring consistency in terminology and format across all requirements
- Spotting gaps or ambiguities in stakeholder input

**Where Human Judgment Is Essential:**
- Validating that requirements truly reflect stakeholder intent
- Prioritizing conflicting requirements when stakeholders disagree
- Assessing technical feasibility and implementation complexity
- Making scope decisions about what's in or out
- Confirming non-functional requirements align with system architecture
- Obtaining stakeholder sign-off on finalized requirements

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| **Meeting Notes** | Discovery session transcripts with pain points and needs | Extracting user stories and requirements |
| **Stakeholder Emails** | Follow-up clarifications and feature requests | Refining acceptance criteria and details |
| **Existing Documentation** | Current system data models, workflows | Understanding constraints and integration points |
| **User Research** | Personas, journey maps, pain point analysis | Creating user-centered stories and scenarios |
| **Technical Constraints** | Architecture decisions, platform limitations | Documenting non-functional requirements |

**Sample Input:**
```
DISCOVERY MEETING: Order Management Enhancement
Date: [Date]
Attendees: Product (Maria), Operations (Tom), Customer Service (Lisa), IT (James)

CURRENT STATE:
- Orders come in through website, phone, and email
- Manual data entry for phone/email orders (error-prone)
- Order status only visible internally
- Customers call to check status (high volume)
- Returns processed separately, not linked to orders
- No visibility into order changes/history

PAIN POINTS DISCUSSED:
Maria: "Customers are frustrated they can't see their order status online"
Tom: "We need to see who changed an order and when - compliance requirement"
Lisa: "I spend half my day looking up orders for customers calling in"
James: "Any changes need to work with our existing inventory system"

DESIRED FUTURE STATE:
- Customers can see order status online (self-service)
- Order history tracked with audit trail
- Returns linked to original orders
- Real-time inventory integration
- Proactive notifications to customers
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 10-15 minutes**

Gather all requirement inputs:
- Compile meeting notes from discovery sessions
- Collect follow-up emails and clarifications
- Review existing system documentation
- Document known constraints and dependencies

**Tip:** Organize by topic or feature area to make analysis easier.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Requirements Analysis Prompt
**Time: 15-20 minutes for Claude to process**

---

**PRIMARY PROMPT: Requirements Extraction**

```
Claude, I need to create requirements documentation for [FEATURE/PROJECT NAME].

Here are my inputs:

Meeting notes:
[Paste discovery meeting notes]

Stakeholder feedback:
[Paste follow-up communications]

Existing context:
[Paste relevant existing documentation]

Help me:
1. Identify all requirements mentioned
2. Categorize them (functional, non-functional, constraints)
3. Flag any gaps or ambiguities
4. Suggest clarifying questions I need to answer
```

---

### Step 4: Review and Validate
**Time: 15-20 minutes**

**Check immediately:**
- All pain points mentioned in notes are addressed by requirements
- Requirements cover happy path, error cases, and edge cases
- User stories are written from user perspective (not system perspective)
- Acceptance criteria are testable and specific

**Spot-check specifics:**
- Do requirements conflict with each other?
- Are any requirements technically infeasible?
- Is anything missing that would make this feature incomplete?
- Are non-functional requirements (performance, security) defined?

---

### Step 5: Refine and Iterate
**Time: 30-45 minutes**

Use these follow-up prompts to develop complete requirements:

**To create user stories:**
```
Based on the requirements gathered, create user stories for each capability.

For each user story:
1. User type (who)
2. Action/need (what)
3. Benefit (why)
4. Format: "As a [USER], I want to [ACTION] so that [BENEFIT]"

Group by:
- Epic or feature area
- User type
- Priority (if determinable)

Include all user types identified.
```

**To develop acceptance criteria:**
```
For each user story, develop detailed acceptance criteria.

Format acceptance criteria as:
- Given [CONTEXT/PRECONDITION]
- When [ACTION TAKEN]
- Then [EXPECTED RESULT]

Include:
- Happy path scenarios
- Error scenarios
- Edge cases
- Boundary conditions
- Security/permission considerations

Be specific and testable.
```

**To document functional specifications:**
```
Create detailed functional specifications for [FEATURE NAME].

For each function, document:
1. Description
2. User interface elements
3. Business rules
4. Data requirements (inputs/outputs)
5. Validations
6. Error handling
7. Integration points
8. Audit/logging requirements
```

**To define non-functional requirements:**
```
Document non-functional requirements:

1. PERFORMANCE (response time, throughput, concurrent users)
2. SECURITY (authentication, authorization, data protection)
3. AVAILABILITY (uptime, recovery requirements)
4. USABILITY (accessibility, browser/device support)
5. COMPLIANCE (regulatory, audit requirements)
6. INTEGRATION (system dependencies, data sync)

Be specific with measurable criteria where possible.
```

---

### Step 6: Export Final Output
**Time: 10 minutes**

```
Assemble the complete requirements document with:

1. Executive Summary
2. Scope and Objectives
3. User Stories by Epic
4. Functional Specifications
5. Non-Functional Requirements
6. Data Requirements
7. Integration Requirements
8. Dependencies and Assumptions
9. Risks and Mitigation
10. Appendix (glossary, references)

Include traceability linking requirements to objectives.
Format for stakeholder review and development team use.
```

---

## Example Output

Below is an abbreviated example of what well-executed requirements documentation looks like:

---

> ### Requirements Document: Order Management Enhancement
>
> ---
>
> #### Document Information
>
> | Field | Value |
> |-------|-------|
> | Document Title | Order Management Enhancement - Requirements |
> | Version | 1.0 |
> | Author | [Business Analyst] |
> | Date | [Date] |
> | Status | Draft |
>
> ---
>
> #### 1. Executive Summary
>
> This document specifies requirements for the Order Management Enhancement project, which will enable customer self-service order tracking, implement order audit trails for compliance, and improve customer service efficiency.
>
> **Key Capabilities:**
> - Customer-facing order status tracking and history
> - Comprehensive audit trail for order changes
> - Internal tools for customer service
> - Integration with SAP inventory system
>
> **Primary Benefits:**
> - Reduce customer service call volume by 40%+
> - Meet SOC compliance requirements for audit trails
> - Improve customer satisfaction with self-service visibility
>
> ---
>
> #### 3. User Stories by Epic
>
> ##### Epic 1: Customer Order Tracking
>
> ###### US-1.1: View Order Status
> **As a** customer
> **I want to** view the current status of my orders
> **So that** I know when to expect delivery without calling customer service
>
> **Acceptance Criteria:**
>
> | AC ID | Scenario | Expected Result |
> |-------|----------|-----------------|
> | AC-1.1.1 | Given I am logged in, when I navigate to My Orders, then I see a list of my recent orders with current status |
> | AC-1.1.2 | Given I have orders in multiple statuses, when I view My Orders, then each order shows its current status (Order Received, Processing, Shipped, Delivered, Cancelled, On Hold) |
> | AC-1.1.3 | Given an order has shipped, when I view order details, then I see the estimated delivery date |
>
> **Priority:** Must Have
> **Story Points:** 5
>
> ---
>
> #### 4. Functional Specifications
>
> ##### FS-1: Order Status Values
>
> | Status Code | Customer-Facing Display | Internal Display | Description |
> |-------------|------------------------|------------------|-------------|
> | 10 | Order Received | Order Received | Order placed, not yet processing |
> | 20 | Processing | Processing | Order being prepared |
> | 30 | Shipped | Shipped | Order has shipped |
>
> **Business Rules:**
> - BR-1: "On Hold" status (91) displays as "Processing" to customers
> - BR-2: Once status reaches "Shipped" (30), it cannot revert to earlier status
> - BR-3: Estimated delivery date is required when status changes to "Shipped"
>
> ---
>
> #### 5. Non-Functional Requirements
>
> | Requirement | Specification |
> |-------------|---------------|
> | NFR-1 | Page load time < 3 seconds for 95th percentile |
> | NFR-2 | Support 10,000 concurrent users |
> | NFR-6 | Authentication required for all order views |
> | NFR-7 | Customers can only view their own orders |
>
> *(Full document includes complete specifications across all sections)*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| **Conflicting requirements** | Different stakeholders have different needs | Document both perspectives; escalate to product owner for prioritization; record rationale for decision |
| **Requirements too vague** | Stakeholders spoke in generalities | Push for specific, measurable criteria; use Given/When/Then format; ask "How would we test this?" |
| **Scope creep during documentation** | New requirements keep emerging | Document but flag as out of scope or future phase; get product owner sign-off on scope boundary |
| **Technical feasibility unknown** | Don't know if requirements are possible | Flag technical dependencies; involve tech lead early; document assumptions with risk mitigation |
| **Edge cases missed** | Only happy path documented | Explicitly ask "What could go wrong?"; review past bugs; involve QA in requirements review |
| **Acceptance criteria not testable** | Criteria use subjective language | Replace "fast," "easy," "good" with measurable criteria; use numbers, percentages, specific behaviors |

---

## Tips from Experience

1. **Start with user stories.** Keep focus on user needs, not solutions. The "so that" clause is crucial—it explains the value and helps with prioritization.

2. **Make everything testable.** Every requirement should be verifiable. If QA can't write a test case from it, the requirement isn't clear enough.

3. **Think through edge cases early.** What happens when data is missing? When the user does something unexpected? When systems are unavailable? Document these scenarios.

4. **Be consistent with terminology.** Use the same terms throughout. Create a glossary if needed. Inconsistent language causes confusion and defects.

5. **Get early feedback.** Don't wait until requirements are "perfect." Review drafts with stakeholders and developers to catch misunderstandings early.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Requirements cover 90%+ of delivered functionality (minimal requirements discovered during development)
- [ ] Defects traceable to missing/unclear requirements are < 10% of total defects
- [ ] Rework due to requirements gaps is < 15% of development effort
- [ ] Stakeholders sign off on requirements without significant rework
- [ ] Development team can start work without extensive clarification sessions

**Track over time:**
- Time from requirements draft to stakeholder approval
- Percentage of requirements that change after approval
- Defect density by requirements quality (well-specified vs. vague)

---

## Variations

### Lightweight User Story Format
**When to use:** Agile teams working in short iterations

```
Create lightweight stories with acceptance criteria only—skip detailed specifications.

For each story:
- User story statement (As a/I want/So that)
- 3-5 acceptance criteria (Given/When/Then)
- Definition of done checklist
- Estimated story points

Keep specifications verbal or in spike stories. Document just enough for the next sprint.
```

### Technical Specification Document
**When to use:** Developer-focused projects (APIs, platforms, infrastructure)

```
Create developer-focused requirements with:
- Technical user stories (As a system/API/service)
- Detailed technical specifications (data structures, algorithms, protocols)
- API contract definitions (endpoints, request/response formats)
- Performance benchmarks and SLAs
- Error handling and logging requirements

Include code examples and technical diagrams.
```

### RFP/Vendor Requirements
**When to use:** Procurement or vendor selection

```
Format requirements for vendor evaluation:

For each requirement:
- Requirement ID and description
- Priority (Must Have, Should Have, Nice to Have)
- Evaluation criteria (how proposals will be scored)
- Acceptance criteria for vendor demonstrations

Include scoring rubric and evaluation process.
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create requirement templates.** Build standard templates for user stories, functional specs, and NFRs. Include all required sections and format guidelines.

2. **Build a requirements checklist.** Document what makes requirements "complete" in your organization. Use as quality gate before moving to development.

3. **Establish review workflow.** Define who reviews requirements (stakeholders, tech lead, QA, legal) and in what order. Build approval process into your tools.

4. **Archive requirements with outcomes.** Link requirements documents to delivered features. Track which requirements were accurate vs. which changed. Learn from patterns.

**Sample Folder Structure:**
```
requirements/
├── templates/
│   ├── user-story-template.md
│   ├── requirements-doc-template.md
│   └── acceptance-criteria-checklist.md
├── active-projects/
│   └── [project-name]/
│       ├── requirements-v1.0.md
│       ├── user-stories/
│       └── review-comments/
└── archive/
    └── [year]/
        └── [completed-requirements-docs]
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming informal stakeholder needs into structured, testable specifications**—applies broadly:

| Role | Application |
|------|-------------|
| **Software Engineers** | API design documentation from integration requirements |
| **Technical Writers** | User documentation from feature specifications |
| **Data Scientists** | Model requirements from business problem statements |
| **Compliance Officers** | Control specifications from regulatory requirements |
| **Training Developers** | Learning objectives from capability requirements |

---

## Next Steps

1. **This week:** Select an upcoming feature. Gather stakeholder input and draft requirements using this recipe. Compare time spent vs. your usual process.

2. **Track your results:** Measure defects attributed to requirements quality. Track rework due to requirements gaps. Monitor stakeholder satisfaction with clarity.

3. **Iterate:** After 2-3 requirements documents, identify patterns. What requirements are consistently well-specified? Which areas need more attention? Refine your approach.

4. **Share:** Create a requirements best practices guide for your team. Include examples of well-written user stories and acceptance criteria from your work.

---

*Recipe #82 of 100 in the Claude Code Knowledge Worker Recipe Collection*
