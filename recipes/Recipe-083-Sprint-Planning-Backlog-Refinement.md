# Sprint Planning and Backlog Refinement Support

**Recipe #83: From Vague Ideas to Sprint-Ready Stories**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 1-2 hours per sprint | Intermediate | Product Owners, Scrum Masters, Development Teams |

---

## The Problem

Sprint planning and backlog refinement are critical agile ceremonies that often feel inefficient. Stories arrive at planning poorly defined, estimates vary wildly, dependencies are discovered mid-sprint, and acceptance criteria are vague. Product owners spend hours refining stories that could be drafted faster, while teams spend meeting time asking basic clarifying questions that should have been answered beforehand.

**Pain Points:**
- Writing detailed acceptance criteria for every story takes significant prep time
- Identifying edge cases and error scenarios is often an afterthought
- Stories are sized inconsistently because complexity factors aren't articulated
- Dependencies between stories surface late, blocking sprint progress
- Large stories arrive at planning without being split into deliverable chunks
- Team spends 30+ minutes in planning just clarifying basic story details
- Refinement backlogs pile up because story prep is tedious and time-consuming

---

## The Outcome

Well-refined backlog items with clear acceptance criteria, estimated complexity, identified dependencies, and sprint-ready stories—enabling efficient sprint planning meetings that focus on strategy and commitment rather than basic story refinement.

**What You'll Have When Done:**
- User stories with comprehensive acceptance criteria in Given/When/Then format
- Complexity estimates with reasoning for each story
- Dependency map showing story-to-story and external dependencies
- Large epics decomposed into sprint-sized stories
- Edge cases and error scenarios documented before development
- Refinement output ready for team estimation and sprint planning

---

## When to Use This Recipe

**Good Fit:**
- Backlog refinement sessions requiring story prep work
- Sprint planning preparation to reduce meeting time
- Epic decomposition into deliverable user stories
- Story splitting when items are too large for a sprint
- Technical spike planning to reduce uncertainty
- Bug triage and refinement for better prioritization
- Release planning with multiple sprints of work
- Backlog cleanup to improve story quality

**Not a Good Fit:**
- Real-time refinement during team meetings (use for prep, not replacement)
- Stories where requirements are intentionally exploratory
- Tasks so small they don't benefit from structured acceptance criteria
- Emergency hotfixes requiring immediate action without planning

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have backlog items (epics, stories) to refine
- [ ] Product context and objectives are documented
- [ ] Technical constraints or architecture are known
- [ ] Team velocity and capacity data are available
- [ ] Definition of done is established
- [ ] Previous sprint learnings are captured
- [ ] You have 30-60 minutes for backlog refinement prep

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Drafting comprehensive acceptance criteria covering happy path, errors, and edge cases
- Identifying complexity factors and suggesting story point estimates
- Surfacing dependencies between stories and external systems
- Splitting large stories into smaller, valuable increments
- Organizing stories by theme, user type, or dependency order
- Generating refinement questions to clarify ambiguous requirements
- Creating consistent story format across the backlog

**Where Human Judgment Is Essential:**
- Final story point estimation based on team capacity and experience
- Prioritizing stories when tradeoffs must be made
- Assessing technical risk and implementation approach
- Validating that acceptance criteria match product vision
- Making scope decisions about what's in vs. out of sprint
- Facilitating team discussion during planning meetings

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| **Epic Description** | High-level feature with business context | Decomposing into user stories |
| **Team Context** | Velocity, estimation scale, capacity | Sizing stories appropriately |
| **Product Notes** | Stakeholder feedback, feature requests | Creating acceptance criteria |
| **Technical Constraints** | Architecture, existing systems, dependencies | Identifying risks and dependencies |
| **Definition of Done** | Team's quality standards | Ensuring stories are complete |

**Sample Input:**
```
EPIC: User Notification Preferences
Product: E-commerce mobile app
Description: Users should be able to manage their notification preferences
including push notifications, email, and SMS.

CONTEXT:
- Currently no notification preferences exist
- Users receive all notifications
- Complaints about too many notifications
- Marketing wants granular opt-in for campaigns
- Technical: Using Firebase for push, SendGrid for email, Twilio for SMS

TEAM INFO:
- Velocity: 32-38 points per sprint (2 weeks)
- Estimation scale: 1=hours, 2=1-2 days, 3=2-3 days, 5=3-5 days, 8=full sprint
- Available capacity this sprint: 34 points
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 5-10 minutes**

Gather backlog context:
- Copy epic or story descriptions needing refinement
- Document team velocity and estimation scale
- Note any known constraints or dependencies
- Include product context and user needs

**Tip:** Even incomplete information helps—Claude Code will identify gaps.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Story Refinement Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Epic Decomposition**

```
Claude, help me decompose this epic into sprint-sized user stories.

Epic:
[Paste epic description and context]

Our estimation scale:
[Paste estimation approach]

Please:
1. Break this epic into appropriately sized stories
2. Ensure each story delivers incremental value
3. Identify a logical sequence (what depends on what)
4. Flag any stories that need technical spikes
5. Suggest a minimum viable epic scope vs. full scope
```

---

### Step 4: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- Each story is independently valuable (not just technical tasks)
- Acceptance criteria are testable and specific
- Story sizes are appropriate for your sprint length
- Dependencies are clearly identified

**Spot-check specifics:**
- Do stories build on each other in the right order?
- Are any stories too vague to estimate?
- Is the MVP scope truly minimal and valuable?
- Do acceptance criteria cover edge cases?

---

### Step 5: Refine and Iterate
**Time: 20-30 minutes**

Use these follow-up prompts for deeper refinement:

**To refine individual stories:**
```
Help me refine this story for sprint planning:

Story: [TITLE]
Notes: [Paste available notes]
Open questions: [List known questions]

Please provide:
1. Refined story statement (As a... I want... So that...)
2. Complete acceptance criteria (Given/When/Then)
3. Edge cases to consider
4. Technical considerations
5. Dependencies (on other stories, systems, teams)
6. Estimated complexity (using our scale)
7. Questions that need answering before development
```

**To identify dependencies:**
```
Analyze dependencies for these stories:

Stories: [List stories]
System context: [Describe architecture/integrations]
Team structure: [Who's available]

Identify:
1. Story-to-story dependencies (sequence)
2. External system dependencies
3. Cross-team dependencies
4. Data dependencies
5. Infrastructure dependencies

Create a dependency map and flag any blockers.
```

**To split large stories:**
```
This story is too large (estimated [X]+ points). Help me split it.

Story: [TITLE and description]
Current acceptance criteria: [List]
Constraint: Each resulting story should be [Y] points or less

Provide:
1. Recommended split approach
2. Each resulting story with:
   - Story statement
   - Acceptance criteria
   - Estimated points
   - Value delivered
3. Dependencies between split stories
4. Suggested sequence
```

**To estimate complexity:**
```
Help estimate complexity for these stories:

[List stories with acceptance criteria]

Our estimation scale:
[Paste estimation scale]

For each story:
1. Recommended estimate (with reasoning)
2. Key complexity factors
3. Risk factors that could increase effort
4. Comparison to similar past work (if known)
5. Flag if story is too large and needs splitting
```

---

### Step 6: Export Final Output
**Time: 5 minutes**

```
Help me prepare for sprint planning:

Available capacity: [X] points
Backlog items (in priority order):
[List refined stories with estimates]

Sprint goal options:
[List potential themes/goals]

Please:
1. Recommend sprint goal
2. Suggest which stories to commit to
3. Identify risks to the sprint
4. Flag stories that need more refinement
5. Suggest placeholder for unplanned work
```

---

## Example Output

Below is an abbreviated example of what well-refined sprint planning materials look like:

---

> ### Epic Decomposition: User Notification Preferences
>
> ---
>
> #### Epic Overview
>
> **Epic:** User Notification Preferences
> **Total Estimated Points:** 42 points
> **Recommended Sprints:** 2 sprints (MVP in Sprint 1)
>
> ---
>
> #### Refined Stories
>
> ##### Story 1: Notification Preferences Backend Service
>
> **Story Statement:**
> As the system, I need a preferences service to store and retrieve user notification settings, so that preferences can be managed consistently across all channels.
>
> **Priority:** P1 (Foundation)
> **Estimate:** 8 points
> **Sprint:** 1
>
> **Acceptance Criteria:**
>
> | AC ID | Given | When | Then |
> |-------|-------|------|------|
> | AC-1.1 | A user exists | Preferences are requested | Return default preferences (all categories enabled except marketing, which defaults to disabled) |
> | AC-1.2 | A user has preferences | User updates a preference | Preference is saved with timestamp |
> | AC-1.3 | A preference is updated | Notification service queries preferences | Updated preference is returned |
>
> **Technical Notes:**
> - Create preferences table: user_id, channel, category, enabled, updated_at
> - REST API: GET /users/{id}/preferences, PUT /users/{id}/preferences
> - Add caching (Redis) for high-frequency reads
>
> **Dependencies:** None (foundation story)
>
> ---
>
> ##### Story 2: Push Notification Preferences UI (Mobile)
>
> **Story Statement:**
> As a mobile app user, I want to manage my push notification preferences by category, so that I only receive notifications I care about.
>
> **Priority:** P1
> **Estimate:** 5 points
> **Sprint:** 1
> **Depends on:** Story 1 (Backend Service)
>
> **Acceptance Criteria:**
>
> | AC ID | Given | When | Then |
> |-------|-------|------|------|
> | AC-2.1 | User opens notification settings | Screen loads | See toggles for: Order Updates, Shipping Alerts, Promotions, Price Drops, Back in Stock |
> | AC-2.2 | User views settings | Current state is displayed | Toggles reflect current preference state |
> | AC-2.3 | User toggles a preference | Toggle is changed | Preference updates in backend; confirmation shown |
>
> **Edge Cases:**
> - Device push notifications disabled at OS level → Show message to enable in settings
> - Marketing category toggled on → Show GDPR consent confirmation
> - Rapid toggle changes → Debounce API calls (500ms)
>
> **Dependencies:** Story 1 (Backend API must exist), Design mockups
>
> ---
>
> #### Sprint 1 Plan
>
> **Sprint Goal:** Enable users to manage push notification preferences with real-time sync
>
> **Committed Stories:**
>
> | Story | Points | Owner |
> |-------|--------|-------|
> | Story 1: Backend Service | 8 | Backend team |
> | Story 2: Push Notification UI | 5 | Mobile team |
> | Story 4: Sync and Caching | 5 | Mobile team |
> | Buffer for unplanned | 3 | - |
> | **Total** | **21** | |
>
> **Velocity:** 34 points available
> **Committed:** 21 points (62% capacity)
> **Rationale:** Conservative commitment due to technical risk of new service
>
> **Risks:**
> - Backend service may take longer than estimated (new service pattern)
> - Push notification category mapping needs design input
>
> **Blockers:**
> - Design mockups needed by Day 2
>
> ---
>
> #### Dependency Map
>
> ```
> [Story 1: Backend] ───┬────────────────────┐
>       │               │                    │
>       │               │                    │
>       ▼               ▼                    ▼
> [Story 2: Push]  [Story 4: Sync]   [Story 3: Email]
>       │               │                    │
>       └───────────────┼────────────────────┘
>                       │
>                       ▼
>              [Story 5: Migration]
> ```

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| **Stories keep growing during refinement** | Every discussion adds more requirements | Timebox refinement; use "parking lot" for future items; separate must-have from nice-to-have |
| **Estimates don't match actuals** | Team consistently over/under estimates | Use story point calibration sessions; compare to completed similar stories; track velocity trends |
| **Hidden dependencies emerge mid-sprint** | Work gets blocked by unknown dependencies | Explicitly map dependencies during refinement; involve all impacted teams; flag external dependencies early |
| **Acceptance criteria are ambiguous** | QA and dev interpret criteria differently | Use Given/When/Then format strictly; review criteria with QA during refinement; include edge cases explicitly |
| **Stories too large for sprint** | Epic wasn't decomposed enough | Split by user type, workflow step, or technical layer; ensure each delivers value; re-estimate pieces |
| **Team debates estimates endlessly** | Lack of shared understanding | Document complexity factors; use reference stories; timebox estimation discussion; accept ranges |

---

## Tips from Experience

1. **Refine ahead of planning.** Stories should be refined at least one sprint before they're planned. Don't wait until the planning meeting to start refinement.

2. **Keep stories small.** Nothing over 8 points in a 2-week sprint. If it's larger, split it. Smaller stories = better estimates and faster feedback.

3. **Include the team in refinement.** Developers should participate in backlog refinement, not just planning. Their input improves technical accuracy.

4. **Focus on "what" not "how."** Stories define the problem and acceptance criteria. Leave implementation details to developers during the sprint.

5. **Use real examples.** Concrete scenarios ("Given a user with 10 items in cart...") beat abstract criteria ("Support multiple items").

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Stories complete within sprint without carryover due to poor refinement
- [ ] Estimates are within 20% of actual effort
- [ ] No mid-sprint scope clarifications needed (criteria were clear)
- [ ] QA accepts stories on first pass (acceptance criteria were accurate)
- [ ] Sprint goals are achieved consistently

**Track over time:**
- Refinement prep time (should decrease as templates develop)
- Percentage of stories estimated accurately (within 20% of actual)
- Sprint planning meeting duration (should decrease with better prep)

---

## Variations

### Continuous Refinement for Kanban
**When to use:** Kanban teams without sprint boundaries

```
Create just-in-time refinement workflow:

- Refine stories as they near the top of backlog
- Keep 2 weeks of refined stories ready
- Use WIP limits to control refinement flow
- Focus on story clarity and dependencies
- Skip sprint-specific planning elements

Maintain flow-based metrics instead of velocity.
```

### Technical Story Refinement
**When to use:** Infrastructure, platform, or architecture work

```
Adapt story format for technical work:

- Use technical user stories (As a [system/API/service])
- Emphasize architecture decisions and technical debt reduction
- Include performance benchmarks and acceptance criteria
- Document integration points and API contracts
- Add technical spike stories for research/proof-of-concept

Focus on architectural impact, not just feature delivery.
```

### Bug Triage Refinement
**When to use:** Bug reports needing prioritization

```
Structure bug refinement:

For each bug:
- Severity (Critical/High/Medium/Low)
- Reproduction steps (Given/When/Then)
- Expected vs. actual behavior
- Affected users/frequency
- Workaround availability
- Estimated fix effort
- Root cause hypothesis

Prioritize by severity × frequency, not just severity alone.
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create story templates.** Build standard templates with required sections (story statement, acceptance criteria, dependencies, estimates). Store in wiki or backlog tool.

2. **Schedule regular refinement.** Book recurring refinement sessions (1-2 hours per sprint). Make refinement a habit, not a scramble before planning.

3. **Build estimation calibration data.** Document reference stories for each point value. Track actual vs. estimated effort. Use data to improve future estimates.

4. **Maintain an acceptance criteria library.** Archive well-written acceptance criteria patterns. Reuse patterns for similar stories (login, search, CRUD operations).

**Sample Folder Structure:**
```
backlog-refinement/
├── templates/
│   ├── user-story-template.md
│   ├── acceptance-criteria-checklist.md
│   └── dependency-map-template.md
├── reference-stories/
│   ├── 1-point-examples.md
│   ├── 2-point-examples.md
│   ├── 3-point-examples.md
│   └── 5-point-examples.md
├── current-sprint/
│   └── sprint-[N]-plan.md
└── refined-backlog/
    └── [epic-name]-stories.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming vague concepts into actionable, estimated work items**—applies broadly:

| Role | Application |
|------|-------------|
| **Product Teams** | Feature development and user story management |
| **Platform Teams** | Infrastructure work and technical debt stories |
| **Support Teams** | Bug triage and issue prioritization |
| **Data Teams** | Analytics requests and ML model development |
| **Marketing Teams** | Campaign planning and content creation tasks |

---

## Next Steps

1. **This week:** Select your next refinement session. Use this recipe to prep stories beforehand. Compare prep time and planning meeting efficiency.

2. **Track your results:** Measure refinement prep time, planning meeting duration, and story completion rates. Compare to baseline before using this approach.

3. **Iterate:** After 2-3 sprints, review which prompts worked best. Customize templates for your team's estimation scale and definition of done.

4. **Share:** Once refined stories are consistently sprint-ready, share your approach with other teams. Help your organization improve refinement quality.

---

*Recipe #83 of 100 in the Claude Code Knowledge Worker Recipe Collection*
