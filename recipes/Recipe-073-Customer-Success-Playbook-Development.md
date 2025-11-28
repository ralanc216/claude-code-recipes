# Customer Success Playbook Development

**Recipe #73: From Tribal Knowledge to Scalable Customer Success Processes**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 1-2 hours (first time) / 30 minutes (repeat) | 8-15 hours per playbook | Advanced | CS Leaders, CS Operations |

---

## The Problem

Customer success teams operate reactively when they lack standardized playbooks for common scenarios. Without documented best practices, responses to at-risk customers vary by CSM, onboarding quality is inconsistent, and expansion opportunities are missed.

**Pain Points:**
- Inconsistent customer experiences across different CSMs
- New CSMs take months to ramp up without documented processes
- Top performer knowledge stays trapped in their heads, not shared
- At-risk interventions happen too late or miss key steps
- No clear escalation paths when standard approaches fail
- Building comprehensive playbooks manually takes 8-15 hours per scenario
- Tribal knowledge scattered across team without centralization

## The Outcome

**What You'll Have When Done:**
- Comprehensive customer success playbook with clear trigger conditions
- Step-by-step action sequences with timing and ownership
- Communication templates for emails, calls, and escalations
- Decision trees for key branching points in the process
- Success metrics and leading indicators to track effectiveness
- FAQ and example cases for common scenarios
- Consistent, high-quality customer engagement across entire CS team
- Faster CSM onboarding with documented best practices

## When to Use This Recipe

**Good Fit:**
- Building CS operations from scratch or formalizing ad-hoc practices
- Standardizing inconsistent practices across team
- Onboarding new CSMs quickly during rapid team scaling
- Improving customer health management systematically
- Reducing churn through proactive intervention processes
- Systematizing expansion/upsell motions that currently vary by rep
- After identifying best practices from top performers to codify
- When audit or leadership requires documented procedures

**Not a Good Fit:**
- Very small CS team (1-2 people) where flexibility is more important
- Scenarios that truly require case-by-case judgment with no patterns
- When you haven't yet identified what works (need to experiment first)
- If team culture strongly resists process documentation

## Before You Start: Quick Checklist

- [ ] Customer journey stages clearly defined
- [ ] Health score metrics and thresholds established
- [ ] Common customer scenarios identified and prioritized
- [ ] Best practices documented from top-performing CSMs
- [ ] Communication templates that have proven effective
- [ ] Escalation paths and roles clearly defined
- [ ] Tools and systems CSMs use documented
- [ ] Time allocated for thorough playbook development

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforming unstructured CSM knowledge into structured playbooks
- Creating comprehensive documentation including triggers, actions, templates, metrics
- Developing decision trees and flowcharts from described scenarios
- Generating communication templates with appropriate tone and personalization
- Ensuring playbook completeness by identifying gaps in provided information
- Structuring complex multi-step processes into clear, actionable sequences
- Creating consistent formatting across multiple playbooks
- Drafting talk tracks and email templates for different scenarios

**Where Human Judgment Is Essential:**
- Validating that playbook steps match reality of customer interactions
- Determining appropriate escalation thresholds based on company culture
- Assessing which templates feel authentic vs. too scripted
- Understanding nuances of different customer segments requiring variations
- Deciding on metrics and success criteria that matter for your business
- Testing playbook with real CSMs to ensure usability
- Adjusting based on team feedback and actual usage patterns

## Input Examples

| Input Type | What to Include | Example |
|------------|-----------------|---------|
| Playbook Context | Scenario description, current state, goals, health score components | At-Risk Customer Intervention: Health score drops below 60 or declining 3 weeks. Goal: 70%+ save rate within 48 hours |
| Best Practices | Top performer approaches, common tactics, what works | "I never wait more than a day. First I pull usage data to identify what changed. Then reach out with specific hypothesis, not generic check-in." |
| Available Resources | Tools, team structure, communication channels, constraints | ChurnZero for health, CRM, 8 CSMs carrying 50-60 accounts each, limited executive time |

### Sample Input (Best Practices from Top CSMs):
```
TOP CSM PRACTICES (from interviews):

Maria (top performer - 85% save rate):
"I never wait more than a day when health drops. First thing I do
is pull usage data and try to identify what changed. Is it a champion
leaving? A specific feature they stopped using? Then I reach out with
a specific hypothesis, not a generic 'how are things going' call.

For example: 'I noticed your team's usage of the reporting module
dropped 40% this month. I wanted to check in - did something change
with your reporting needs, or is there a blocker I can help with?'

If I can't figure out the root cause from data, I call the champion
immediately. If champion isn't responding, I find another contact
or escalate internally to get executive outreach."

James (second highest - 78% save rate):
"The key is treating it like triage. Not all at-risk accounts are
equal. I categorize into:
- Fixable (product issue, training need) - I can handle
- Relationship (champion left, exec misalignment) - need exec help
- Value (they're not seeing ROI) - need business case work
- Lost cause (they've already decided) - focus elsewhere

I also loop in my manager early on high-value accounts. Too many
CSMs wait until it's too late to escalate."
```

## Step-by-Step Implementation

### Step 1: Define Playbook Scope (15 minutes)
```
Claude, I'm building a customer success playbook for [scenario].

Context:
- Scenario description: [What triggers this playbook]
- Current state: [How it's handled today]
- Goal: [What success looks like]

Best practices we know work:
[Paste top performer insights]

Please help me structure a comprehensive playbook. Start by:
1. Confirming the trigger conditions
2. Identifying the key phases of intervention
3. Outlining what the playbook should cover
4. Flagging any additional information you need
```

### Step 2: Build Trigger Framework (15 minutes)
```
Help me define precise trigger conditions for this playbook.

Health score components: [List components and weights]
Data available: [What signals we can detect]

Create:
1. PRIMARY TRIGGERS (automatic playbook activation)
2. SECONDARY TRIGGERS (CSM judgment required)
3. SEVERITY LEVELS (determines response urgency)
4. EXCLUSIONS (when NOT to trigger)

For each trigger, specify:
- Exact threshold or condition
- Data source
- Detection timing (real-time, daily, weekly)
```

### Step 3: Develop Action Sequence (20 minutes)
```
Now create the step-by-step action sequence for this playbook.

For each step, include:
- Action description
- Owner (CSM, Manager, Executive)
- Timing (when relative to trigger)
- Inputs needed
- Outputs/deliverables
- Decision points
- Escalation triggers

Consider:
- Different severity levels
- Enterprise vs. mid-market variations
- Available resources and tools
- Time constraints of CSMs
```

### Step 4: Create Communication Templates (20 minutes)
```
Create communication templates for each stage of the playbook.

For each template, include:
- When to use (trigger/context)
- Subject line (if email)
- Message body with personalization placeholders
- Call-to-action
- Follow-up timing if no response
- Talk track alternative (for calls)

Templates needed:
1. Initial outreach
2. Follow-up if no response
3. Escalation request (internal)
4. Executive outreach
5. Recovery confirmation
6. If save unsuccessful
```

### Step 5: Define Success Metrics (15 minutes)
```
Define how we'll measure this playbook's effectiveness.

Include:
1. PROCESS METRICS
   - Compliance measures (is the playbook being followed?)
   - Timing measures (intervention speed)

2. OUTCOME METRICS
   - Save rate (accounts recovered)
   - Time to recovery
   - Health score improvement

3. LEADING INDICATORS
   - Early signals the intervention is working
   - Warning signs it's not working

4. BENCHMARKS
   - Current baseline
   - Target performance
   - Top performer comparison
```

### Step 6: Add Decision Trees (15 minutes)
```
Create decision trees for key branching points in the playbook.

For each major decision point:
- Question to answer
- Options/paths
- Criteria for each path
- Actions for each path

Decision points to address:
1. Root cause categorization
2. Escalation decisions
3. When to increase/decrease intervention intensity
4. When to consider account "saved" vs. ongoing risk
5. When to stop intervention efforts
```

## Example Output

> **Customer Success Playbook: At-Risk Customer Intervention**
>
> **Purpose:** Standardized approach to identifying, engaging, and recovering at-risk customers before they churn.
>
> **Scope:** All customers whose health score drops below 60 or shows declining trend for 3+ consecutive weeks.
>
> **Goals:** 70%+ save rate, intervention within 48 hours, clear escalation paths
>
> **Trigger Framework:**
> - PRIMARY: Health score < 60, 3 consecutive weekly declines, >40% usage drop, champion departure, NPS detractor (0-6)
> - SEVERITY LEVELS: Critical (<4 hours), High (24 hours), Medium (48 hours), Monitoring (1 week)
>
> **Action Sequence:**
> Phase 1 (Hours 0-4): Detection, data pull, severity assignment, root cause hypothesis, manager notification
> Phase 2 (Hours 4-48): Personalized outreach with specific hypothesis, phone attempt if Critical/High
> Phase 3 (Days 2-10): Diagnostic conversation, confirm root cause, develop recovery plan, present to customer
> Phase 4 (Days 10-30): Execute recovery actions, weekly check-ins, track progress, adjust plan
> Phase 5 (Day 30+): Confirm recovery criteria met, lessons learned, ongoing monitoring
>
> **Success Metrics:** Save rate >70%, first response <24 hours, playbook compliance >90%, repeat at-risk <15%

## Troubleshooting Common Issues

| Issue | Symptoms | Solution |
|-------|----------|----------|
| Playbook too complex for new CSMs | New team members overwhelmed, low adoption | Create "quick start" version with essential steps only; pair new CSMs with senior CSM for first interventions; build training module |
| CSMs not following playbook | Low playbook compliance despite documentation | Understand barriers (time, disagreement, awareness); simplify where possible; automate in CRM/tools; include in performance reviews |
| Templates feel generic | Customers receiving similar-sounding outreach | Encourage personalization of templates; update quarterly based on what works; create segment-specific variations |
| Escalations overwhelming leadership | Too many accounts escalated to managers/execs | Refine escalation criteria; add peer escalation tier (Senior CSM); provide more CSM training on difficult scenarios |

## Tips from Experience

1. **Start with one playbook and perfect it** - Don't try to document everything at once. Build your first playbook, test it, iterate based on feedback, then expand to other scenarios. Perfect one before creating five mediocre ones.

2. **Test with top performers first** - Get buy-in and feedback from your best CSMs before rolling out broadly. They'll identify gaps and ensure the playbook captures what actually works, not just theory.

3. **Make it accessible where CSMs work** - Store playbooks in your CRM, knowledge base, or wherever CSMs spend their time. The best playbook is useless if it takes three clicks and a search to find.

4. **Update regularly based on reality** - Playbooks get stale as your product, customers, and market evolve. Schedule quarterly reviews to update based on what's working and what's changed.

5. **Allow flexibility, not rigid rules** - Playbooks should be guidelines that improve consistency while still allowing CSM judgment. The goal is better outcomes, not robotic adherence to steps.

## Measuring Success

**Process Completion:**
- [ ] Playbook includes all core sections (triggers, actions, templates, metrics, decision trees)
- [ ] Tested with 2-3 CSMs before broad rollout
- [ ] Templates are personalization-ready, not generic scripts
- [ ] Decision trees cover key branching points
- [ ] Success metrics defined with baseline and targets
- [ ] FAQ addresses common CSM questions

**Tracking Metrics:**
- Save rate improvement after playbook implementation (target: match top performer rates)
- Time to first intervention reduction (target: <24 hours for all severity levels)
- Playbook compliance rate (target: >90% of triggered cases)
- Consistency across CSMs measured by variance in save rates (target: reduce variance by 50%)
- CSM satisfaction with playbook usability (survey: >4/5)
- Customer feedback on support experience during interventions

## Variations

### Variation 1: Onboarding Success Playbook
**Prompt:** "Create a playbook for guiding new customers from contract signature through implementation to first value milestone. Include kickoff meeting template, weekly check-in cadence, common blockers decision tree, and go-live criteria."

### Variation 2: Expansion Playbook
**Prompt:** "Build a systematic playbook for identifying and executing upsell/cross-sell opportunities. Include signals that indicate expansion readiness, qualification questions, business case template, and timing considerations for different expansion types."

### Variation 3: Executive Business Review Playbook
**Prompt:** "Develop a playbook for conducting strategic quarterly business reviews with customer executives. Include preparation checklist, presentation template, discussion guide, and follow-up action plan framework."

## Building Your Repeatable System

**1. Templates to Create:**
- Playbook template with standard structure for all CS playbooks
- Decision tree template with consistent format for branching logic
- Communication template library organized by scenario and stage
- Case study template to document successful interventions

**2. Process Integration:**
- Link playbook triggers to automated alerts in CS platform
- Embed communication templates in CRM/email tools for one-click access
- Build playbook steps into customer success platform workflows
- Include playbook metrics in team dashboards and reporting

**3. Training and Adoption:**
- Create onboarding module teaching new CSMs how to use playbooks
- Run workshops on complex playbooks with role-playing exercises
- Celebrate successful playbook usage in team meetings
- Include playbook compliance in performance discussions

**4. Knowledge Repository Structure:**
```
/cs-playbooks/
  /at-risk-intervention/
    playbook-v2.1.md
    templates/
      initial-outreach.txt
      follow-up.txt
      escalation-request.txt
    decision-trees/
      root-cause-categorization.png
      escalation-decision.png
    examples/
      successful-recovery-case-1.md
      successful-recovery-case-2.md
  /onboarding/
    playbook-v1.3.md
    templates/
    decision-trees/
  /expansion/
    playbook-v1.0.md
  /playbook-metrics-dashboard.md
```

## How This Pattern Applies Elsewhere

| Role/Function | Application | Example Use Case |
|---------------|-------------|------------------|
| Sales | Discovery, demo, negotiation playbooks | Standardize discovery call approach with question frameworks, objection handling, and qualification criteria |
| Support | Escalation, outage response playbooks | Define when and how to escalate issues, communication templates for customers during outages, resolution workflows |
| HR | Onboarding, offboarding playbooks | Consistent new hire experience with checklists, communication templates, and milestone tracking |
| Product | Feature launch, beta program playbooks | Standardized approach to launching features with stakeholder communication, training materials, feedback collection |
| Operations | Crisis response, incident management | Standard operating procedures for different incident types with clear roles, escalation paths, communication plans |

## Next Steps

1. **Pilot with subset of team** - Test playbook with 2-3 CSMs for 2-4 weeks before full rollout

2. **Gather structured feedback** - Survey pilots on what works, what doesn't, what's missing; observe actual usage patterns

3. **Refine based on results** - Adjust triggers, simplify steps, improve templates based on pilot feedback

4. **Train entire team** - Workshop format teaching the "why" behind playbook, not just documentation share

*Recipe #73 of 100 in the Claude Code Knowledge Worker Recipe Collection*
