# Tom Occon

**Forward Deployed Engineer · AI & Data Systems · Customer Outcomes**

Lehi, UT · [LinkedIn](https://linkedin.com/in/tom-occon) · tom.occon@gmail.com

---

## The Short Version

I build systems that solve real customer problems. I was a Support Manager who started
building AI tools proactively — before anyone asked. Domo's Chief AI & Analytics Officer
saw one of those tools and cited it to the CTO in a company-wide executive brief as an
example of what's possible. The CEO doubled down on the FDE motion. I was one of the
first people to transition into that role.

That's not a resume arc. That's a demonstrated pattern:

> **See a problem → build the solution → create a business outcome → be trusted with the next, harder problem.**

---

## Career Arc

```
Manager, Preferred Technical Support
        │
        ├─ Built an AI-powered account review workflow using
        │  Domo's own platform. Showed it to the Chief AI Officer.
        │  He cited it to the CTO in an executive distribution email
        │  as the reference example for what's possible.
        │
        ├─ Led the Brilliance Bar at Domo's annual customer conference
        │  (Domopalooza): ~300 customer sessions, $78.6M total ACV engaged,
        │  9.64/10 CSAT (81% perfect scores), 43% Director-level+ attendees.
        │  VP of Technical Support called out my leadership specifically.
        │
        ├─ Built an AI ROI calculator for a strategic customer whose
        │  analytics director wrote: "Easily the most impressed I've been
        │  coming out of a vendor meeting in the decade I've been doing this."
        │  It reached the CEO and CMO. Domo's CCO emailed me directly:
        │  "May have heard YOU were the mastermind?"
        │
        ↓
Forward Deployed Engineer
        │
        ├─ Part of the first wave of the CEO's strategic initiative
        │  to double down on Domo's FDE motion
        │
        ├─ Led a high-stakes executive onsite for a customer whose CEO
        │  flew in people from across the country for the single meeting.
        │  Live from the room: "The customer has said game changer
        │  more times than I can count."
        │
        ├─ 35+ enterprise customer builds across 10+ industries
        │  in the first 4 months in the role
        │
        └─ Built the internal operating system for Domo's entire
           Professional Services organization (v9+, 50-100+ users)
```

---

## What I Actually Build

### Internal Platform (Production)

**[Professional Services Operations Platform](https://github.com/Concon8991/forward-deployed-operations-platform)**

The operating system for an enterprise professional services organization — built from
a 1,464-line spec I authored, now in **v9+ and live in production** serving 50–100+
employees. Not a prototype. Not a POC. A production system with:

- 22 data sources integrated (Salesforce, SPP, Gong calls, health signals, support cases)
- 14 application state collections
- 7 persona-aware views (IC, manager, leader, client, partner, admin)
- AI meeting prep: Gong transcripts + pending tasks → structured briefing document
- Live AI account intelligence ("Why this account needs attention")
- Automated timesheet workflow that cut a 20-minute weekly task to under 5 minutes — for every IC on the team
- Full audit trail, Salesforce writeback, client portal with external persona isolation

**Stack:** React 19 + TypeScript + Vite + Tailwind + AppDB + Code Engine + DomoGPT + Magic ETL

---

### Enterprise Customer Delivery

**Aviation Capital Group — Trading Tape Automation**

ACG manages 100+ aircraft leases globally. Their team spent 3–4 hours per week
manually extracting data from 6+ sources into Excel, formatting per-aircraft tabs.
I automated the entire process end-to-end: Jupyter workspace (44 datasets), Snowflake
ODBC integration, Documents API, multi-environment promotion via Domo Sandbox.

A critical Snowflake field truncation bug surfaced under a same-day deadline from
the customer's director. I diagnosed and resolved it in the same session.
At go-live, senior stakeholders called it "flooring." A trader requested a live pull
before V1 was even released.

**Home Depot — AI Markup Pricing Tool (built in under 24 hours)**

For a Fortune 50 stakeholder demo, I built a complete AI-driven salvage pricing
system: 16.2M-row HDR scan data + Google BigQuery inventory → AI-recommended markups
by department/class/subclass with confidence scores + approve/deny workflow that
writes back to audit tables. Zero to demo in under one business day.

**Power BI → Domo Migration Tooling**

Built a Power BI REST API automation script that converts Power BI dashboards to
Domo App Studio using Claude Code. Applied at multiple Fortune 500 accounts.
Reference outcome: ~1,000 Power BI dashboards migrated for a prior customer in
approximately one week. At one engagement, the executive sponsor designated
Domo as the company's sole reporting platform and began sunsetting Power BI
as a direct result.

**Instance Governance (73% credit reduction program)**

Full audit of a customer's cloud analytics environment: 2,000+ orphaned datasets,
22M duplicate rows across 55 datasets, one dataset at 126M rows with no clear owner.
Developed and am executing a phased remediation program. Projected outcome:
73% reduction in cloud computing credit consumption by year-end.

---

### AI Systems

**[AI Support Intelligence Pipeline](https://github.com/Concon8991/ai-support-intelligence)**

LLM pipeline for scoring and analyzing support cases at operational scale.
The engineering problems that actually matter at scale: context preservation across
long case threads, token-bucket throttling at 90K TPM, hash-based idempotent re-runs,
structured output enforcement so downstream SQL never breaks. Real code included.

**[Scoob — Personal AI Operating System](https://github.com/Concon8991/scoob-ai-architecture)**

The multi-agent system I built to run my own FDE work:
175+ persistent memories, 40 specialist agents, 200+ MCP tools, continuous monitoring
of email + Teams + SharePoint across active customer accounts. Referenced internally
as "auto-monitoring for [multiple customers] every 15 minutes."

---

### Data Engineering

**[Customer Data Engineering Patterns](https://github.com/Concon8991/customer-data-engineering)**

Production failure modes and the patterns that prevent them — from real engagements:
the silent row multiplication ($40K financial delta, no error in the log), the memory
failure that only appears at production data volume, the connector that returns 98%
of records and calls it success. Documented because these are what distinguish
a reliable system from a demo that breaks the third time it runs.

---

## Industry Breadth

In 4 months as an FDE, I've built across:

| Industry | What I Delivered |
|----------|-----------------|
| Aviation / Asset Leasing | Automated trading tape, Snowflake integration, multi-env deployment |
| Retail / Home Improvement | AI pricing engine, BigQuery integration, Fortune 50 stakeholder delivery |
| Mortgage / Financial Services | Turn time automation, AI chatbot, Power BI displacement |
| Construction / Engineering | ECAC cost-at-completion modeling, S-curve project tracking |
| Media / Broadcasting | Campaign performance platform, advertiser portal |
| Consumer Food / Franchise | 36M-row POS + delivery + e-commerce unified analytics |
| Nonprofit / Retail Operations | AI document intelligence, multi-location data intake |
| Technology / SaaS | Agentic analytics, competitive displacement of ThoughtSpot + Snowflake Cortex |
| Enterprise IT | Vendor lifecycle management, contract risk intelligence |
| Professional Services (Internal) | Full PS operating system, capacity planning, AI synthesis |

---

## What "Business Acuity" Actually Looks Like

I don't build dashboards. I build things that change what people do.

The Support team at Domopalooza wasn't just a customer touchpoint — I helped
frame it as a pipeline engine: 60% of the $78.6M ACV we engaged were on lower
support tiers, which meant every conversation was a live expansion opportunity.
I co-wrote the executive summary that surfaced that analysis to VP and C-suite.

When I built the Trimble AI account review workflow, I didn't just build it —
I showed it to the Chief AI & Analytics Officer and explained what it enabled
strategically. That conversation went from the CAO to the CTO in an
executive distribution email. From a manager with a side project.

When the opportunity existed to displace Power BI at a financial services company,
I understood the commercial play well enough to build migration tooling that
made the transition cost nearly nothing — and let the executive sponsor declare
Domo as the company's sole platform with confidence.

The technical work is real. The business outcomes are the point.

---

## Strategic Contributions

**Domo Preferred Support — Brilliance Bar Co-Lead (Domopalooza 2026)**
Co-led all on-site customer operations at Domo's annual conference:
~300 appointments, $78.6M ACV engaged, 9.64/10 CSAT, 43% Director+.
VP of Technical Support cited me and two other leaders specifically:
*"You set the tone, coordinated the team seamlessly, and ensured that every
customer interaction reflected our commitment to excellence."*

**FDE Enablement Program (Co-Designer)**
Co-designed and delivered the 2-day AI-first enablement program for Domo's
entire Professional Services delivery team — the methodology, the tooling,
the pattern library that every FDE now uses.

**AI Center of Excellence**
Active member of the internal AI COE. Pitched autonomous account monitoring.
Contributed workflow skills to the shared team library.

**Product Influence**
Championed an AI readiness tool to Domo's Chief AI Officer and SVP Product.
It was evaluated for integration into the formal product roadmap.

**Team Pattern Library**
Patterns I develop on customer builds are promoted to the shared team library
and used by other FDEs on subsequent engagements — institutional knowledge
that outlives any individual project.

---

## Stack

`Python` · `TypeScript` · `React 19` · `Vite` · `Tailwind CSS` · `Framer Motion` ·
`SQL` · `pandas` · `Snowflake` · `BigQuery` · `Salesforce` · `Jupyter` ·
`Magic ETL` · `Claude Code` · `MCP` · `Domo` · `AppDB` · `Code Engine` ·
`Domo Workflows (BPMN)` · `LLM API integration` · `multi-agent orchestration`

---

*I'm open to the right opportunity — forward-deployed engineering, technical solutions
leadership, Head of FDE / Customer Engineering, or Director-level roles where deep
technical ownership and customer business outcomes are the same job.*
