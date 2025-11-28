# Technical Specification Writing

**Recipe #96: From Requirements to Comprehensive Technical Specifications**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 4-8 hours per specification | Intermediate | Engineers, Technical Writers, Product Managers |

---

## The Problem

Technical specifications are critical for alignment—they ensure everyone understands what's being built before code is written. But writing good specs is hard. Engineers often skip them ("I'll just start coding"), write specs that are too vague to be useful, or create documents so detailed they're obsolete by the time they're finished. The result is miscommunication, rework, and features that don't match expectations.

**Pain Points:**
- Engineers view spec writing as bureaucratic overhead that delays actual coding
- Vague specifications leave critical details undefined, leading to implementation surprises
- Overly detailed specs become outdated before implementation begins
- Misalignment between engineering, product, and stakeholders causes costly rework
- Missing edge cases and failure scenarios discovered too late in development
- Inconsistent specification formats make reviews and handoffs difficult
- Difficulty balancing technical depth with readability for non-technical stakeholders

---

## The Outcome

Clear, comprehensive technical specifications that define requirements, architecture, interfaces, and acceptance criteria—enabling teams to build the right thing the first time with shared understanding across engineering, product, and stakeholders.

**What You'll Have When Done:**
- Structured technical specification with goals, architecture, and implementation details
- Clear interface definitions (APIs, events, data models) ready for implementation
- Identified edge cases, failure modes, and mitigation strategies
- Documented technical decisions with rationale and alternatives considered
- Acceptance criteria and success metrics for validation
- Alignment across engineering, product, and business stakeholders

---

## When to Use This Recipe

**Good Fit:**
- New feature development requiring cross-team coordination
- System architecture changes with broad impact
- API design and contracts for external or internal consumption
- Integration specifications between multiple systems
- Database schema design and migration planning
- Technical design reviews before major implementation efforts
- Complex features with multiple integration points

**Not a Good Fit:**
- Minor bug fixes or trivial changes that don't affect architecture
- Exploratory prototypes where requirements are deliberately undefined
- Emergency hotfixes requiring immediate action
- Simple configuration changes or parameter adjustments

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Product requirements or user stories documented
- [ ] Existing system context and architecture available
- [ ] Constraints and non-functional requirements identified
- [ ] Stakeholder input gathered
- [ ] Related technical documentation accessible
- [ ] Success criteria defined
- [ ] Timeline and milestone information available
- [ ] You have 2-4 hours for iterative specification development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforms requirements into structured, comprehensive specifications
- Ensures technical completeness by identifying missing sections and details
- Identifies edge cases, failure modes, and error scenarios often overlooked
- Maintains consistency with existing system architecture and patterns
- Generates appropriate diagrams, interface definitions, and data models
- Organizes complex information into readable, hierarchical structures

**Where Human Judgment Is Essential:**
- Making architectural trade-offs based on team capabilities and constraints
- Prioritizing features and determining scope boundaries
- Evaluating performance and scalability requirements for your specific context
- Deciding what level of detail is appropriate for your team and project
- Reviewing security implications and compliance requirements
- Validating that the specification aligns with business objectives

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Product Requirements | User stories, business context, success metrics | Understanding objectives and extracting functional requirements |
| Technical Context | Current architecture, tech stack, existing services | Ensuring design consistency and identifying integration points |
| Constraints | Performance targets, security requirements, timeline | Shaping technical decisions and identifying limitations |
| Stakeholder Input | Customer feedback, team concerns, business priorities | Balancing trade-offs and prioritizing features |

---

## Step-by-Step Implementation

### Step 1: Prepare Your Requirements and Context
**Time: 15-30 minutes**

Gather product requirements, existing system documentation, constraints, and stakeholder input. The more context you provide, the better Claude can help structure your specification.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Requirements Clarification Prompt
**Time: 5-10 minutes for Claude to process**

Start by clarifying and organizing your requirements before diving into technical design.

---

**PRIMARY PROMPT: Clarify and Extract Requirements**

```
Claude, I need to write a technical specification.

Product requirements:
[PASTE YOUR PRODUCT REQUIREMENTS, USER STORIES, OR FEATURE DESCRIPTION]

Help me:
1. Identify ambiguous requirements that need clarification
2. Extract explicit and implicit requirements
3. List non-functional requirements (performance, security, reliability, etc.)
4. Identify potential edge cases
5. Suggest clarifying questions for product/stakeholders
```

---

### Step 4: Design High-Level Architecture
**Time: 10-15 minutes for Claude to process**

Once requirements are clear, design the system architecture.

**PROMPT: Design Architecture**

```
Design the high-level architecture for this feature:

Requirements: [PASTE REFINED REQUIREMENTS FROM STEP 3]
Existing systems: [PASTE CURRENT ARCHITECTURE, TECH STACK, SERVICES]
Constraints: [PASTE PERFORMANCE, SECURITY, TIMELINE, TEAM CONSTRAINTS]

Provide:
1. System components needed
2. Data flow between components
3. Integration points with existing systems
4. Technology recommendations with rationale
5. Trade-offs and alternatives considered
```

---

### Step 5: Define Interfaces and Data Models
**Time: 10-15 minutes for Claude to process**

**PROMPT: Define Interfaces**

```
Define the interfaces and data models for this specification:

Architecture: [PASTE HIGH-LEVEL DESIGN FROM STEP 4]

Create:
1. API endpoint definitions (REST/GraphQL/gRPC)
2. WebSocket or event schemas (if applicable)
3. Database schema changes or new tables
4. Event/message queue formats
5. Configuration schema
```

---

### Step 6: Detail Implementation Approach
**Time: 10-15 minutes for Claude to process**

**PROMPT: Implementation Planning**

```
Detail the implementation approach:

Architecture and interfaces: [PASTE FROM PREVIOUS STEPS]
Team capacity: [DESCRIBE TEAM SIZE, SKILLS, AVAILABILITY]
Timeline: [DESCRIBE DEADLINE OR MILESTONE CONSTRAINTS]

Include:
1. Implementation phases/milestones
2. Dependencies and sequencing
3. Risk areas and mitigations
4. Testing approach (unit, integration, E2E)
5. Deployment strategy and rollout plan
```

---

### Step 7: Define Acceptance Criteria and Success Metrics
**Time: 5-10 minutes for Claude to process**

**PROMPT: Acceptance Criteria**

```
Define acceptance criteria and success metrics:

Feature requirements: [PASTE FUNCTIONAL REQUIREMENTS]
Non-functional requirements: [PASTE PERFORMANCE, SECURITY, RELIABILITY REQUIREMENTS]

Create:
1. Functional acceptance criteria (testable conditions)
2. Performance benchmarks and targets
3. Security requirements verification steps
4. User acceptance criteria
5. Rollout success criteria and monitoring metrics
```

---

### Step 8: Review and Validate
**Time: 15-30 minutes**

**Check immediately:**
- All requirements from the original product spec are addressed
- Architecture integrates properly with existing systems
- Interfaces are clearly defined and complete
- Edge cases and failure modes are documented

**Spot-check specifics:**
- Data models include all necessary fields and relationships
- API endpoints cover all required operations
- Error handling is defined for each integration point
- Performance targets are measurable and realistic

---

### Step 9: Refine and Iterate
**Time: 10-20 minutes**

Based on review, refine specific sections:

**Add missing details:**
```
The [SECTION NAME] section needs more detail on [SPECIFIC ASPECT]. Please expand to include [WHAT'S NEEDED].
```

**Clarify technical decisions:**
```
Explain why we chose [TECHNOLOGY/APPROACH] over [ALTERNATIVE], including trade-offs.
```

**Add diagrams:**
```
Create a [SEQUENCE/ARCHITECTURE/DATA FLOW] diagram showing [SPECIFIC INTERACTION OR COMPONENT].
```

**Address stakeholder concerns:**
```
How does this design address [SPECIFIC CONCERN LIKE SCALABILITY/SECURITY/COST]?
```

---

### Step 10: Export Final Specification
**Time: 2-5 minutes**

```
Compile all sections into a final technical specification document formatted for [CONFLUENCE/GOOGLE DOCS/MARKDOWN]. Include:
- Table of contents with section links
- Executive summary (1 paragraph)
- All technical sections developed above
- Open questions and items requiring decisions
- Approval sign-off section
```

---

## Example Output

Below is an abbreviated example of what a well-executed technical specification looks like:

---

> **TECHNICAL SPECIFICATION**
> **Real-Time Notification System**
>
> | Field | Value |
> |-------|-------|
> | Version | 1.0 |
> | Author | Engineering Team |
> | Status | Draft for Review |
> | Last Updated | January 2024 |
> | Reviewers | Engineering Lead, Product Manager, Security |
>
> ---
>
> ## 1. Overview
>
> ### 1.1 Background
> Users currently receive notifications via email only, which is slow and often ignored. This leads to missed mentions, delayed task responses, and poor user engagement.
>
> ### 1.2 Objective
> Implement a real-time notification system that delivers notifications within 2 seconds across web (push/in-app), iOS, and Android platforms, with user-configurable preferences.
>
> ### 1.3 Success Metrics
> - End-to-end latency (p95) < 2 seconds
> - Notification delivery rate > 99.5%
> - WebSocket connection stability > 99.9% uptime
>
> ---
>
> ## 2. Goals and Non-Goals
>
> **Goals:**
> - G1: Deliver notifications within 2 seconds of triggering event
> - G2: Support web push, mobile push, and in-app notifications
> - G3: Allow users to configure notification preferences per event type
>
> **Non-Goals:**
> - NG1: Email notification replacement (email remains for digest)
> - NG2: Rich media in notifications (text only for MVP)
> - NG3: Cross-device notification sync (read on one, read on all)
>
> ---
>
> ## 3. Architecture
>
> ### 3.1 High-Level Components
>
> | Component | Purpose | Technology |
> |-----------|---------|------------|
> | notification-service | Core notification logic, preferences, delivery orchestration | Python/FastAPI |
> | WebSocket Gateway | Real-time connection management | Go + Redis Pub/Sub |
> | Push Delivery Worker | Send push notifications via platform services | Python + AWS Pinpoint |
>
> ### 3.2 Technology Decisions
>
> | Decision | Choice | Rationale |
> |----------|--------|-----------|
> | WebSocket server | Go | Better concurrency model for many connections |
> | Push service | AWS Pinpoint | Managed service, already on AWS, unified API |
> | Connection state | Redis Cluster | Fast pub/sub, connection tracking |
>
> ---
>
> ## 4. Data Models
>
> ```sql
> CREATE TABLE notifications (
>     id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
>     user_id UUID NOT NULL REFERENCES users(id),
>     event_type VARCHAR(50) NOT NULL,
>     title VARCHAR(200) NOT NULL,
>     body TEXT,
>     target_url VARCHAR(500),
>     read_at TIMESTAMP,
>     created_at TIMESTAMP NOT NULL DEFAULT NOW(),
>     INDEX idx_notifications_user_created (user_id, created_at DESC)
> );
> ```
>
> ---
>
> ## 5. API Specification
>
> **Get Notifications**
> ```
> GET /api/v2/notifications
> Query Parameters: limit, before, unread_only
> ```
>
> **WebSocket Protocol**
> ```
> WSS://api.example.com/ws/notifications
> Authorization: Bearer <jwt_token>
> ```
>
> ---
>
> ## 6. Implementation Plan
>
> | Phase | Duration | Deliverables |
> |-------|----------|--------------|
> | Phase 1: Foundation | Week 1-2 | Database schema, notification-service skeleton |
> | Phase 2: WebSocket | Week 2-3 | WebSocket gateway, connection management |
> | Phase 3: Push | Week 3-4 | Pinpoint integration, device token management |
>
> ---
>
> ## 7. Testing Strategy
>
> - Unit tests for notification preference logic
> - Integration tests for end-to-end notification delivery
> - Load testing: 10K concurrent WebSocket connections per server
>
> ---
>
> ## 8. Security Considerations
>
> - WebSocket connections require valid JWT
> - Users can only receive their own notifications
> - No sensitive data in push notification payload
>
> ---
>
> ## 9. Monitoring and Alerting
>
> | Metric | Alert Threshold |
> |--------|-----------------|
> | Delivery latency (p95) | > 2s for 5 minutes |
> | Delivery rate | < 99% for 15 minutes |
> | Connection drop | > 20% drop in 5 minutes |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Spec is too vague, doesn't answer key questions | Started writing before requirements were clear | Run Step 3 thoroughly; clarify ambiguities before architecture |
| Spec has unnecessary detail that will become outdated | Trying to specify implementation instead of interfaces | Focus on contracts (APIs, data models); leave implementation flexible |
| Missing edge cases discovered during implementation | Didn't systematically consider failure modes | Add section on error handling, failure scenarios, edge cases |
| Stakeholders interpret spec differently | Assumptions not made explicit | Add Goals/Non-Goals section; be explicit about scope boundaries |
| Design doesn't integrate well with existing systems | Insufficient context about current architecture | Provide detailed system context in prompts; validate integration points |
| Spec is too technical for product stakeholders | Single document trying to serve all audiences | Create executive summary; use tables and diagrams for clarity |

---

## Tips from Experience

1. **Start with goals and non-goals.** Being explicit about what you're NOT building is as important as what you are. This prevents scope creep and misalignment.

2. **Define interfaces first, implementation second.** Contracts between components (APIs, events, data schemas) are what matter for coordination. Leave implementation details flexible.

3. **Use tables and diagrams liberally.** Technical prose is hard to parse. Tables comparing options, diagrams showing flow, and structured data models communicate faster.

4. **Document the "why" not just the "what."** Future readers need to understand decisions. Include alternatives considered and trade-offs made.

5. **Keep it iterative.** Don't try to write the perfect spec in one pass. Draft architecture, get feedback, refine. Specs improve through review cycles.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Implementation can begin without major unanswered questions
- [ ] Cross-team reviews identify only minor gaps or clarifications
- [ ] Stakeholders (engineering, product, business) all agree on scope and approach
- [ ] The spec serves as a reference during implementation, not shelf-ware
- [ ] Post-implementation, minimal rework was required due to misunderstanding

**Track over time:**
- Time from spec completion to implementation start (shorter is better)
- Number of clarifying questions during implementation (fewer is better)
- Scope changes after spec approval (fewer is better)

---

## Variations

### Variation 1: API Specification Document
When the primary deliverable is an API, focus on endpoint definitions:
```
Create a detailed API specification for [SERVICE NAME]:

Endpoints needed: [LIST OPERATIONS]
Data models: [DESCRIBE ENTITIES]
Authentication: [DESCRIBE AUTH APPROACH]

Include:
- OpenAPI/Swagger schema
- Request/response examples
- Error codes and handling
- Rate limiting and pagination
- Versioning strategy
```

### Variation 2: Database Design Document
For schema changes or new databases:
```
Design the database schema for [FEATURE]:

Entities: [LIST MAIN ENTITIES]
Relationships: [DESCRIBE RELATIONSHIPS]
Query patterns: [DESCRIBE HOW DATA WILL BE ACCESSED]

Include:
- Entity-relationship diagram
- Table definitions with indexes
- Migration strategy
- Data retention and archival
```

### Variation 3: Lightweight RFC for Smaller Changes
For changes that don't need full specs:
```
Create a lightweight RFC (Request for Comments) for [CHANGE]:

Problem: [DESCRIBE PROBLEM]
Proposed solution: [HIGH-LEVEL APPROACH]

Include:
- Brief problem statement
- Proposed approach
- Alternatives considered
- Open questions for discussion
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create specification templates.** Save prompts and document structures that work for your team. Customize for common scenarios (new features, API changes, data migrations).

2. **Integrate into development workflow.** Make specs a required step before major implementation. Link specs to implementation tickets. Review specs in design meetings.

3. **Build a specification library.** Archive completed specs as reference materials. New specs can build on patterns from previous successful projects.

4. **Establish review process.** Define who needs to approve specs (engineering lead, product, security). Set expectations for review turnaround time.

**Sample Folder Structure:**
```
technical-specs/
├── templates/
│   ├── full-feature-spec.md
│   ├── api-spec.md
│   └── database-design.md
├── 2024/
│   ├── notifications-system.md
│   ├── analytics-pipeline.md
│   └── user-auth-v2.md
└── archived/
    └── 2023/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**structured documentation that bridges business requirements and technical implementation**—applies broadly:

| Role | Application |
|------|-------------|
| **Product Managers** | Product requirement documents that clarify scope and success criteria |
| **Data Engineers** | Data pipeline specifications defining sources, transformations, and outputs |
| **DevOps Engineers** | Infrastructure specifications for deployment architecture and scaling |
| **Security Engineers** | Security design documents defining threat models and mitigations |
| **Technical Writers** | Documentation plans that structure complex information for different audiences |

---

## Next Steps

1. **This week:** Use this recipe for your next feature or system design. Start with a clear problem statement and iterate through the prompts.

2. **Track your results:** Note time saved vs. writing from scratch. Track questions during implementation (fewer questions = better spec).

3. **Iterate:** Customize prompts for your tech stack and team preferences. Add sections your organization requires (compliance, cost analysis).

4. **Share:** Show your team this approach. Collaborative spec writing with Claude can be done in real-time during design meetings.

---

*Recipe #96 of 100 in the Claude Code Knowledge Worker Recipe Collection*
