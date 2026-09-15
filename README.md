# Tom Occon

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║   FORWARD DEPLOYED ENGINEERING                                   ║
║   AI  ·  DATA SYSTEMS  ·  CUSTOMER SOLUTIONS                    ║
║                                                                  ║
║   I turn ambiguous customer problems into production systems.    ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

Most engineers build software. I build the bridge between a customer's
operational reality and a system that actually changes how they work.

That means I've spent years at the intersection of: **customer discovery →
data architecture → application engineering → AI integration → measurable
outcome.** And I've shipped all of it myself—from the first whiteboard to
the production deploy.

---

## Selected Systems

| System | Domain | What It Demonstrates |
|--------|--------|----------------------|
| [AI Support Intelligence](#-ai-support-intelligence) | AI · Data Engineering | LLM pipelines at operational scale |
| [Professional Services Platform](#-professional-services-platform) | Product · Full-Stack | AI-native operational software, v9+ |
| [Customer Data Reliability](#-customer-data-engineering) | Data Engineering | Production ETL, failure modes, real fixes |
| [Forward-Deployed AI Patterns](#-forward-deployed-ai-patterns) | AI · Architecture | Reusable patterns for FDE/solutions work |

---

## AI Support Intelligence

**Repo:** [`ai-support-intelligence`](https://github.com/Concon8991/ai-support-intelligence)

> Turn unstructured support case data into a repeatable operational intelligence system.

Support organizations accumulate thousands of cases. None of it is machine-readable by default—it lives in free-text comments, inconsistent severity tags, and agent notes written under pressure. This project is a pipeline that changes that.

**What it does:**

- Ingests raw support case data (Salesforce Cases + comment threads)
- Runs structured AI analysis per case: root cause hypothesis, quality score, customer sentiment, resolution pattern classification
- Outputs a normalized dataset consumable by any BI tool
- Designed around real constraints: token limits, API throttling, cost efficiency, idempotent re-runs

**Architecture:**

```
Salesforce Cases + Comments
        │
        ▼
  Data Preparation
  (dedup · filter · chunk)
        │
        ▼
  LLM Analysis Layer
  (batch · throttle · retry)
        │
        ▼
  Structured Scoring
  (quality · sentiment · root cause · pattern)
        │
        ▼
  Output Dataset
        │
        ▼
  Analytics / Operational Dashboards
```

**Technologies:** Python · pandas · SQL · Jupyter · Domo · LLM APIs

**Engineering challenges I actually solved:**
- Chunking long case threads without losing context across turns
- Throttling LLM calls to stay within rate limits while maximizing throughput
- Making the pipeline re-runnable without re-processing already-scored cases
- Structured output enforcement so downstream SQL queries don't break

[→ Full case study](https://github.com/Concon8991/ai-support-intelligence)

---

## Professional Services Platform

**Repo:** [`forward-deployed-operations-platform`](https://github.com/Concon8991/forward-deployed-operations-platform)

> The operating system for a Forward Deployed / Professional Services organization.

When I looked at how PS teams actually operate—managing customer engagements,
tracking delivery health, coordinating resources, surfacing risk—I saw a gap
that no off-the-shelf tool fills cleanly. CRMs track pipeline. Project tools track tasks.
Neither understands the specific operational reality of an FDE team delivering technical
outcomes for strategic accounts.

So I built it.

**What it is:**

A full-stack React application (v9+, production) with:

- **Portfolio view** — real-time engagement health index across all active accounts
- **Engagement workspace** — delivery tracking, milestones, risk surface, EVM
- **Meeting Prep AI** — Gong call data + pending tasks → AI-synthesized briefing document
- **Time & resource management** — logged hours, capacity planning, utilization by role
- **Client portal** — external persona with tailored engagement visibility
- **Command Center** — practice-wide capacity, needs-attention queue, strategic account tracking
- **AI-native throughout** — DomoGPT integration for account intelligence, meeting prep synthesis, anomaly explanations
- **Admin surface** — configurable per-org with toggles, persona maps, master data

**Architecture decisions:**

```
┌─────────────────────────────────────────┐
│              React + Vite + TS           │
│         Tailwind · Framer Motion         │
├─────────────────────────────────────────┤
│         Service Layer (CE functions)     │
│   computeCapacity · recordChange ·       │
│   logTime · extractSOW · sppSync         │
├─────────────────────────────────────────┤
│            Data Layer (22 datasets)      │
│   Salesforce · SPP · Gong · HG · ETL    │
├─────────────────────────────────────────┤
│          State (14 AppDB collections)    │
│   Audit · Config · Historical · Metrics  │
└─────────────────────────────────────────┘
```

**Personas:** `technical_ic` · `engagement_owner` · `scoping_team` · `leader` · `admin` · `csm` · `client`

Each persona gets a different view of the same underlying data—enforced at the application layer, not just via CSS visibility.

**What I'd build next:**
- Native mobile (the current web-responsive approach works, but a true mobile-first client portal deserves its own surface)
- Real-time collaborative editing on engagement plans (currently last-write-wins on overlapping AppDB writes)
- ML-based engagement risk scoring (current risk surface is rule-based; the training data is now large enough to train a real model)

[→ Full case study](https://github.com/Concon8991/forward-deployed-operations-platform)

---

## Customer Data Engineering

**Repo:** [`customer-data-engineering`](https://github.com/Concon8991/customer-data-engineering)

> Real-world data pipeline patterns. Things that break. How to fix them.

Most portfolio projects work in ideal conditions. This one documents what happens when:

- A join produces the wrong row count and you don't find out until a finance team flags a $40K discrepancy
- A dataflow succeeds in test but fails in production with `Join inner did not fit in memory`
- A connector silently truncates a field due to a regex pattern mismatch
- A Snowflake federated query shows 0 rows in the UI but has data (and the fix is non-obvious)
- An ETL fan-out bug causes a metric to be double-counted across date × reason combinations

These are real failures from real production pipelines. The patterns I developed to avoid them are worth more than any clean demo.

**Documented patterns:**

- SQL dialect constraints (what the docs don't mention until it breaks)
- Join key cardinality limits and when they silently corrupt results
- Multi-source fan-out bugs and how to detect them with row count assertions
- Structured ETL testing before connecting to production data
- Magic ETL: native tiles vs SQL tiles (and why the choice matters for customer maintainability)
- Connector state management across credential rotations

**Technologies:** SQL · Python · pandas · Magic ETL · Snowflake · Salesforce · Domo

[→ Full case study](https://github.com/Concon8991/customer-data-engineering)

---

## Forward-Deployed AI Patterns

> Patterns I've developed for embedding AI into customer-facing operational workflows.

These aren't tutorials. They're documented decisions from shipping AI features into
production systems used by real teams.

**Topics:**
- AI meeting prep: using call transcripts + task data to generate pre-meeting briefs
- Structured LLM output for downstream SQL queries
- When rule-based logic beats an LLM (and the cost of getting that wrong)
- Client-facing AI: what to show, what to hide, what to never let the model say
- Account intelligence: grounding LLM output in structured signals to avoid hallucinations in high-stakes contexts

---

## How I Work

```
01  Start with the customer problem — not the technology
02  Understand the data (what exists, what's missing, what's wrong)
03  Design the smallest useful system
04  Ship something into users' hands
05  Measure what actually changed
06  Scale what works
07  Document what broke along the way — that's the real IP
```

I've done this across support operations, professional services, marketing analytics,
logistics, and financial services. The domain changes. The loop doesn't.

---

## Background

**Current:** Forward Deployed Engineer, Domo — building AI-native operational applications
for enterprise customers across multiple industries.

**Before that:** Support engineering, customer success, technical consulting.
The through-line is always: *technical depth in service of customer outcomes.*

---

## Stack

**Languages:** Python · TypeScript · JavaScript · SQL

**Frameworks:** React · Vite · pandas · Tailwind CSS · Framer Motion

**Data:** Snowflake · Salesforce · Magic ETL · Domo · Jupyter

**AI:** LLM API integration · structured output · prompt engineering · embedding pipelines

**Infrastructure:** REST APIs · OAuth · MCP · Code Engine · Workflows · AppDB

---

*Available for the right opportunity — particularly forward-deployed engineering,
technical solutions leadership, or Head of FDE/Customer Engineering roles.*

*Reach out: [LinkedIn](https://linkedin.com/in/tom-occon) · tom.occon@gmail.com*
