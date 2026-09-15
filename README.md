# Tom Occon

**Forward Deployed Engineering · AI & Data Systems · Leadership**

Wellsville, UT · [LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tom.occon@gmail.com

---

At some point I realized that the most interesting problems at the intersection of technology
and business don't get solved by engineers who escalate to leaders, or by leaders who wait
for engineers. They get solved by someone who can do both and loves doing it.

That's what I've been building toward, deliberately, since I started in this industry.

I genuinely love leading teams toward outcomes they care about. I also love building the
systems that make those outcomes possible. I've been fortunate to spend my career in roles
where those two things aren't in conflict — where the best way to lead is to understand
the technical reality deeply enough to make the right call and then go build the thing that
proves it.

---

## How I Got Here

```
2022 · Sr. Technical Advisor, Preferred Support
  │
  │  Managing enterprise escalations and technical triage for
  │  Fortune 500 accounts. This is where I developed the customer
  │  instinct that drives everything I've built since.
  │
  ├─ Early 2024: Initiated an AI + NPS collaboration with Domo's
  │    product team on my own initiative as an individual contributor.
  │    I saw an opportunity, scoped it out, and brought it to the
  │    right people. Nobody asked me to. That's the pattern I've
  │    tried to follow ever since.
  │
  ↓
November 2024 · Promoted to Manager, Technical Support
  │
  │  Took over the West Coast Preferred Support team.
  │
  ├─ Co-led the Brilliance Bar at Domopalooza, Domo's annual
  │    customer conference. About 300 customer sessions across
  │    $78.6M in total ACV, 9.64/10 CSAT, 43% Director-level
  │    attendees. I helped frame it as an expansion opportunity,
  │    not just a support touchpoint. 60% of the customers we
  │    engaged were on lower support tiers.
  │
  ├─ Named co-lead for one of five AI initiatives formally
  │    prioritized by Domo's CCO across the support organization.
  │
  ├─ Authored an SME Program proposal and brought it directly
  │    to the VP and the full senior manager group. A structured
  │    program designed to build cross-functional subject matter
  │    experts with ties into Product, Engineering, and PS.
  │
  ├─ Built an AI-powered account review workflow using Domo's
  │    own platform and shared it with the Chief AI and Analytics
  │    Officer. He cited it in a company-wide executive brief
  │    to the CTO as a reference example of what was possible.
  │
  └─ December 2025: Advanced to an in-person interview with Domo's
       CCO for the VP, Support role. Thirteen months into management.
       That conversation meant a lot to me and clarified a lot about
       where I want to go.

May 2026 · Forward Deployed Engineer
  │
  │  Part of the CEO's initiative to double down on Domo's FDE motion.
  │  I was excited about the transition because it put me closer to
  │  the kinds of problems I love most: strategic accounts, ambiguous
  │  challenges, and the chance to build something meaningful fast.
  │
  ├─ In my first week, I led a customer demo that their analytics
  │    director described as the most impressive vendor meeting
  │    they'd experienced in a decade. Domo's CCO reached out
  │    personally: "May have heard YOU were the mastermind?"
  │
  ├─ "Tom is crushing it. The customer has said game changer
  │    more times than I can count." (Account executive, live
  │    from a high-stakes executive onsite)
  │
  ├─ Co-designed and delivered the AI-first enablement program
  │    for Domo's entire Professional Services delivery team.
  │
  ├─ 35+ enterprise customer builds across 10+ industries
  │    in the first four months.
  │
  └─ Built the internal operating system for Domo's Professional
       Services organization from scratch. It's in production
       at v9+, used by 50-100+ employees across the team daily.
```

---

## Selected Work

These aren't demos. They're the record of real problems I've been trusted to solve.

### The PS Ops Platform

**[Full Case Study](https://github.com/TomOccon/forward-deployed-operations-platform)**

I wrote the full specification, built the application, and have been iterating it
through nine major versions. It runs in production at Domo and is the primary
operational tool for the Professional Services team.

The reason I built it wasn't a mandate. I saw that the organization was running on
a combination of spreadsheets, Slack threads, and disconnected CRM data, and I had
a clear enough picture of what a well-designed operating system for a PS team should
look like that I decided to build it. That kind of decision has to come from a place
of caring about the org and understanding both the people side and the technical side.

What it replaced: 20-minute weekly timesheet entry processes (now under five minutes
per IC across the whole team), no visibility into engagement health, no systematic
AI-assisted preparation for customer meetings, and no client portal for external stakeholders.

Stack: React 19 · TypeScript · Vite · Tailwind · 22 datasets · 14 AppDB collections · Code Engine · DomoGPT

---

### Aviation Capital Group

ACG manages over 100 aircraft leases globally. Their team was spending three to four
hours each week manually pulling data from six different views and reformatting it
into per-aircraft Excel tabs.

I automated the entire process end-to-end using a Jupyter workspace connected to 44 datasets,
Snowflake ODBC integration, and a full multi-environment deployment from dev through UAT
to production.

The harder part of this story: midway through the engagement, the customer's director
presented me with a same-day deadline to resolve a critical Snowflake field truncation
bug I had never encountered before. I diagnosed it and resolved it in the same session.
At go-live, a trader submitted a live pull request before version one was even officially
released. Senior stakeholders called the whole experience "flooring."

---

### Home Depot

A Fortune 50 stakeholder demo with less than one business day to prepare. I built a
complete AI-driven salvage pricing recommendation system: 16.2 million rows of HDR scan
data combined with Google BigQuery inventory feeding AI-recommended markup percentages
by department, class, and subclass, with confidence scores and an approve/deny workflow
writing back to audit tables. The demo landed.

---

### Power BI Migration Tooling

I built automation using Claude Code and the Power BI REST API that converts Power BI
dashboards to Domo App Studio. I used it to migrate approximately 1,000 dashboards for
a prior customer in about one week.

At First Colony Mortgage, the executive sponsor designated Domo as the company's sole
reporting platform and started sunsetting Power BI. That's what competitive displacement
through execution looks like.

---

### Instance Governance: 73% Credit Reduction

I audited a customer's entire cloud analytics environment and found over 2,000 orphaned
datasets feeding nothing, 22 million duplicate rows across 55 datasets, and one dataset
sitting at 126 million rows with no clear owner. I built the remediation plan and am
currently executing it. The projected outcome is a 73% reduction in cloud computing
credit consumption by year-end.

---

### [Scoob: Personal AI Operating System](https://github.com/TomOccon/scoob-ai-architecture)

I designed and built a multi-agent AI system to run my own FDE work: 40 specialist agents,
175+ persistent memories, and over 200 tools spanning Domo, GitHub, Slack, Teams, Snowflake,
and Salesforce. It monitors multiple active customer accounts every 15 minutes and automatically
contributes patterns from my work to the team's shared knowledge base.

I built it because I believe one of the most important things a technical leader can do is
design systems that multiply their own judgment rather than just working harder. I wanted to
understand what that actually looks like in practice. This is my answer.

---

### [AI Support Intelligence Pipeline](https://github.com/TomOccon/ai-support-intelligence)

An LLM pipeline that transforms unstructured support cases into structured operational
intelligence: quality scores, root cause patterns, and sentiment trends across thousands
of cases. Includes real solutions to real engineering constraints around chunking, throttling,
and structured output enforcement.

---

### [Customer Data Engineering Patterns](https://github.com/TomOccon/customer-data-engineering)

A collection of production failure modes from real customer pipelines and the patterns that
prevent them. The silent row multiplication that caused a $40,000 financial discrepancy
with no error in the log. The connector that returned 98% of records and reported success.
The memory failure that only appeared at production data volume. The things that actually
matter when you're responsible for systems that people depend on.

---

## Industries I've Led Delivery In

Aviation · Retail · Mortgage · Construction · Media · Food and Franchise ·
Nonprofit · Enterprise SaaS · Enterprise IT · Professional Services

---

## How I Think About Leadership

Technical depth is credibility, not identity. I can go deep on architecture, data pipelines,
and AI systems, and that earns the right to be in the room. But it is not the reason to
be in the room.

The best leaders build leverage. I built Scoob so one person could monitor eight accounts
instead of one. I built the PS Ops platform so fifty people could operate better. I co-designed
the FDE enablement program because I wanted the whole team to level up, not just myself.
Every system I build reflects a decision about where to concentrate organizational leverage,
and those decisions feel more like leadership to me than anything else I do.

Outcomes are the only scoreboard. "The most impressive vendor meeting in a decade."
"Game changer more times than I can count." "Beyond brilliant." "You were the mastermind."
I keep those not because I need the recognition, but because they confirm that the judgment
behind the work was sound.

The trajectory I'm building is intentional. Individual contributor to manager to VP candidate
at thirteen months in to FDE on the most strategic accounts. Every step has been toward wider
scope, more organizational leverage, and closer to where strategy gets made. I'm working
toward C-suite leadership the way I approach every other goal: by earning it through delivery
and learning everything I can along the way.

---

## Stack

`Python` · `TypeScript` · `React 19` · `Vite` · `Tailwind CSS` · `SQL` · `pandas` ·
`Snowflake` · `BigQuery` · `Salesforce` · `Jupyter` · `Magic ETL` · `Claude Code` ·
`MCP` · `Domo` · `AppDB` · `Code Engine` · `Domo Workflows` · `LLM API integration` ·
`multi-agent orchestration`

---

*I'm looking for the right opportunity at a company where technical credibility and
business leadership are the same job, and where the path to the C-suite is earned
through delivering outcomes and building great teams.*

*[LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tom.occon@gmail.com*
