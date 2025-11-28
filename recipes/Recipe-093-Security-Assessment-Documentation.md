# Security Assessment Documentation

**Recipe #93: From Raw Findings to Actionable Security Reports**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 25 minutes (first time) / 15 minutes (repeat) | 4-8 hours per assessment | Advanced | Security Analysts, Compliance Officers, IT Auditors |

---

## The Problem

Security assessments generate extensive technical findings that need translation into actionable documentation for multiple audiences—technical teams need remediation details, management needs risk context, and compliance teams need evidence mapping. Writing comprehensive security reports that serve all these audiences while maintaining accuracy is time-consuming and often results in reports that satisfy no one fully.

**Pain Points:**
- Technical findings don't translate into business risk for executives
- Inconsistent severity ratings across different assessors or tools
- Remediation guidance too vague to be actionable
- Compliance framework mapping missing or incomplete
- Reports too long and technical for stakeholders to read
- Finding descriptions lack context for non-security personnel
- No clear prioritization of what to fix first

---

## The Outcome

Clear, structured security assessment documentation that presents findings with appropriate context, risk ratings, remediation guidance, and compliance mapping—enabling stakeholders to understand risks and take action.

**What You'll Have When Done:**
- Executive summary translating technical risks to business impact
- Detailed findings with CVSS scores and risk classifications
- Compliance framework mapping (SOC 2, PCI DSS, GDPR, etc.)
- Prioritized remediation roadmap with effort estimates
- Technical procedures for validation and verification
- Evidence documentation for auditors

---

## When to Use This Recipe

**Good Fit:**
- Vulnerability assessment reports
- Penetration testing documentation
- Security audit reports
- Compliance gap analysis
- Third-party security reviews
- Risk assessment documentation
- Security control evaluations

**Not a Good Fit:**
- Real-time vulnerability dashboards (use automated tools)
- Incident response reports (different format and urgency)
- Continuous monitoring alerts (different workflow)
- Bug bounty triage (faster turnaround needed)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Raw assessment findings collected
- [ ] Vulnerability scan results available
- [ ] Testing scope and methodology documented
- [ ] Asset inventory accessible
- [ ] Compliance framework requirements listed
- [ ] Risk tolerance definitions from management
- [ ] Remediation timeline expectations known
- [ ] Stakeholder audience definitions clear
- [ ] You have 60-90 minutes for report creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforms raw security findings into structured reports
- Assigns consistent risk ratings across findings
- Maps findings to compliance frameworks systematically
- Generates actionable remediation recommendations
- Creates executive summaries translating technical risks to business impact
- Organizes findings by severity, category, and compliance impact
- Formats technical details appropriately for different audiences

**Where Human Judgment Is Essential:**
- Validating CVSS scores match actual exploitability
- Determining business-specific risk ratings
- Assessing compliance impact based on certification timeline
- Prioritizing remediation based on organizational context
- Reviewing for false positives or tool errors
- Deciding what information to redact for different audiences

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Assessment scope | Systems tested, methodology, timeframe | Context and limitations section |
| Raw findings | Vulnerability descriptions, evidence | Detailed findings documentation |
| Compliance requirements | SOC 2, PCI DSS, GDPR criteria | Framework mapping and gap analysis |
| Risk framework | CVSS, internal risk matrix | Consistent severity ratings |
| Asset context | System criticality, data sensitivity | Business impact assessment |

**Sample Input:** *(Raw vulnerability finding)*
```
FINDING: SQL Injection in Search Function
Location: /api/v2/search endpoint, 'query' parameter
CVSS: 9.8 (AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H)
Evidence: Parameter accepts unescaped SQL. Payload ' OR '1'='1 returns
all records. Sqlmap confirmed database enumeration possible.
Impact: Full database access, potential data exfiltration
```

---

## Step-by-Step Implementation

### Step 1: Gather Assessment Materials
**Time: 15-20 minutes**

Collect all assessment artifacts:
- Export vulnerability scan results
- Compile manual testing findings
- Gather screenshots and proof-of-concept evidence
- Document testing methodology and scope
- List compliance frameworks that apply
- Identify stakeholder audiences

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Findings Analysis Prompt
**Time: 20-25 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze Security Findings**

```
Claude, I need to create a security assessment report.

Assessment scope:
- System: [Customer Portal Application]
- Components tested: [Web app, API, database tier, authentication]
- Methodology: [OWASP Testing Guide, manual pentesting, vulnerability scanning]
- Period: [October 15-30, 2024]
- Environment: [Staging / Production]

Raw findings:
[Paste all findings with evidence, severity, location, impact]

Compliance context:
- Frameworks: [SOC 2 Type II, PCI DSS, GDPR]
- Certification timeline: [In progress / upcoming audit]

Help me:
1. Validate severity ratings for consistency
2. Categorize findings by type (injection, auth, config, etc.)
3. Identify any related or duplicate findings
4. Assess overall risk posture based on findings
```

---

### Step 4: Review and Validate
**Time: 15 minutes**

**Check immediately:**
- Severity ratings are consistent and justified
- Finding categories make sense
- No duplicate or overlapping findings

**Spot-check specifics:**
- CVSS scores match attack vectors
- Evidence supports severity claims
- Business impact assessments are realistic

---

### Step 5: Generate Report Sections
**Time: 30-40 minutes**

Create each section systematically:

**For Risk Ratings and Compliance Mapping:**
```
Standardize risk ratings for these findings:

Findings: [Paste analyzed findings]
Compliance frameworks: [SOC 2, PCI DSS, GDPR requirements]

For each finding, provide:
1. Severity (Critical/High/Medium/Low/Informational) with justification
2. CVSS score breakdown
3. Exploitability rating (Easy/Moderate/Difficult)
4. Business impact (High/Medium/Low)
5. Relevant compliance requirements affected
6. Gap or violation type for each framework
```

**For Remediation Guidance:**
```
Create remediation recommendations:

Findings: [Paste findings]
Tech stack: [Programming languages, frameworks, platforms in use]

For each finding:
1. Immediate mitigation steps (if applicable)
2. Long-term remediation with code examples or configuration changes
3. Verification method to confirm fix
4. Estimated effort (hours/days)
5. Priority ranking based on risk and effort
```

**For Executive Summary:**
```
Write an executive summary for this security assessment:

Key findings count by severity: [Critical: 1, High: 1, Medium: 3, Low: 2]
Most critical risks: [SQL injection, authorization bypass]
Business context: [System handles customer orders and payment data]
Compliance status: [SOC 2 in progress, PCI DSS applicable]
Audience: [Executive leadership, board]

Include:
1. Overall security posture assessment (1-2 sentences)
2. Critical risks requiring immediate attention (2-3 items)
3. Compliance impact summary (table format)
4. Recommended action plan with timeline (immediate/short/medium term)
5. Business risk summary (breach risk, regulatory penalties, reputation)
```

---

### Step 6: Assemble Complete Report
**Time: 15-20 minutes**

```
Compile the security assessment into a complete report:

Sections to include:
- Executive Summary: [Paste]
- Assessment Overview: [Scope, methodology, limitations]
- Findings Summary: [Statistics, risk distribution]
- Detailed Findings: [Each finding with full technical details]
- Compliance Mapping: [Framework impact tables]
- Remediation Roadmap: [Prioritized action plan with timeline]
- Appendix: [CVSS calculations, tool output, references]

Please:
1. Ensure consistent terminology and severity language
2. Add table of contents with page numbers
3. Include document control (version, date, classification)
4. Cross-reference findings to remediation roadmap
5. Format for professional presentation
```

---

### Step 7: Export Final Output
**Time: 5 minutes**

```
Format this security assessment report for [PDF / Confluence / SharePoint]. Include:
- Professional formatting with headers and footers
- Document classification markings (Confidential)
- Version control information
- Proper page breaks and section navigation
```

---

## Example Output

Below is an abbreviated example of what a well-executed security assessment report looks like:

---

> **SECURITY ASSESSMENT REPORT**
> **Customer Portal Application**
> *Q4 2024*
>
> **Classification:** Confidential
> **Prepared for:** [Client Name]
> **Date:** November 1, 2024
> **Version:** 1.0
>
> ---
>
> ## Executive Summary
>
> **Overall Risk Rating: HIGH**
>
> The Customer Portal application contains critical security vulnerabilities that pose significant risk to customer data and regulatory compliance. Immediate attention is required for two critical/high-severity findings that could result in unauthorized data access.
>
> **Key Findings:**
>
> | Severity | Count | Description |
> |----------|-------|-------------|
> | Critical | 1 | SQL injection allowing full database compromise |
> | High | 1 | Authorization bypass exposing customer orders |
> | Medium | 3 | Authentication and encryption weaknesses |
> | Low | 2 | Information disclosure and missing hardening |
>
> **Critical Risks:**
>
> 1. **SQL Injection Vulnerability** - Unauthenticated attacker can extract all database contents including customer data, payment information, and credentials. This represents critical breach risk and compliance violation.
>
> 2. **Authorization Bypass (IDOR)** - Any authenticated user can access any other customer's order data, violating data privacy principles.
>
> **Compliance Impact:**
>
> | Framework | Status | Impact |
> |-----------|--------|--------|
> | SOC 2 | At Risk | Critical findings may affect certification timeline |
> | PCI DSS | Non-Compliant | Requirement 6.5 violations identified |
> | GDPR | At Risk | Data protection inadequacies present |
>
> **Recommended Action Plan:**
>
> - **Immediate (0-7 days):** Patch SQL injection, implement authorization checks
> - **Short-term (7-30 days):** Strengthen password policy, update TLS, implement session timeout
> - **Medium-term (30-90 days):** Deploy security headers, sanitize error messages
>
> ---
>
> ## Detailed Findings
>
> ### Finding #1: SQL Injection in Search Function
>
> | Attribute | Value |
> |-----------|-------|
> | **Severity** | Critical |
> | **CVSS Score** | 9.8 (Critical) |
> | **Location** | /api/v2/search |
>
> **Description:**
> The search API endpoint is vulnerable to SQL injection through the 'query' parameter. User input is concatenated directly into SQL queries without sanitization.
>
> **Proof of Concept:**
> ```
> GET /api/v2/search?query=' OR '1'='1
> ```
>
> **Impact:**
> - Confidentiality: Complete loss - all database data accessible
> - Integrity: High risk - data modification possible
> - Availability: Medium risk - denial of service possible
>
> **Compliance Mapping:**
>
> | Framework | Requirement | Status |
> |-----------|-------------|--------|
> | SOC 2 | CC6.1 - Access controls | Non-compliant |
> | PCI DSS | 6.5.1 - Injection flaws | Violated |
> | GDPR | Article 32 - Security measures | Inadequate |
>
> **Remediation:**
>
> **Immediate (24-48 hours):**
> 1. Implement input validation on query parameter
> 2. Deploy WAF rule to block SQL injection patterns
> 3. Consider temporarily disabling search if fix delayed
>
> **Long-term:**
> ```python
> # Secure implementation
> from sqlalchemy import text
> query = text("SELECT * FROM products WHERE name LIKE :search")
> result = db.execute(query, {"search": f"%{user_input}%"})
> ```
>
> **Verification:** Re-test with SQL injection payloads; confirm prepared statements in code review
>
> **Estimated Effort:** 4-8 hours development + 2 hours testing

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Findings lack business context | Technical focus without business translation | Include business impact, compliance mapping, breach scenarios for each critical finding |
| Inconsistent severity ratings | Different assessors or tools rate differently | Use standardized framework (CVSS); document rating rationale; have single reviewer calibrate |
| Remediation too vague | Generic "fix the vulnerability" guidance | Provide specific code examples, configuration changes, step-by-step procedures |
| Report too long for executives | Burying critical findings in details | Strong executive summary up front; critical findings first; detailed technical appendix |
| Compliance mapping incomplete | Not considering all applicable frameworks | Create checklist of frameworks; map each finding systematically; review with compliance team |
| False positives not filtered | Automated scan results used without validation | Manually verify all findings; test proof-of-concept; remove or downgrade false positives |

---

## Tips from Experience

1. **Lead with risk.** Critical findings first, always. Don't make executives hunt for what matters most.

2. **Show evidence.** Screenshots, logs, and proof-of-concept demonstrations build credibility and help developers reproduce issues.

3. **Be specific.** Document exact endpoints, parameters, and conditions. Generic findings waste everyone's time during remediation.

4. **Provide context.** Why does this matter to THIS organization? Connect technical vulnerabilities to business consequences.

5. **Include working fixes.** Code examples and configuration samples accelerate remediation and reduce back-and-forth.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Executive team understands security posture without asking clarifying questions
- [ ] Development team can remediate findings without additional guidance
- [ ] Compliance team can map findings to framework requirements
- [ ] Remediation timeline is met (critical items fixed within target window)
- [ ] Follow-up assessment shows significant improvement

**Track over time:**
- Time from assessment completion to report delivery
- Remediation rate within target timeframes
- Reduction in repeat findings across assessments

---

## Variations

### Penetration Test Report
**When to use:** External attacker simulation with exploitation chain
```
Emphasis on attack narrative and business impact demonstration:
- Executive briefing on what attacker could achieve
- Attack chain: reconnaissance → exploitation → lateral movement → data access
- Business impact demonstration (screenshots of accessed data)
- Detection gap analysis (what security controls missed)
- Remediation roadmap prioritized by attack path
```

### Compliance Gap Analysis
**When to use:** Mapping current state against framework requirements
```
Focus on framework compliance:
- Control-by-control assessment against framework
- Gap identification with severity
- Evidence requirements for closing gaps
- Remediation roadmap aligned to audit timeline
- Sample evidence documentation
```

### Third-Party Security Assessment
**When to use:** Vendor or partner security evaluation
```
Structured for external stakeholder consumption:
- Executive summary suitable for vendor sharing
- Risk ratings in business terms
- Remediation requirements and timeline
- Appropriate redaction of sensitive details
- Follow-up verification process
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create finding templates** with consistent structure: description, evidence, impact, compliance mapping, remediation, verification. This ensures nothing is missed.

2. **Establish severity calibration sessions** where team reviews ratings together monthly. This creates consistency across assessors.

3. **Build a remediation guidance library** of common vulnerability fixes with code examples. Reference this library in reports.

4. **Implement a report review workflow** where technical findings are peer-reviewed before executive summary is written.

**Sample Folder Structure:**
```
security-assessments/
├── templates/
│   ├── finding-template.md
│   ├── executive-summary-template.md
│   └── remediation-roadmap-template.md
├── 2024-Q4-customer-portal/
│   ├── raw-findings/
│   ├── evidence/
│   ├── draft-report.md
│   └── final-report.pdf
├── remediation-library/
│   ├── sql-injection-fixes.md
│   ├── auth-best-practices.md
│   └── tls-configuration.md
└── compliance-mapping/
    ├── soc2-controls.md
    ├── pci-dss-requirements.md
    └── gdpr-articles.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming technical findings into multi-audience reports**—applies broadly:

| Role | Application |
|------|-------------|
| **Vendor Risk Teams** | Third-party security review documentation, vendor risk assessments |
| **Audit Teams** | Evidence compilation for auditors, control testing documentation |
| **Incident Response** | Post-incident reports, lessons learned documentation |
| **Policy Teams** | Security policy documentation, control framework documentation |
| **Risk Management** | Risk register maintenance, risk assessment documentation |

---

## Next Steps

1. **This week:** Present findings to stakeholders. Brief executives on critical risks, developers on remediation details.

2. **Track your results:** Create remediation tickets with clear acceptance criteria. Track completion rate against timeline.

3. **Iterate:** Schedule re-testing of fixed vulnerabilities. Update report with verification results.

4. **Share:** Update compliance documentation with assessment results. Brief audit team on findings and remediation progress.

---

*Recipe #93 of 100 in the Claude Code Knowledge Worker Recipe Collection*
