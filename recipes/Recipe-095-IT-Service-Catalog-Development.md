# IT Service Catalog Development

**Recipe #95: From Scattered IT Services to Organized Self-Service Catalog**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 30 minutes (first time) / 15 minutes (repeat) | 8-12 hours per catalog section | Intermediate | IT Service Management, IT Operations, CIOs |

---

## The Problem

IT departments provide dozens of services, but employees don't know what's available, how to request it, or what to expect. This leads to shadow IT (people finding their own solutions), repeated questions to IT staff, inconsistent service delivery, and difficulty measuring IT value. A service catalog should answer "what can IT do for me?" but most are either nonexistent, incomplete, or too technical to be useful.

**Pain Points:**
- Employees don't know what IT services are available
- Requests come through informal channels (email, walk-ups, Slack DMs)
- No standardized request process leads to inconsistent delivery
- Service levels undefined, creating mismatched expectations
- IT can't measure demand or demonstrate value
- Shadow IT proliferates because official process is unclear
- Same questions answered repeatedly by different IT staff

---

## The Outcome

A comprehensive, user-friendly IT service catalog that clearly defines available services, request processes, service levels, and costs—enabling employees to self-serve and IT to manage demand effectively.

**What You'll Have When Done:**
- User-facing catalog with clear service descriptions in plain language
- Standardized request processes for each service
- Defined service level expectations (response and resolution times)
- Cost transparency for chargebacks or budgeting
- IT-facing fulfillment procedures and support documentation
- Measurable service delivery metrics

---

## When to Use This Recipe

**Good Fit:**
- Building first IT service catalog
- Modernizing legacy IT documentation
- ITIL/ITSM implementation projects
- IT department reorganization
- Cloud migration service catalog updates
- Annual IT portfolio review and cleanup

**Not a Good Fit:**
- Customer-facing external services (different audience)
- Highly specialized one-off requests (not catalogable)
- Emergency incident management (different workflow)
- Services still in pilot or experimental phase

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] List of IT services currently provided compiled
- [ ] Service ownership information identified
- [ ] Current request processes documented (formal and informal)
- [ ] SLA definitions or targets established
- [ ] Cost/chargeback information gathered (if applicable)
- [ ] User feedback on current services collected
- [ ] Service dependencies mapped
- [ ] Support tier definitions clear
- [ ] You have 60-90 minutes for catalog development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforms scattered IT service information into structured catalog entries
- Ensures consistent format across all service descriptions
- Generates user-friendly descriptions from technical specifications
- Creates appropriate documentation for both end-users and IT staff
- Identifies service bundles and logical groupings
- Extracts request workflows from existing processes
- Maps service levels to business expectations

**Where Human Judgment Is Essential:**
- Validating service ownership and accountability
- Setting realistic SLAs based on capacity
- Determining appropriate pricing or chargebacks
- Prioritizing which services to catalog first
- Deciding service eligibility and approval workflows
- Reviewing for compliance with organizational policies

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Service inventory | List of services IT provides | Service catalog structure and categorization |
| Service details | How services work, requirements, limitations | User-facing and IT-facing documentation |
| Current processes | Email threads, procedures, tribal knowledge | Request workflows and fulfillment steps |
| User feedback | Common questions, pain points | FAQ sections and troubleshooting |
| Organizational context | Approval hierarchies, cost structure | Workflow design and pricing information |

**Sample Input:** *(Service details)*
```
SERVICE: VPN Access

Current process:
- Manager submits request via email to it-helpdesk@
- IT verifies employee status
- IT installs VPN client on next available date
- User gets credentials via encrypted email
- No formal SLA, usually 2-3 days

Requirements:
- Company-issued laptop with endpoint security
- Manager approval for employees
- Security approval for contractors

Known Issues:
- Users forget to connect, can't access resources
- Mac users report connectivity drops
- License limit causes issues during major events
```

---

## Step-by-Step Implementation

### Step 1: Inventory and Categorize Services
**Time: 15-20 minutes**

Gather your service information:
- List all services IT currently provides (formal and informal)
- Identify service owners for each
- Document current request methods (even if informal)
- Collect any existing documentation
- List known pain points or frequent questions

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Service Analysis Prompt
**Time: 15-20 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze IT Services**

```
Claude, I need to build an IT service catalog.

Here's our service inventory:
[Paste list of services by category: Infrastructure, End User Computing, Applications, Security, Support]

Help me:
1. Group services into logical categories for end users (not IT's internal structure)
2. Identify which services need individual entries vs service bundles
3. Suggest user-friendly service names (not technical jargon)
4. Note dependencies between services
5. Identify which services are highest priority for cataloging (by request volume or business impact)
```

---

### Step 4: Review and Validate
**Time: 10 minutes**

**Check immediately:**
- Categories make sense from user perspective, not IT organization chart
- Service names are clear without IT jargon
- Priority aligns with business needs and request volume

**Spot-check specifics:**
- Service bundles are logical (e.g., "New Employee Setup" vs separate services)
- Dependencies are identified correctly
- No duplicate or overlapping services

---

### Step 5: Define Service Levels
**Time: 20 minutes**

```
Define service levels for these IT services:

Services: [List from analysis]
Current reality: [What actually happens today - response times, fulfillment times]
Desired state: [Goals for improvement]
Capacity constraints: [Team size, licenses, budget]

For each service, recommend:
1. Response time target (acknowledgment of request)
2. Resolution time target (service delivered)
3. Service hours (24/7, business hours, specific availability)
4. Availability target (uptime percentage if applicable)
5. Escalation path for exceptions or issues
```

---

### Step 6: Create User-Facing Catalog Entries
**Time: 20-30 minutes per service**

**For each priority service:**
```
Write a user-facing service catalog entry:

Service: [Name, e.g., "VPN Access for Remote Work"]
Technical details: [Paste internal info about how it works]
Target audience: [Who can request this - all employees, specific roles, etc.]
Current process: [How it works today]

Create:
1. Clear, user-friendly service name and subtitle
2. Plain-language description (2-3 sentences) - what it is and why you'd need it
3. Who can request (eligibility criteria)
4. What's included (bullet points of what you get)
5. What's NOT included (common misconceptions or out-of-scope items)
6. How to request (step by step)
7. Service levels (when you'll get it, support hours)
8. Cost (if applicable, or "No charge to your department")
9. FAQ section (common questions from users)
10. Related services
```

---

### Step 7: Create IT-Facing Documentation
**Time: 15-20 minutes per service**

```
Create internal IT documentation for this service:

User-facing entry: [Paste from previous step]
Technical details: [How it actually works, tools, dependencies]
Service owner: [Who owns this service]

Include:
1. Technical architecture overview (what systems are involved)
2. Fulfillment procedures (step-by-step for IT staff)
3. Support procedures by tier (Tier 1, 2, 3 responsibilities)
4. Known issues and workarounds
5. Escalation contacts and when to escalate
6. Dependencies and integrations with other services
7. Capacity and licensing constraints
8. Tools and access required to fulfill service
```

---

### Step 8: Assemble Complete Catalog
**Time: 15 minutes**

```
Compile the IT service catalog for publication:

Platform: [ServiceNow / Confluence / SharePoint / Custom portal]

Structure:
- User-facing catalog with all service entries
- Category organization and navigation
- Search functionality keywords
- Request submission integration
- My Requests tracking portal

Please:
1. Ensure consistent formatting across all services
2. Create intuitive category structure
3. Add cross-links for related services
4. Include "How to Use This Catalog" guide
5. Format for your specific platform
```

---

### Step 9: Export Final Output
**Time: 5 minutes**

```
Format this service catalog for [ServiceNow / Confluence / etc.]. Include:
- Service request forms with appropriate fields
- Approval workflows where needed
- Integration with ticketing system
- Analytics/reporting structure
```

---

## Example Output

Below is an abbreviated example of what a well-executed IT service catalog looks like:

---

> ## IT Service Catalog
>
> **Your Guide to IT Services**
>
> ---
>
> ### How to Use This Catalog
>
> 1. Browse categories below or use search
> 2. Click a service to see details
> 3. Click "Request" to submit your request
> 4. Track your request in the My Requests portal
>
> **Questions?** Contact the Help Desk at x5000 or it-help@company.com
>
> ---
>
> ## Service Categories
>
> ### Computer & Devices
> - New Computer Request
> - Mobile Device Setup
> - Monitor/Peripheral Request
> - Loaner Equipment
>
> ### Network & Access
> - VPN Access
> - Guest WiFi
> - Network Drive Access
>
> ### Communication & Collaboration
> - Email Account (Microsoft 365)
> - Microsoft Teams
> - Distribution List Management
>
> ---
>
> ## VPN Access (Remote Work)
>
> **Get secure access to company resources from anywhere.**
>
> #### What is this?
>
> VPN (Virtual Private Network) lets you securely connect to company systems when you're working from home, traveling, or using public WiFi. Once connected, you can access email, files, and applications just like you're in the office.
>
> #### Who can request this?
>
> - All employees
> - Contractors (requires manager and Security approval)
>
> #### What's included
>
> ✓ VPN software installed on your computer
> ✓ Secure connection to company network
> ✓ Access to internal applications and files
> ✓ Multi-factor authentication setup
> ✓ Initial training/walkthrough
>
> #### What's NOT included
>
> ✗ VPN on personal devices (company devices only)
> ✗ Internet service at your home
> ✗ 24/7 support (business hours only)
>
> #### How to request
>
> 1. Click **Request Service** below
> 2. Confirm your device is company-issued
> 3. Select your preferred installation date/time
> 4. Submit request
>
> Your manager will be notified. No additional approval needed for employees.
>
> **[Request VPN Access]** (button)
>
> #### Service levels
>
> | Metric | Target |
> |--------|--------|
> | Request acknowledgment | Within 4 business hours |
> | Installation completed | Within 3 business days |
> | Support hours | Mon-Fri, 8am-6pm |
>
> #### Cost
>
> No charge to your department.
>
> #### Frequently Asked Questions
>
> **Q: Can I use VPN on my personal computer?**
> A: No, VPN is only supported on company-issued devices for security reasons.
>
> **Q: Do I need to be connected to VPN all the time?**
> A: When working remotely, yes—you'll need VPN to access company email, files, and applications.
>
> **Q: VPN is running slowly. What can I do?**
> A: VPN speed depends on your home internet. Try moving closer to your WiFi router or using a wired connection. If problems persist, contact support.
>
> #### Related Services
> - New Computer Request
> - Password Reset
> - IT Help Desk

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Catalog too technical for users | Written from IT perspective | Write from user perspective; focus on outcomes; avoid jargon; test with actual employees |
| Services too granular | Creating entry for every technical task | Bundle related services; create service packages; think user journeys not IT tasks |
| No one uses the catalog | Easier to email IT directly | Integrate with ticketing; make catalog the only way to request; promote heavily; measure adoption |
| Information gets stale | No ownership or update process | Assign service owners; set review cadence (quarterly); trigger updates on service changes |
| Inconsistent service delivery | No standard procedures documented | Create fulfillment procedures for IT staff; train on standards; measure consistency |
| Service levels unrealistic | Optimistic targets without capacity check | Base SLAs on historical data; account for capacity; review and adjust quarterly |

---

## Tips from Experience

1. **User language.** Write from the employee's perspective, not IT's. "Get remote access" not "VPN provisioning."

2. **Outcome focus.** Lead with what the user gets, not the technology. They don't care about VPN protocols, they care about working from home.

3. **Clear expectations.** Tell users exactly when they'll get the service and what the process looks like. Uncertainty creates support calls.

4. **Bundle smartly.** Package related services for common needs. "New Employee IT Setup" is better than 7 separate service requests.

5. **Show costs transparently.** Even if there's no charge, say "No charge to your department" explicitly. It demonstrates value.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Catalog usage increases month over month (track service requests)
- [ ] Informal requests (email, walk-ups) decrease significantly
- [ ] User satisfaction with IT services improves
- [ ] Service delivery times meet SLA targets
- [ ] Self-service adoption rate increases

**Track over time:**
- Catalog views and service request submissions
- Request-to-fulfillment time per service
- User satisfaction scores (post-service surveys)

---

## Variations

### Customer-Facing Service Catalog
**When to use:** External service offerings for customers or partners
```
Adapt for external audience:
- Customer-friendly language and branding
- Payment and billing integration
- Self-service portal for customers
- Different SLA structure
- Support escalation to customer success teams
```

### Shared Services Catalog
**When to use:** Cross-functional services (HR, Finance, Facilities)
```
Unified catalog across departments:
- HR services (benefits, leave, onboarding)
- Finance services (expense reporting, procurement)
- Facilities services (parking, moves, supplies)
- Consistent UX across all service types
- Single portal for all employee needs
```

### Cloud Service Catalog
**When to use:** Self-service provisioning of cloud resources
```
Developer self-service focus:
- AWS/Azure/GCP resource provisioning
- Environment templates (dev, test, prod)
- Automated approval and provisioning
- Cost tracking and chargebacks
- Governance guardrails built-in
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create service entry templates** ensuring consistent user-facing and IT-facing format. Include all required sections (description, eligibility, what's included, SLAs, cost).

2. **Establish service ownership model** where each service has a named owner responsible for documentation, SLAs, and continuous improvement.

3. **Integrate with ITSM platform** (ServiceNow, Jira Service Management) so catalog is connected to ticketing, approvals, and fulfillment workflows.

4. **Set up regular review cycles** (quarterly) where service owners review and update their catalog entries. Trigger reviews on major IT changes.

**Sample Folder Structure:**
```
it-service-catalog/
├── user-facing/
│   ├── computer-devices/
│   │   ├── new-computer.md
│   │   ├── mobile-device.md
│   │   └── peripherals.md
│   ├── network-access/
│   │   ├── vpn-access.md
│   │   └── guest-wifi.md
│   └── applications/
│       ├── software-installation.md
│       └── application-access.md
├── it-facing/
│   ├── fulfillment-procedures/
│   ├── support-procedures/
│   └── known-issues/
├── templates/
│   ├── service-entry-template.md
│   ├── technical-doc-template.md
│   └── fulfillment-procedure-template.md
└── governance/
    ├── sla-definitions.md
    ├── service-ownership.md
    └── review-schedule.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming scattered services into organized, self-service catalog**—applies broadly:

| Role | Application |
|------|-------------|
| **HR Teams** | Employee service catalog (benefits, leave, policy questions, onboarding) |
| **Facilities** | Office services catalog (parking, room booking, supplies, moves) |
| **Finance** | Finance service offerings (expense reporting, procurement, vendor setup) |
| **Legal** | Legal services menu (contract review, NDA requests, compliance questions) |
| **External Services** | Customer-facing service catalogs for B2B or B2C offerings |

---

## Next Steps

1. **This week:** Catalog your top 5 services by request volume. Publish them and promote to employees.

2. **Track your results:** Measure baseline request volume through email/walk-ups. Track shift to catalog requests.

3. **Iterate:** Collect user feedback after service delivery. Use feedback to improve catalog entries and service delivery.

4. **Share:** Promote catalog in onboarding, email signatures, intranet homepage. Make it the path of least resistance.

---

*Recipe #95 of 100 in the Claude Code Knowledge Worker Recipe Collection*
