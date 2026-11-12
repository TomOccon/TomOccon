# Tom Occon

**Director of Technical Customer Success · Enterprise Retention and AI Adoption**

Salt Lake City, UT · [LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tomoccon@gmail.com

---

Enterprise customers renew when the product starts running part of their business. I build the production AI and data systems that get it there, and I lead the technical customer teams that keep those accounts renewing and growing.

Currently a Senior Consultant in Professional Services at Progress Software (which acquired Domo in 2026). I carry Domo's enterprise AI delivery and MCP tooling through the integration, and I am building the project operating system that moves Professional Services from billing hours to managing margin across 150+ engagements in five delivery pods, India, data science and partner delivery. Before that, a founding Forward Deployed Engineer at Domo, where I delivered 50+ production AI and data builds for 25 enterprise accounts across 7+ industries in six months, ranked first on the team at 3x the peer average. Before that, I ran Domo's Preferred Support (Technical Account Management) program across North America West and APAC.

Customers I have built for: Sony Interactive Entertainment, The Home Depot, First Colony Mortgage, A+E Networks, ClarisHealth, The Walt Disney Company, and premium enterprise accounts across aviation, retail, financial services and media. Renewals as technical lead include Trimble ($1.15M) and Cosmo Energy ($799K expansion).

---

## What I Build

### Multi-agent AI systems and MCP servers

- **[Scoob](https://github.com/TomOccon/scoob-ai-architecture):** a multi-agent operating system for FDE work. 40 specialist agents, 175+ persistent memories, 200+ MCP tools, orchestrated through Claude Code with a delegation gate, effort routing and adversarial QA and security agents that are separate from the builders.
- **Custom MCP servers and LLM integrations** for Sony Interactive Entertainment and Home Depot, compressing implementation from months to days. The MCP tooling I built now ships in Domo's product as an out-of-the-box offering.
- **Databricks MCP server (43 tools):** Databricks ships managed MCP servers for SQL, Unity Catalog and Genie. I mapped the rest of the platform and built a Python server covering MLflow, Model Serving, Mosaic AI Vector Search, Lakebase, Delta Live Tables, compute lifecycle, governance grants, Databricks Apps and multi-workspace routing. Headless PAT auth, with graceful degradation for features a workspace's region does not have yet. Built in a single session on top of the Scoob toolset. The production server lives in an employer repo. **[mcp-server-patterns](https://github.com/TomOccon/mcp-server-patterns)** is a clean-room reference implementation of the same design (tool registry, multi-workspace routing, capability probing with graceful degradation, destructive-action gates, output caps) with 45 tests.

### LLM pipelines

- **[AI Support Intelligence Pipeline](https://github.com/TomOccon/ai-support-intelligence):** turns raw support cases and comment threads into structured scores: resolution quality, sentiment, root cause pattern, escalation risk, documentation gaps. Token-bucket rate limiting, retry with backoff, content-hash idempotency, overlapping chunking for long threads and strict JSON validation. Runs end to end with a stub client and 18 tests, and includes a root cause report. The same approach I used to run AI agents over 5,000+ case reviews and 169 root cause analyses.

### Data engineering

- **[Customer Data Engineering Patterns](https://github.com/TomOccon/customer-data-engineering):** production failures and the fixes that prevent them. A silent $40K row multiplication, a connector that reported success at 98% completeness, a join that fails only at production scale, and a service account that sees different data than the UI. Now ships as runnable checks (`dataguard`, 47 tests): reconciliation, join fanout detection, connector completeness, memory-bounded joins and a governance audit.
- **Instance governance:** audited 2,000+ orphaned datasets, 22M duplicate rows and a 126M-row dataset with no owner. Built the remediation plan, projecting a 73% reduction in cloud compute spend.
- **Aviation lease reporting:** automated 3-4 hours a week of manual Excel reformatting for a global aircraft lessor. Jupyter workspace over 44 datasets, Snowflake ODBC integration and dev to UAT to prod promotion through Domo Sandbox.
- **Fortune 50 retail pricing tool:** built in under 24 hours for a stakeholder demo. A 16.2M-row dataset and BigQuery feeding AI-recommended salvage pricing with confidence scores, plus an approve or deny workflow that writes back to audit tables.
- **Power BI migration tooling:** automation on Claude Code and the Power BI REST API that converts Power BI dashboards to Domo App Studio. Migrated about 1,000 dashboards for one customer in roughly a week. **[bi-migration-toolkit](https://github.com/TomOccon/bi-migration-toolkit)** is the clean-room version of the approach: inventory, triage into auto, assisted and manual waves, idempotent conversion and a readiness report.

### Internal platform

- **[PS Ops Platform](https://github.com/TomOccon/forward-deployed-operations-platform):** I wrote the 1,464-line spec and shipped 9+ versions. Used daily by 50-100+ Professional Services employees. Design decisions are in the [ADRs](https://github.com/TomOccon/forward-deployed-operations-platform/tree/main/docs/adr). Weekly time entry dropped from 20 minutes to under 5. React 19, TypeScript, Vite, Tailwind, 22 datasets, 14 AppDB collections, Code Engine and DomoGPT with rule-based fallbacks.

---

## Claim to Evidence

| What my resume says | Where to see how it was done |
|---|---|
| 50+ production AI builds for 25 accounts in 6 months, 3x peer output | [Scoob](https://github.com/TomOccon/scoob-ai-architecture): delegation gate, ADRs, [AI-first delivery framework](https://github.com/TomOccon/scoob-ai-architecture/blob/main/docs/ai-first-delivery-framework.md) |
| Custom MCP servers and LLM integrations; MCP tooling now ships in Domo's product | [mcp-server-patterns](https://github.com/TomOccon/mcp-server-patterns) |
| AI agents for 5,000+ case reviews and 169 RCAs | [ai-support-intelligence](https://github.com/TomOccon/ai-support-intelligence) |
| Added tickets and escalations to the health score; renewal forecasting extended to 18 months | [account-health-and-renewal-forecasting](https://github.com/TomOccon/account-health-and-renewal-forecasting): health score, backtest, 18-month forecast, at-risk triage |
| About 1,000 Power BI dashboards migrated in about a week | [bi-migration-toolkit](https://github.com/TomOccon/bi-migration-toolkit) |
| Instance governance audit, 73% projected compute reduction | [customer-data-engineering](https://github.com/TomOccon/customer-data-engineering): `dataguard.governance` |
| Silent row multiplication, connector completeness, join failures | [customer-data-engineering](https://github.com/TomOccon/customer-data-engineering) |
| Internal PS platform, 9+ versions, 50-100+ daily users | [forward-deployed-operations-platform](https://github.com/TomOccon/forward-deployed-operations-platform) and its [ADRs](https://github.com/TomOccon/forward-deployed-operations-platform/tree/main/docs/adr) |

The code in these repos is clean-room: synthetic data, no customer or employer code. The forecasting backtest uses a generator with the signal built in, so it demonstrates the method and is not a claim about real customer results.

---

## Technical Skills

**AI:** Multi-agent systems · MCP (Model Context Protocol) · LLM integration · Prompt engineering · Claude Code · OpenAI · GitHub Copilot

**Languages and web:** Python · SQL · TypeScript · React 19 · Vite · Tailwind CSS · pandas · Jupyter

**Data platforms:** Domo (Major Domo certified) · Snowflake · BigQuery · Databricks (Unity Catalog, Delta Lake, MLflow) · Power BI · Magic ETL · AppDB · Code Engine · Workflows

**Business systems:** Salesforce · Gong · Jira · Zendesk

---

## Technical Customer Success Leadership

Engineering depth is what lets me lead technical customer teams credibly.

| Result | Detail |
|---|---|
| Team | Led a 42-person Preferred Support (TAM) team across 5 regions and 306 accounts: 11 direct reports including managers in Japan and India, 28 advisors; built the India team from zero through 200+ interviews; first response cut from 6.15 hours to about 1 |
| Service quality | 98.9% SLA vs 97.9% global, 9.14 CSAT vs 8.96, 14.0 days to close vs 19.5, 458 vs 408 cases per advisor |
| Retention | 136% NRR and 99.9% dollar renewal on 53 premium accounts, and 93.3% dollar renewal vs 79.8% for the rest of Domo. 78 at-risk renewals won with 1 loss ($33.3M renewed) as technical lead |
| Forecasting | Extended renewal forecasting from 2 quarters to 18 months out; co-led quarterly post-sales strategy with the CCO |
| Voice of the customer | Raised 492 engineering issues affecting 500+ accounts ($86.5M+ in annual revenue) and 122 enhancement requests from 81 accounts; 17 of 21 product changes delivered |
| Executive engagement | Co-led the Brilliance Bar at Domopalooza (~5,000 attendees): 300+ executive appointments tied to $78.6M in ACV, $41.3M in tier upgrades surfaced |
| Enablement | Trained the 35-person consulting organization (20 pod consultants, 5 data scientists, 10+ India reps) on the AI-first delivery framework, proving each pattern in one engagement before the group adopts it; trained a customer's CEO and full C-suite onsite as they made Domo their only reporting platform |

## Experience

| Role | Dates | Highlights |
|---|---|---|
| Senior Consultant, Professional Services, **Progress Software** | Sep 2026 - Present | Margin operating system across 150+ engagements; AI-first delivery training for 35 people; continuity of Domo enterprise AI builds and MCP tooling through the acquisition |
| Founding Forward Deployed Engineer, **Domo** | May 2026 - Sep 2026 | 50+ production AI and data builds for 25 accounts, ranked first at 3x peer average; MCP servers and LLM integrations for Sony and Home Depot; a $1M Home Depot expansion positioned |
| Technical Support Manager, North America West and APAC, **Domo** | Dec 2024 - May 2026 | Ran Preferred Support (TAM); 136% NRR on 53 premium accounts; 42-person team; finalist for VP of Support from 2,000+ applicants |
| Senior Technical Advisor, **Domo** | Nov 2022 - Dec 2024 | 1,200+ complex cases across 306 accounts (~$79M ARR); #3 of 22 for resolution speed; 492 engineering issues raised |
| Sales Operations Manager, **Fox Pest Control** | Feb 2021 - Nov 2022 | Revenue operations and Power BI analytics for 80+ reps and $4M+ ARR; infrastructure behind a $360M acquisition |
| Regional Manager, **Fox Pest Control** | Sep 2019 - Feb 2021 | Ran 52 people across three branches; churn under 1% vs a 5% company average |
| Chief Operating Officer, **Sure Systems Group** | Jul 2018 - Sep 2019 | Operations, books, payroll and multi-state tax for a ~$2M, 6-state business; P&L reporting for the owner |

**Education and certifications:** MBA, IT Management (Western Governors University, 2026) · BS, IT Management (WGU, 2025) · Major Domo certification (Domo, 2022; earned in 1 week against a standard 8-week track) · Certificate, Strategic Thinking and Innovation (WGU)

**Languages:** Portuguese (native), Dutch and Flemish (professional), French, Spanish. Lived in Brazil, the Netherlands and France.

---

*[LinkedIn](https://www.linkedin.com/in/tom-occon-06563a193/) · tomoccon@gmail.com*
