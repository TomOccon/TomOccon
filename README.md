# Tom Occon

**Forward Deployed Engineer · AI & Data Systems**

Lehi, UT · [LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tom.occon@gmail.com

---

I build things that actually change how people work.

Not dashboards that sit on a page. Systems that replace a 3-hour manual process,
that flag the account that's about to churn before the CSM calls, that let an aircraft
trader pull a live portfolio report instead of copying data into Excel for 4 hours.

That's the job. And I love it.

---

## The Career Arc That Got Me Here

```
2022–2024 · Sr. Technical Advisor, Preferred Support
  │
  ├─ January 2024: Initiated a cross-functional AI project with Domo's
  │    product team to apply OpenAI to NPS sentiment analysis in Support.
  │    I was still an individual contributor. Nobody asked me to do this.
  │
  └─ Managing enterprise escalations, onboarding, and technical triage
       for Fortune 500 Preferred Support accounts.

November 2024 · Promoted to Manager, Technical Support
  │
  ├─ Took over the West Coast Preferred Support team.
  │
  ├─ April 2025: Named co-lead for one of five AI initiatives
  │    formally prioritized by Domo's CCO for the support organization.
  │
  ├─ June 2025: Authored and circulated an SME Program proposal
  │    directly to the VP and all senior support managers —
  │    a cross-functional program designed with Product, Engineering,
  │    and Professional Services integration.
  │
  ├─ December 2025: Advanced to an in-person interview with Domo's CCO
  │    for the VP, Support role — 13 months after becoming a manager.
  │
  ├─ Co-led Domopalooza Brilliance Bar:
  │    ~300 customer appointments · $78.6M total ACV engaged
  │    9.64/10 CSAT · 81% perfect scores · 43% Director-level+
  │    VP of Technical Support: "You set the tone... your leadership
  │    elevated what we accomplished together."
  │
  └─ Built AI account review workflow → Chief AI Officer cited it
       to the CTO in a company-wide executive brief.

May 2026 · Forward Deployed Engineer
  │
  ├─ Week one: drove a customer demo that made an analytics director
  │    write "Easily the most impressed I've been coming out of a vendor
  │    meeting in the decade I've been doing this." The VP of PS called
  │    it out on the executive staff thread personally.
  │    CCO texted: "May have heard YOU were the mastermind?"
  │
  ├─ "Tom is crushing it... The customer has said game changer
  │    more times than I can count." (AE live from high-stakes onsite)
  │
  ├─ 35+ enterprise builds in the first 4 months
  │
  └─ Built the internal operating system for Domo's entire
       Professional Services organization (v9+, 50-100+ users)
```

---

## What I've Built

### The PS Ops Platform — Internal Production App

**[→ Case Study](https://github.com/Concon8991/forward-deployed-operations-platform)**

I wrote a 1,464-line spec, then built it. Now it's in **v9+ in production**
serving 50-100+ Domo PS employees. This is not a prototype.

What it does: engagement tracking, resource capacity planning, AI-synthesized
meeting prep from Gong transcripts, live AI account intelligence, client portal
with external persona isolation, full audit trail, Salesforce writeback via ETL,
automated SPP timesheets.

One metric: the weekly timesheet prep process went from **20 minutes of manual
work to under 5 minutes** — for every IC on the team.

Stack: React 19 · TypeScript · Vite · Tailwind · 22 datasets · 14 AppDB collections · Code Engine · DomoGPT

---

### Aviation Capital Group — Trading Tape Automation

ACG manages 100+ aircraft globally. Their team was spending 3-4 hours per week
manually pulling data across 6 views and reformatting it into Excel.

I automated all of it: Jupyter workspace (44 datasets), Snowflake ODBC integration,
multi-environment deployment (dev→UAT→prod via Domo Sandbox), full user playbook.

Midway through the project, the customer's director gave me a same-day deadline to
fix a critical Snowflake field truncation bug I'd never seen before. I fixed it same session.
At go-live, a trader requested a live pull before V1 was even released.
Senior stakeholders called it "flooring."

---

### Home Depot — AI Markup Pricing Tool (Built in Under 24 Hours)

**For a Fortune 50 stakeholder demo.** I had less than one business day.

I built a complete AI-driven salvage pricing recommendation system: 16.2M-row
HDR scan dataset + Google BigQuery inventory → AI-recommended markup percentages
by department/class/subclass with confidence scores + approve/deny workflow that
writes back to audit tables.

It worked. The demo landed.

---

### Power BI → Domo Migration Tooling

I built a Power BI REST API automation script using Claude Code that converts
Power BI dashboards to Domo App Studio. I used it to migrate ~1,000 Power BI
dashboards for one customer in approximately one week.

At First Colony Mortgage, the executive sponsor used it as the reason to
designate Domo as the company's sole reporting platform and start sunsetting Power BI.

---

### Instance Governance — 73% Credit Reduction Program

I audited a customer's entire cloud analytics environment. Found: 2,000+ orphaned
datasets, 22M duplicate rows across 55 datasets, one dataset at 126M rows with no
clear owner.

I built the remediation plan and am executing it. Projected outcome: 73% reduction
in cloud computing credit consumption by year-end.

---

### [AI Support Intelligence Pipeline](https://github.com/Concon8991/ai-support-intelligence)

An LLM pipeline for scoring and classifying support cases at scale.

The engineering problems that actually matter: how do you preserve context across
a 40-turn case thread when it won't fit in a single LLM call? How do you score
10,000 cases without blowing through rate limits? How do you make the pipeline
re-runnable without re-processing already-scored cases?

All of that is solved in this repo, with real code.

---

### [Scoob — My Personal AI Operating System](https://github.com/Concon8991/scoob-ai-architecture)

I built a multi-agent AI system to run my own FDE work.

175+ persistent memories across 4 typed categories. 40 specialist agents. 200+ MCP
tools. Continuous monitoring of email + Teams + SharePoint across active customer
accounts. The whole thing automatically shares patterns to a knowledge lake used
by the entire PS team.

It monitors multiple customer accounts every 15 minutes while I'm doing other things.
That's not an exaggeration.

---

### [Customer Data Engineering Patterns](https://github.com/Concon8991/customer-data-engineering)

Production failures from real customer pipelines — and the patterns that prevent them.

The silent row multiplication ($40K financial delta, no error in the log). The memory
failure that only showed up at production data volume. The connector that returned
98% of records and called it success.

These are the things that separate a reliable system from a demo that breaks
the third time someone runs it.

---

## Industries I've Built In

| Industry | What I Delivered |
|----------|-----------------|
| Aviation / Asset Leasing | Automated trading tape · Snowflake integration · multi-env deployment |
| Retail / Home Improvement | AI pricing engine · BigQuery integration · Fortune 50 delivery |
| Mortgage / Financial Services | Turn time automation · AI chatbot · Power BI displacement |
| Construction / Engineering | ECAC cost-at-completion modeling · S-curve project tracking |
| Media / Broadcasting | Campaign performance platform · advertiser portal |
| Food & Franchise | 36M-row POS + delivery + e-commerce unified analytics |
| Nonprofit / Retail | AI document intelligence · multi-location data intake |
| Enterprise SaaS | Agentic analytics · competitive displacement of ThoughtSpot + Snowflake Cortex |
| Enterprise IT | Vendor lifecycle management · contract risk intelligence |
| Professional Services | Full PS operating system · capacity planning · AI synthesis |

---

## Beyond Building

**Domopalooza Brilliance Bar Co-Lead**
Co-led all on-site support operations at Domo's annual customer conference.
~300 customer appointments. $78.6M total ACV engaged. 9.64/10 CSAT.
43% Director-level or above. 60% of engaged customers were on lower tiers —
we turned the event into a live expansion pipeline.

**FDE Enablement Program (Co-Designer)**
Co-designed and delivered the 2-day AI-first training program for Domo's
entire Professional Services delivery team. Established the methodology every
FDE now uses.

**Product Influence**
Championed an AI readiness tool to Domo's Chief AI Officer. It got evaluated
at the SVP Product level for the formal roadmap. I was an IC at the time.

**Pattern Library Contributor**
Patterns I build on customer engagements go into the team's shared library.
Other FDEs use them on the next build.

---

## Stack

`Python` · `TypeScript` · `React 19` · `Vite` · `Tailwind CSS` · `SQL` · `pandas` ·
`Snowflake` · `BigQuery` · `Salesforce` · `Jupyter` · `Magic ETL` · `Claude Code` ·
`MCP` · `Domo` · `AppDB` · `Code Engine` · `Domo Workflows` · `LLM API integration` ·
`multi-agent orchestration`

---

*Looking for the right opportunity — forward-deployed engineering, technical solutions
leadership, Head of FDE / Customer Engineering. Roles where you're judged by what
changes for customers, not how many meetings you attend.*

*[LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tom.occon@gmail.com*
