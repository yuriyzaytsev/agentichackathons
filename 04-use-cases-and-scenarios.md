---
layout: default
title: "4. Use Cases & Scenarios"
permalink: /04-use-cases-and-scenarios/
---

# 4. Use Cases & Scenarios

## Core Principles

### 1. Inspire, Don't Implement

> ⚠️ **Field Insight:** The goal is NOT to apply the customer's real scenario end-to-end. It is to **inspire** — show that their scenario CAN be done. Use invented companies and simplified scenarios. It's a hackathon, not reality.

### 2. Process Automation Over RAG

> ⚠️ **Field Insight:** Customers often want a "magic system to retrieve documents" — but RAG is not the best fit for Copilot Studio. Instead, steer scenarios toward **process automation**: linked email data, structured data, workflow orchestration. Copilot Studio excels at business process automation, not unstructured document retrieval.

### 3. Business Process Focus = Higher Continuation Rate

> ⚠️ **Field Insight:** If scenarios are business-process focused, they have a high chance of actually continuing post-event because there will be a business owner interested in making them real. RAG use cases are often more horizontal — they benefit individuals but not necessarily the business. Process automation has a clear owner.

### 4. Prioritize Repeatable/Generalizable Use Cases

> ⚠️ **Field Insight:** Partners should prioritize use cases that can be **generalized and sold repeatedly** — not bespoke one-off demos. When partners invest time in a hackathon use case, it should scale their business. Example: a document redaction agent for government/public sector that can be sold to many organizations.

> 🔍 **[Enrichment]** Corporate agent-ready content team (presented week of April 2026) explicitly mandates that scenarios must be applicable across multiple customers to qualify for partner GTM support. This is a gating criterion for inclusion in official materials.

### 5. Quantify Benefits

> ⚠️ **Field Insight:** Quantify benefits — or at minimum show HOW you would quantify benefits. This feeds the ROI/business value case that makes post-event conversion easier.

## Use Case Preparation

### What to Prepare

| Element | Description | Who Prepares |
|---------|-------------|--------------|
| **One scenario per table** | Pre-built agent scenario aligned to industry/function | Partner (with Microsoft input) |
| **Backup simple use cases** | Quick-start scenarios to spur discussion when attendees hesitate | Partner/PSA |
| **Demo environment** | Working Copilot Studio environment with appropriate data | Partner (Spektra/CDX/customer) |
| **Dummy data** | Industry-relevant data loaded into SharePoint, Dataverse, etc. | Partner |

### Why Pre-Built Use Cases Are Essential

> ⚠️ **Field Insight:** You MUST have use cases in hand before the event. Reasons:
> 1. **Drives attendee selection** — process-specific use cases need process-knowledgeable people
> 2. **Avoids tumbleweed** — attendees often won't speak up first; no one wants to be first to share
> 3. **Gives each table a starting point** — look at the example first, try it out, THEN think of their own
> 4. **Right people in room** — if you define use cases at the event, you may not have the right people
>
>

### Use Case Design Guidelines

**DO:**
- Focus on business process automation (approvals, document generation, data enrichment)
- Design scenarios that showcase Copilot Studio's strengths (connectors, actions, orchestration)
- Make scenarios relevant to attendees' industries
- Keep scenarios achievable in 1–2 hours of hands-on time
- Show clear before/after value

**DON'T:**
- Default to RAG/document retrieval scenarios (Copilot Studio is not the best tool for this)
- Create scenarios that require production data or complex integrations
- Assume attendees can design from scratch without a starting point
- Make scenarios so simple they don't demonstrate real value

### Influencing Scenario Choice

When working with partners to define scenarios, help them evaluate:

1. **Is this a process automation scenario?** (preferred) vs. pure document retrieval
2. **Can this be sold to multiple customers?** (scalable IP) vs. bespoke one-off
3. **Is there a clear business process owner?** (ensures continuation)
4. **Can it be meaningfully demonstrated in 1–2 hours?** (hackathon-feasible)
5. **Does it show measurable value?** (leads to ROI conversation)

## Use Cases Drive Attendee Selection

```
Define use cases → Identify required process knowledge → Invite people with that knowledge
```

This is the correct sequence. Never:
```
Invite people → Hope they bring use cases → Try to make it work on the day
```

## Data Preparation

### Generating Dummy Data

> ⚠️ **Field Insight:** Teach partners to use **Copilot itself to generate dummy data** for scenarios. Partners may not think of this approach initially but once shown, they can prepare data for any scenario independently.

### Using MCP for Data Generation

> ⚠️ **Field Insight:** Use **MCP (Model Context Protocol) servers** to generate data directly in the right locations — SharePoint, Dataverse, D365 — rather than manually copy-pasting generated content. This is more powerful than generating data and manually placing it.

> 🔍 **[Enrichment]** MCP servers can expose structured data and tools to agents. For hackathon prep, they can provide read-only synthetic datasets, avoid direct DB access, and reduce hallucinations through structured context. No official "hackathon MCP template" exists yet — usage is optional and scenario-driven.

### Data Sources for Scenarios

| Source | Best For | Setup Effort |
|--------|----------|--------------|
| Copilot-generated dummy data | Any scenario; quick customization | Low |
| MCP server-generated data | Structured data in correct locations (SP, D365) | Medium |
| Spektra pre-built scenarios | Standard industry scenarios | Very Low |
| Partner-prepared datasets | Partner IP scenarios | Medium |

## Environment Options

### Decision Matrix

| Option | Best For | Scale | Setup Effort | Duration | Cost |
|--------|----------|-------|--------------|----------|------|
| **Spektra Systems** | Hands-on agent build; multi-customer | Medium–Large | Very low | 24 hours | ~$1,000 USD per event (up to 50 participants) |
| **Customer environment** | Real data PoV; single customer | Small–Medium | High | 60-90 days (trial licenses) | Internal |
| **CDX** | Demos, PSA-led workshops | Small | Medium | Limited | Free (internal) |
| **Partner benefits** | Partner's own demos | Small | Low | Ongoing | Included in MAICPP |

### Spektra Systems (Recommended for Multi-Customer Events)

Each attendee receives a dedicated environment with:
- Microsoft Copilot Studio
- Copilot for Microsoft 365
- Microsoft 365 Business Premium licenses

**Environment lifetime**: 24 hours (reset post-event, not for production use)

**How to request**: See [Resources & Tools](07-resources-and-tools.md#spektra-systems)

**Pre-built scenarios**: Spektra has scenarios they can incorporate. Partners can supplement with their own.

### Customer Environment (For Enterprise 1:1 Hackathons)

> ⚠️ **Field Insight:** For enterprise customers with an existing opportunity, you can request trial licenses running for 60–90 days. This turns the hackathon into a real pilot — not just a playing environment. Much more powerful because you have real data and real system access.

Requirements:
- Existing opportunity in place
- Customer approval for environment access
- IT admin available for setup and troubleshooting
- Sufficient lead time for provisioning

### Power Platform Environment Configuration

> ⚠️ **Field Insight:** Create **one Power Platform environment per table/team** to ensure isolation. Each table gets its own environment with one category of business.

> 🔍 **[Enrichment]** Power Platform environment-level isolation is supported. DLP / connector governance is handled in Power Platform Admin Center. Exact step-by-step creation and naming conventions are left to event design — not standardized in guidance.

## Table Topic Suggestions

### By Industry
Energy, Banking, Insurance, Capital Market, Pharma, Government, Manufacturing, Retail, Health Provider, Media & Entertainment, Non-Profit, Education, Information Technology

### By Business Function
Finance, Legal, Corporate Communication, Marketing, Customer Service, Sales, Human Resources, Operations, Executive, Accessibility, Sustainability

---

## Related

- [People & Roles](03-people-and-roles.md) — Use cases drive who should attend
- [Planning & Timeline](02-planning.md) — Step 4 preparation details
- [Resources & Tools](07-resources-and-tools.md) — Environment setup specifics
- [Event Execution](05-event-execution.md) — How scenarios are used on the day
