# Tom Occon

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║   FORWARD DEPLOYED ENGINEERING                                   ║
║   AI  ·  DATA SYSTEMS  ·  CUSTOMER SOLUTIONS                    ║
║                                                                  ║
║   35+ enterprise builds. 10+ industries. One loop:              ║
║   customer problem → architecture → production system.          ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

I'm a Forward Deployed Engineer who operates at the intersection of
**customer discovery, data architecture, AI integration, and full-stack engineering.**

I don't hand off to an engineering team. I am the engineering team — from the
first whiteboard session to the production deploy and the iteration after
the customer uses it for the first time.

---

## Selected Work

### Internal Platform Engineering

**[Professional Services Operations Platform](https://github.com/Concon8991/forward-deployed-operations-platform)**  
The operating system for an enterprise professional services organization.
Built from a 1,464-line spec I authored myself. Now in **v9+, live in production**,
serving 50–100+ employees across FDE, consulting, leadership, and operations roles.

Stack: React 19 + TypeScript + Vite + Tailwind + AppDB + Code Engine (7 functions) + DomoGPT + 22 datasets + 14 state collections. Seven personas, AI meeting prep synthesis, client/partner portals, immutable audit trail, Salesforce writeback via ETL, SPP timesheet automation.

One specific outcome: the weekly SPP timesheet process went from **20 minutes
of manual data entry to under 5 minutes**, replicated across every IC on the team.

---

### Enterprise Customer Delivery

**Aviation Capital Group — Automated Trading Tape Report Generator**  
ACG manages 100+ aircraft leases globally. Their team spent 3–4 hours per week
manually pulling data across 6+ views, copying into Excel, formatting per-aircraft
tabs. I automated this end-to-end: Jupyter workspace (44 datasets, Snowflake ODBC
integration, Domo Documents API, multi-environment dev→UAT→prod migration via Domo Sandbox).

One specific moment: the customer's director delivered a **same-day ultimatum**
on a critical Snowflake ODBC bug (1,024-character field truncation silently dropping
data). I diagnosed and resolved it in the same session. Senior stakeholders at
go-live called it "flooring." A trader requested a live pull before V1 was even released.

**Home Depot — AI Markup Pricing Tool**  
Built a complete **AI-driven salvage pricing recommendation system in under 24 hours**
for a Fortune 50 stakeholder demo. Inputs: 16.2M-row HDR scan dataset + Google BigQuery
inventory data. Output: AI-recommended markup percentages by department/class/subclass
with confidence scores and an approve/deny workflow that writes back to audit tables.
Stack: React + Domo Workflows (AI agent backend) + BigQuery cloud integration.

**Power BI Migration Tooling**  
Built a Power BI REST API automation script (Claude Code + REST client) that converts
Power BI dashboards to Domo App Studio. Used to migrate **~1,000 Power BI dashboards
for a previous customer in approximately one week.** Referenced as a competitive proof
point with multiple Fortune 500 accounts. At First Colony Mortgage, the executive
sponsor designated Domo as the company's sole reporting platform and began sunsetting
Power BI as a direct result of the migration engagement.

**Cox Farms — 73% Cloud Credit Reduction Program**  
Delivered a full Domo instance audit: 2,000+ orphaned datasets (feeding no cards),
22M duplicate rows across 55 datasets, one dataset at 126M rows with no clear owner.
Developed a function-by-function remediation plan and am executing the phased
bulk archival program. Projected outcome: 73% reduction in cloud computing credit
consumption by year-end.

---

### AI Agent Architecture

**[Scoob — Personal AI Operating System](https://github.com/Concon8991/scoob-ai-architecture)**  
A multi-agent AI system I designed and built to run my own FDE work.

```
175+ persistent memories
40 specialist agents (QA, security, data engineering, UX, workflow, etc.)
200+ MCP tools across Domo, GitHub, Slack, Teams, Snowflake, Linear
Continuous monitoring: email + Teams + SharePoint every 15 minutes
Shared knowledge lake (Compass) — shared with entire PS team
Automated session snapshots, retros, pattern promotion to team library
```

This isn't a chatbot. It's an autonomous operational intelligence layer that watches
my active customer accounts, surfaces signals, and executes work I would otherwise
have to do manually. It runs while I sleep.

Referenced in an internal team call as "auto-monitoring emails, Teams messages, and
SharePoint for [multiple customer accounts] every 15 minutes."

---

### AI / Data Pipelines

**[AI Support Intelligence Pipeline](https://github.com/Concon8991/ai-support-intelligence)**  
LLM pipeline for scoring and classifying support cases at scale.
Idempotent, throttled, structured-output-enforced. See the case study for
the engineering problems: chunking context across long case threads, token-bucket
throttling at 90K TPM, hash-based incremental re-runs, structured output
enforcement so downstream SQL queries don't break.

**[Customer Data Engineering Patterns](https://github.com/Concon8991/customer-data-engineering)**  
Production data pipeline failure modes and fixes from real engagements:
the silent row multiplication bug (financial delta: $40K undetected), the
memory failure that only appeared at production scale, the connector that
silently returned 98% of records, the federated query that shows 0 rows in the UI
but has 44K rows via API. The patterns I developed to prevent all of these.

---

## Industry Breadth

| Industry | What I Built |
|----------|-------------|
| Aviation / Leasing | Automated trading tape + per-aircraft reporting (Snowflake + Jupyter) |
| Retail / Home Improvement | AI salvage pricing + Power BI displacement |
| Construction | ECAC cost-at-completion modeling + S-curve project tracking |
| Mortgage / Finance | Turn time automation, AI chatbot, governance platform |
| Media / Broadcasting | Campaign performance + advertiser portal (Australia) |
| Nonprofit / Retail | AI document intelligence + multi-location operations |
| Consumer Brands | Demand forecasting, franchise analytics |
| Technology / SaaS | Agentic analytics, competitive displacement of ThoughtSpot + Snowflake Cortex |
| Enterprise IT | Vendor lifecycle management, contract risk flagging |
| Food & Beverage | 36M-row POS + delivery + e-commerce unified analytics |

---

## Strategic Contributions

**FDE AI-First Enablement Program (co-designer)**  
Co-designed and co-delivered the 2-day AI-first enablement program for Domo's
entire Professional Services delivery team — establishing the Pattern Library-first,
AI-native working model for the organization.

**Pattern Library Contributor**  
Active contributor to the team's shared engineering pattern library. Patterns
I developed on customer builds are promoted to the team library and used by
other FDEs on subsequent engagements.

**AI Center of Excellence**  
Member of the internal AI COE working group. Pitched and prototyped a cron-style
scheduling capability for autonomous customer account monitoring. Contributed
workflow skills to the shared team library.

**Customer Enablement (AEGM)**  
Trained a customer's internal team on building their own Claude Code plugin from
my Domo skill files. The customer adapted my patterns into an internal "Codex"
system used across their team — my work multiplied through another organization.

---

## How I Work

```
01  Start with the customer problem — not the technology
02  Understand the data (what exists, what's missing, what's wrong)
03  Design the smallest useful system
04  Build, ship, put it in users' hands
05  Measure what actually changed
06  Scale what works
07  Document what broke — that's the real institutional knowledge
```

I've run this loop across 35+ customer engagements in aviation, retail, healthcare,
construction, finance, media, nonprofits, and enterprise tech.

---

## Stack

**Languages:** Python · TypeScript · JavaScript · SQL

**Frontend:** React 19 · Vite · Tailwind CSS · Framer Motion · react-i18next

**Data:** Snowflake · BigQuery · Salesforce · Magic ETL · Jupyter · pandas · Domo

**AI:** LLM API integration · structured output · prompt engineering · multi-agent orchestration · MCP server configuration · DomoGPT

**Infrastructure:** REST APIs · OAuth · AppDB · Code Engine · Workflows (BPMN) · Domo Sandbox · Domo Everywhere embed · Documents API

**Tooling:** Claude Code · GitHub Actions · Power BI REST API · Domo Publish (multi-instance)

---

## Repos

| Repo | What it is |
|------|-----------|
| [forward-deployed-operations-platform](https://github.com/Concon8991/forward-deployed-operations-platform) | AI-native PS platform, v9+, production |
| [scoob-ai-architecture](https://github.com/Concon8991/scoob-ai-architecture) | Multi-agent AI operating system I built for myself |
| [ai-support-intelligence](https://github.com/Concon8991/ai-support-intelligence) | LLM pipeline for support case scoring |
| [customer-data-engineering](https://github.com/Concon8991/customer-data-engineering) | Production ETL patterns and failure modes |

---

*Open to the right opportunity — forward-deployed engineering, technical solutions
leadership, Head of FDE / Customer Engineering, or Director-level roles where
deep technical ownership and customer outcomes are the job.*

*[LinkedIn](https://linkedin.com/in/tom-occon) · tom.occon@gmail.com · Lehi, UT*
