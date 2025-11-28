# API Integration Documentation

**Recipe #92: From Technical Specifications to Developer-Friendly API Docs**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 20 minutes (first time) / 10 minutes (repeat) | 4-6 hours per API | Intermediate | Technical Writers, API Developers, Developer Relations |

---

## The Problem

APIs are only as useful as their documentation. Developers evaluate APIs in minutes—if documentation is incomplete, confusing, or lacks examples, they'll choose a competitor or build workarounds. Many API docs are auto-generated from code and technically accurate but practically useless, missing context, common use cases, and gotchas that real integrators encounter.

**Pain Points:**
- Auto-generated docs are technically correct but don't help developers actually integrate
- Missing real-world examples that work out of the box
- Authentication setup unclear, causing hours of frustration
- Error codes documented but not explained or contextualized
- No guidance on rate limits until developers hit them
- Edge cases and gotchas discovered through painful trial and error
- Integration patterns left for developers to figure out themselves

---

## The Outcome

Developer-friendly API documentation with clear endpoint descriptions, request/response examples, authentication guidance, error handling, rate limits, and real-world integration patterns that help developers successfully integrate on the first attempt.

**What You'll Have When Done:**
- Complete getting started guide that gets developers to first API call in under 5 minutes
- Detailed endpoint documentation with working code examples
- Clear authentication and authorization documentation
- Comprehensive error reference with troubleshooting guidance
- Real-world integration patterns for common use cases
- Rate limiting and best practices documentation

---

## When to Use This Recipe

**Good Fit:**
- New API launch documentation
- API version migration guides
- Partner integration documentation
- Internal API documentation
- SDK and library documentation
- Webhook documentation
- Authentication flow documentation

**Not a Good Fit:**
- Real-time auto-generated reference (use API spec tools)
- GraphQL introspection docs (different pattern)
- Internal microservice contracts (simpler approach)
- Frequently changing experimental APIs

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] API specification (OpenAPI/Swagger, or code) available
- [ ] Authentication mechanism details documented
- [ ] Rate limits and quotas defined
- [ ] Error codes and meanings catalogued
- [ ] Example requests and responses prepared
- [ ] Common use cases identified
- [ ] Known limitations or gotchas listed
- [ ] Target developer audience defined
- [ ] You have 45-60 minutes for documentation creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transforms technical API specifications into developer-friendly documentation
- Generates realistic, working code examples in multiple languages
- Identifies common integration patterns from API structure
- Anticipates developer questions based on API design
- Creates consistent documentation format across all endpoints
- Maps error codes to actionable troubleshooting steps
- Extracts and organizes authentication flows

**Where Human Judgment Is Essential:**
- Validating code examples actually work against live API
- Determining which integration patterns to highlight
- Identifying which errors are actually common in practice
- Setting appropriate rate limit recommendations
- Deciding level of detail for different audiences
- Reviewing for security best practices

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| OpenAPI/Swagger spec | YAML or JSON spec file | Endpoint structure, request/response schemas, parameters |
| Engineering context | Auth details, rate limits, gotchas | Implementation guidance, best practices |
| Support tickets | Common developer questions | FAQ section, troubleshooting guide |
| Internal docs | How things actually work | Real-world context and edge cases |
| Sample code | Working examples | Code snippets in documentation |

**Sample Input:** *(OpenAPI specification excerpt)*
```yaml
paths:
  /orders:
    post:
      summary: Create a new order
      security:
        - ApiKeyAuth: []
      requestBody:
        required: true
        content:
          application/json:
            schema:
              $ref: '#/components/schemas/CreateOrderRequest'
      responses:
        '201':
          description: Order created successfully
        '400':
          description: Invalid request
        '429':
          description: Rate limit exceeded
```

---

## Step-by-Step Implementation

### Step 1: Analyze API Structure
**Time: 10-15 minutes**

Gather your API specification and context:
- Locate OpenAPI/Swagger spec or equivalent
- Collect authentication documentation
- List rate limits and quotas
- Gather common error codes
- Review support tickets for common issues

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the API Analysis Prompt
**Time: 15-20 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze API Structure**

```
Claude, I need to create API documentation.

Here's my OpenAPI spec:
[Paste spec]

Engineering context:
[Paste authentication details, rate limits, known issues]

Help me:
1. Understand the API's purpose and scope
2. Identify all endpoints and their relationships
3. Map authentication and authorization requirements
4. List rate limits and quotas
5. Note any gotchas or non-obvious behaviors
```

---

### Step 4: Review and Validate
**Time: 10 minutes**

**Check immediately:**
- Does the analysis capture all endpoints correctly?
- Are authentication requirements clear?
- Are there any security concerns flagged?

**Spot-check specifics:**
- Endpoint groupings make logical sense
- Authentication flow is accurate
- Rate limits match your actual implementation

---

### Step 5: Generate Documentation Sections
**Time: 25-35 minutes**

Create each section systematically:

**For Getting Started Guide:**
```
Write a "Getting Started" guide for this API:

API info: [Paste spec and context]
Target audience: [Describe developers - e.g., "Backend developers integrating e-commerce"]

Include:
1. What the API does (1-2 sentences)
2. Authentication setup steps
3. Making your first API call (complete example)
4. Common next steps
5. Where to get help
```

**For Endpoint Documentation:**
```
Create endpoint documentation for: [Specific endpoint]

Endpoint spec: [Paste endpoint from OpenAPI]
Context: [Any additional context about this endpoint]

For each endpoint, include:
1. Description and use case
2. Authentication requirements
3. Request parameters (path, query, body) with descriptions
4. Full request example with all common fields
5. Response structure with example
6. Error responses and meanings
7. Rate limiting considerations
8. Code examples in curl, Python, and Node.js
```

**For Integration Patterns:**
```
Document common integration patterns:

API capabilities: [Describe what API enables]
Use cases: [E.g., "e-commerce checkout", "bulk import", "status tracking"]

For each pattern:
1. Scenario description
2. Recommended approach
3. Complete code example
4. Error handling recommendations
5. Best practices and gotchas
```

---

### Step 6: Create Reference Documentation
**Time: 15 minutes**

```
Create reference documentation for:

Include:
1. Complete error code reference with descriptions and resolutions
2. Webhook event reference (if applicable)
3. Rate limit reference with recommendations
4. Changelog/versioning information
5. Available SDKs and libraries
6. Support and resource links

Format for quick lookup and scanning.
```

---

### Step 7: Export Final Output
**Time: 5 minutes**

```
Format this API documentation for [platform - e.g., "readme.io", "GitBook", "Swagger UI"]. Include:
- Proper navigation structure
- Code syntax highlighting
- Interactive examples where possible
- Search optimization
```

---

## Example Output

Below is an abbreviated example of what well-executed API documentation looks like:

---

> # Orders API Documentation
>
> **Version 2.0** | [Changelog](#) | [Support](#)
>
> ---
>
> ## Quick Start
>
> ### 1. Get Your API Key
>
> 1. Log in to the [Developer Dashboard](https://dashboard.example.com)
> 2. Navigate to **API Keys** → **Create Key**
> 3. Select scopes: `orders:read`, `orders:write`
> 4. Copy your key (shown only once)
>
> ### 2. Make Your First Request
>
> ```bash
> curl https://api.sandbox.example.com/v2/orders/test-order-123 \
>   -H "X-API-Key: your_sandbox_api_key"
> ```
>
> **Response:**
> ```json
> {
>   "id": "test-order-123",
>   "status": "confirmed",
>   "customer_id": "cust_abc123",
>   "created_at": "2024-01-15T10:30:00Z"
> }
> ```
>
> ---
>
> ## Authentication
>
> All API requests require an API key in the `X-API-Key` header.
>
> **Environments:**
>
> | Environment | Base URL | Purpose |
> |-------------|----------|---------|
> | Sandbox | `api.sandbox.example.com` | Testing and development |
> | Production | `api.example.com` | Live transactions |
>
> ⚠️ **Important:** Sandbox and production keys are not interchangeable.
>
> ---
>
> ## Create Order
>
> Creates a new order.
>
> ```
> POST /orders
> ```
>
> **Authentication:** Requires `orders:write` scope
>
> **Request Body:**
>
> | Field | Type | Required | Description |
> |-------|------|----------|-------------|
> | `customer_id` | string | Yes | Your customer identifier |
> | `items` | array | Yes | Order line items |
> | `idempotency_key` | string | Recommended | Prevents duplicate orders |
>
> **Example Request:**
>
> ```bash
> curl -X POST https://api.example.com/v2/orders \
>   -H "X-API-Key: your_api_key" \
>   -H "Content-Type: application/json" \
>   -d '{
>     "customer_id": "cust_abc123",
>     "items": [
>       {"product_id": "PROD-001", "quantity": 2}
>     ],
>     "idempotency_key": "order-12345-attempt-1"
>   }'
> ```
>
> **Response (201 Created):**
>
> ```json
> {
>   "id": "ord_xyz789",
>   "status": "pending",
>   "customer_id": "cust_abc123",
>   "items": [...],
>   "total": 126.63,
>   "created_at": "2024-01-15T10:30:00Z"
> }
> ```
>
> **Errors:**
>
> | Status | Code | Description |
> |--------|------|-------------|
> | 400 | `ORDER_001` | Invalid product_id (check case sensitivity) |
> | 401 | `UNAUTHORIZED` | Invalid or missing API key |
> | 429 | `RATE_LIMITED` | Rate limit exceeded (see Retry-After header) |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Auto-generated docs lack context | Relying solely on OpenAPI output | Supplement with guides, add descriptions and examples manually, focus on use cases |
| Examples don't work | Copy-paste from spec without testing | Test every example against live API; use realistic data; version examples with API |
| Developers confused by auth | Unclear setup or environment mixing | Create step-by-step auth guide; show environment-specific examples; document common mistakes |
| Error scenarios missing | Only documenting success paths | Document all error codes; explain common causes; provide resolution steps for each |
| Integration patterns unclear | Only documenting individual endpoints | Add integration guides for common workflows; show multi-step patterns; include best practices |
| Rate limiting surprises | Not documenting limits upfront | Make rate limits prominent; show headers; provide backoff examples; explain burst allowances |

---

## Tips from Experience

1. **Test everything.** Every code example should be copy-paste runnable. Use realistic data, not `foo` and `bar`.

2. **Think like a developer.** What would you want to know the first time integrating? Lead with that, bury the edge cases in appendices.

3. **Include gotchas prominently.** If product IDs are case-sensitive, say so immediately. Don't let developers discover this the hard way.

4. **Show, don't tell.** A working code example is worth a thousand words of prose. Provide examples in the languages your developers actually use.

5. **Version your docs carefully.** Keep documentation in sync with API versions. Make it crystal clear which docs match which API version.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Developers can make their first successful API call in under 10 minutes
- [ ] Support tickets about documented features decrease significantly
- [ ] Developer satisfaction scores (via surveys) are high
- [ ] API adoption rate increases
- [ ] Error rates among new integrators are low

**Track over time:**
- Time to first successful API call (instrument this if possible)
- Support ticket volume about API usage
- Developer NPS or satisfaction scores

---

## Variations

### GraphQL API Documentation
**When to use:** GraphQL APIs require different documentation approach
```
Focus on queries, mutations, and schema exploration:
- Schema documentation with field descriptions
- Query examples for common operations
- Mutation patterns with variables
- Subscription setup and usage
- GraphQL playground integration
```

### SDK/Library Documentation
**When to use:** You're documenting a client library, not raw HTTP
```
Library-specific documentation:
- Installation instructions per language/platform
- Initialization and configuration
- Method reference with parameters
- Common usage patterns
- Error handling in the SDK
- Upgrading between versions
```

### Internal API Documentation
**When to use:** Documentation for internal microservices
```
Less polish, more technical depth:
- Service-to-service authentication
- Internal error codes and debugging
- Performance characteristics
- Deployment and versioning
- Internal SLAs and support
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create documentation templates** for consistent API docs. Include standard sections: overview, authentication, endpoints, errors, SDKs, changelog.

2. **Establish a doc-before-release process** where API documentation is reviewed and approved before launching new endpoints or versions.

3. **Set up example testing in CI/CD** to ensure code examples stay current. Break the build if examples fail against staging API.

4. **Create a developer feedback loop** through surveys, support ticket analysis, and community channels to identify documentation gaps.

**Sample Folder Structure:**
```
api-docs/
├── getting-started/
│   ├── quickstart.md
│   ├── authentication.md
│   └── environments.md
├── endpoints/
│   ├── orders.md
│   ├── customers.md
│   └── payments.md
├── guides/
│   ├── error-handling.md
│   ├── rate-limits.md
│   └── webhooks.md
├── reference/
│   ├── errors.md
│   ├── sdks.md
│   └── changelog.md
└── examples/
    ├── python/
    ├── node/
    └── curl/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming technical specifications into developer-friendly guides**—applies broadly:

| Role | Application |
|------|-------------|
| **Webhook Providers** | Event-driven integration documentation, payload references, security verification |
| **SDK Maintainers** | Library documentation, method references, upgrade guides |
| **Platform Teams** | Internal service-to-service API documentation |
| **Partner Programs** | Custom integration guides for partner APIs |
| **Developer Advocates** | Public API documentation for developer portals |

---

## Next Steps

1. **This week:** Test your documentation with a developer unfamiliar with the API. Watch where they get stuck.

2. **Track your results:** Instrument time-to-first-successful-call. Set a goal to reduce it by 50%.

3. **Iterate:** Set up a feedback mechanism on every doc page. Review and address feedback weekly.

4. **Share:** Create a developer portal or dedicated docs site. Make documentation as easy to find as the API itself.

---

*Recipe #92 of 100 in the Claude Code Knowledge Worker Recipe Collection*
