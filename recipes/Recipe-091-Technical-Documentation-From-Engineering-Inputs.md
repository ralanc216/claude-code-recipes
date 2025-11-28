# Technical Documentation from Engineering Inputs

**Recipe #91: From Scattered Engineering Artifacts to Comprehensive Technical Documentation**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 3-5 hours per document | Intermediate | Technical Writers, Engineers, DevOps, System Administrators |

---

## The Problem

Engineers build systems but documentation lags months behind—or never happens at all. When documentation does exist, it's often outdated, inconsistent, or written in a style that only the original author understands. Critical knowledge lives in code comments, Slack messages, or people's heads. When those people leave, the knowledge leaves with them.

**Pain Points:**
- Documentation becomes outdated within weeks of system changes
- Knowledge scattered across code comments, Slack threads, and email
- New team members take months to understand system architecture
- Incident response slowed by lack of operational documentation
- Only the original engineer knows why critical decisions were made
- Support tickets pile up because procedures aren't documented
- Compliance audits reveal documentation gaps

---

## The Outcome

Clear, comprehensive technical documentation that captures system architecture, operational procedures, and engineering decisions—written in a consistent style that serves both current team members and future maintainers.

**What You'll Have When Done:**
- Complete system architecture documentation with diagrams and flows
- Configuration reference guides for all services
- Operational runbooks for common scenarios
- Troubleshooting procedures based on real incidents
- Cross-referenced documentation with consistent terminology
- Up-to-date technical specs that reflect current implementation

---

## When to Use This Recipe

**Good Fit:**
- System architecture documentation
- Runbook and playbook creation
- Operational procedure documentation
- Internal developer guides
- Infrastructure documentation
- Deployment documentation
- Troubleshooting guides
- Configuration references

**Not a Good Fit:**
- Marketing or sales documentation (too technical)
- User-facing help content (needs different approach)
- Real-time API documentation (requires automation)
- Documentation requiring legal review

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Code repositories/source files accessible
- [ ] Architecture diagrams (if available) gathered
- [ ] Configuration files collected
- [ ] Engineer interviews or notes scheduled
- [ ] Existing documentation (however outdated) located
- [ ] Slack/email threads with context saved
- [ ] Incident postmortems collected
- [ ] Target audience defined
- [ ] You have 30-60 minutes for documentation creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforms scattered engineering artifacts into structured documentation
- Maintains technical accuracy while improving readability
- Identifies gaps in documentation coverage
- Creates consistent documentation following best practices
- Generates configuration reference tables from raw config files
- Extracts operational procedures from incident reports
- Cross-references sections and maintains terminology consistency

**Where Human Judgment Is Essential:**
- Validating technical accuracy with system owners
- Determining appropriate detail level for audience
- Identifying sensitive information requiring redaction
- Prioritizing which systems need documentation first
- Deciding documentation maintenance schedule

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Architecture notes | Meeting notes, design docs | System overview and component relationships |
| Configuration files | YAML, JSON, properties files | Configuration reference tables and validation |
| Slack/email threads | Team discussions about decisions | Context for "why" decisions were made |
| Incident reports | Postmortems, RCA documents | Troubleshooting procedures and monitoring guidance |
| Code repositories | README files, code comments | Technical implementation details |

**Sample Input:** *(Architecture meeting notes)*
```
SYSTEM: Order Processing Pipeline

"So basically orders come in through the API gateway, hit the order-service
which validates them, then we put them on Kafka. The processor picks them
up, does fraud checks, inventory checks, payment auth, and if all good,
creates fulfillment requests. If anything fails we have DLQs and a retry
mechanism. Payment is tricky - we do auth at order time but capture only
when shipped.

The whole thing runs on K8s in us-east-1 and us-west-2, failover is automatic
through Route53 health checks. DB is Aurora with read replicas..."
```

---

## Step-by-Step Implementation

### Step 1: Gather and Inventory Inputs
**Time: 10-15 minutes**

Collect all available documentation artifacts:
- Clone relevant code repositories
- Export Slack threads about system decisions
- Gather configuration files from production/staging
- Collect incident reports and postmortems
- Screenshot architecture diagrams if they exist

Launch Claude Code in your documentation directory.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Documentation Analysis Prompt
**Time: 15-20 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze Engineering Inputs for Documentation**

```
Claude, I need to create technical documentation from engineering inputs.

System: [System Name]
Purpose: [What it does]

Here's what I have:
- Architecture notes: [Paste or describe]
- Configuration files: [Paste]
- Relevant Slack/email threads: [Paste]
- Incident reports: [Paste]
- Existing docs (even if outdated): [Reference]

Help me:
1. Inventory what information we have
2. Identify gaps in documentation
3. Create an outline for comprehensive docs
4. List questions I need to ask engineers
```

---

### Step 4: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- Does the outline cover all critical system components?
- Are the identified gaps accurate?
- Do the suggested questions make sense for the engineers?

**Spot-check specifics:**
- Technical terminology usage is correct
- Component names match your actual systems
- No sensitive credentials or secrets in examples

---

### Step 5: Generate Documentation Sections
**Time: 20-30 minutes**

Use follow-up prompts to create each section:

**For Architecture Overview:**
```
Write an architecture overview based on these inputs:

System context: [Paste notes]
Configuration details: [Paste config]

Create:
1. High-level system description (1-2 paragraphs)
2. Component diagram description (for diagramming later)
3. Data flow explanation
4. Integration points with other systems
5. Technology stack summary

Write for an audience of: [senior engineers / junior devs / ops team]
```

**For Configuration Documentation:**
```
Document this configuration for operational use:

Config file: [Paste]
Context: [What it's for]

Create:
1. Configuration reference table (parameter, type, description, default)
2. Environment variable requirements
3. Common configuration scenarios
4. Validation and constraints
5. Examples for different environments
```

**For Operational Procedures:**
```
Create runbook procedures from this incident and Slack context:

Incident details: [Paste]
Context from team: [Paste Slack]

Write procedures for:
1. Monitoring and alerting (what to watch)
2. Common issues and troubleshooting steps
3. Escalation procedures
4. Temporary overrides and their process
5. Rollback procedures if applicable
```

---

### Step 6: Assemble and Finalize
**Time: 10-15 minutes**

```
Compile the documentation sections into a cohesive document:

Sections:
- Architecture overview: [Paste]
- Configuration reference: [Paste]
- Operational procedures: [Paste]

Please:
1. Ensure consistent terminology throughout
2. Add cross-references between sections
3. Create table of contents
4. Add "last updated" and version info
5. Identify any remaining gaps to be filled
```

---

### Step 7: Export Final Output
**Time: 2 minutes**

```
Save this documentation in Markdown format suitable for our documentation system [GitHub Pages / Confluence / GitBook / etc.]. Include appropriate frontmatter and formatting for [platform].
```

---

## Example Output

Below is an abbreviated example of what well-executed technical documentation looks like:

---

> **Order Processing Pipeline**
> **Technical Documentation**
> *Version 1.0 | Last Updated: October 2024*
>
> ---
>
> #### Overview
>
> The Order Processing Pipeline handles all customer order workflows from initial submission through fulfillment request creation. It validates orders, performs fraud screening, checks inventory availability, authorizes payments, and coordinates with fulfillment systems.
>
> **Scope:** This document covers system architecture, configuration parameters, operational procedures, and troubleshooting.
>
> **Audience:** Platform engineers, SRE team, on-call rotation
>
> ---
>
> #### Architecture
>
> The Order Processing Pipeline is a distributed, event-driven system built on microservices architecture...
>
> **Technology Stack:**
>
> | Component | Technology | Version |
> |-----------|------------|---------|
> | API Gateway | Kong | 3.4 |
> | Order Service | Go | 1.21 |
> | Message Queue | Apache Kafka | 3.5 |
> | Database | Aurora PostgreSQL | 15.4 |
>
> ---
>
> #### Configuration Reference
>
> | Parameter | Type | Description | Default | Required |
> |-----------|------|-------------|---------|----------|
> | `service.port` | integer | HTTP listener port | 8080 | Yes |
> | `database.pool_size` | integer | Connection pool size | 20 | No |
> | `rate_limits.concurrent_orders_per_merchant` | integer | Per-merchant limit | 50 | No |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Missing "why" information | Engineers didn't document decisions | Schedule 30-min interviews; ask "why" questions; review git blame for context |
| Documentation too technical | Written for engineers, not operators | Create layered docs—overview for leadership, details for operators |
| Outdated within weeks | System evolved but docs didn't | Version docs with code; include "last updated" date; schedule quarterly reviews |
| Can't find when needed | Poor discoverability | Create central index; use consistent naming; link from code READMEs |
| Inconsistent terminology | Multiple authors, no standard | Use glossary; establish style guide; have single reviewer for consistency |
| Too high-level or too detailed | Wrong audience assumed | Define audience upfront; test with newcomers; create multiple views if needed |

---

## Tips from Experience

1. **Start with questions.** Ask "What would someone need to know to operate this system?" Let that guide your documentation structure.

2. **Interview multiple people.** Different engineers have different perspectives. The person who built it and the person who maintains it see different things.

3. **Use actual incidents.** Postmortems reveal what really matters operationally. They show you what to monitor, what breaks, and how to fix it.

4. **Include the "why."** Context prevents future mistakes. Document not just what the configuration is, but why it was set that way.

5. **Make it scannable.** Use tables, headers, and bullet points over long paragraphs. Engineers skim documentation while troubleshooting at 2am.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] New engineers can understand the system without extensive hand-holding
- [ ] On-call engineers can troubleshoot using the documentation
- [ ] Incidents caused by documentation gaps have decreased
- [ ] Documentation is referenced in tickets and Slack conversations
- [ ] Engineers update docs when they make changes

**Track over time:**
- Time for new engineer to become productive with the system
- Number of incidents caused by documentation gaps or outdated info
- Documentation usage metrics (if your platform tracks views)

---

## Variations

### System Architecture Focus
**When to use:** Initial documentation for a new system
```
Focus the documentation on architecture and design decisions. Include:
- Component interaction diagrams
- Data flow diagrams
- Technology choice rationale
- Scalability considerations
- Security architecture
```

### Operational Runbook Focus
**When to use:** System is documented but ops procedures are missing
```
Emphasis on operational procedures with step-by-step instructions:
- Standard operating procedures
- Troubleshooting decision trees
- Escalation paths
- Monitoring and alerting setup
- Common maintenance tasks
```

### Architecture Decision Records (ADRs)
**When to use:** Need to document "why" decisions were made
```
Document architectural decisions in ADR format:
- Context: What problem are we solving?
- Decision: What did we decide?
- Alternatives considered
- Consequences and trade-offs
- Status: Proposed, Accepted, Deprecated
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create documentation templates** for common system types (microservices, databases, infrastructure). This ensures consistency and speeds up future documentation.

2. **Establish a documentation review process** where technical docs are reviewed before merge, just like code. Assign documentation owners for each major system.

3. **Integrate with change management** so documentation updates are part of the deployment checklist. No deployment without updated docs.

4. **Set up regular review cycles** (quarterly) for each system's documentation. Assign this to the on-call rotation or system owners.

**Sample Folder Structure:**
```
docs/
├── architecture/
│   ├── system-overview.md
│   ├── component-diagrams/
│   └── data-flows/
├── operations/
│   ├── runbooks/
│   ├── troubleshooting/
│   └── monitoring/
├── configuration/
│   ├── service-configs/
│   └── environment-variables/
└── decisions/
    └── ADRs/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming scattered technical information into structured documentation**—applies broadly:

| Role | Application |
|------|-------------|
| **Infrastructure Teams** | Network diagrams, data center documentation, disaster recovery plans |
| **Security Teams** | Security architecture docs, incident response procedures, compliance documentation |
| **Data Engineering** | Data pipeline documentation, schema documentation, ETL process guides |
| **DevOps** | CI/CD pipeline docs, deployment procedures, infrastructure-as-code documentation |
| **Support Teams** | Internal knowledge bases, escalation procedures, system integration guides |

---

## Next Steps

1. **This week:** Document your most critical system (the one that causes pain when it breaks and only one person understands).

2. **Track your results:** Note how long it takes new team members to get productive with documented vs. undocumented systems.

3. **Iterate:** After your first incident using the new documentation, update it with what you learned.

4. **Share:** Make documentation the single source of truth. Link to it in Slack answers, ticket resolutions, and code comments.

---

*Recipe #91 of 100 in the Claude Code Knowledge Worker Recipe Collection*
