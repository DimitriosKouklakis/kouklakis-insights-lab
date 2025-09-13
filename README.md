# Kouklakis — Insights Lab

I turn messy data into stories people can act on.  
Think of this repo as my **BI & Analytics atelier**: blueprints, SQL models, and Tableau designs that turn **KPIs → decisions**.

> 🎨 Data artist with a product mindset — equal parts SQL/Python/Tableau and clarity, coaching, and calm under pressure.
> **What I love**
✅ Designing KPIs as a shared language (so Finance, Product & Ops finally agree 😉)
📊 Building reliable dashboards that execs actually use
🔁 Moving teams from “ad-hoc” to repeatable: templates, QA gates, RLS, clear SLAs

**How I work**
🎯 Outcomes > outputs — I start with the decision, not the chart
🍸Governance with taste: one source of truth, group permissions, clean repo
🤝 Human first: I coach, unblock, and give people room to grow

**Stack**
SQL • Python • Tableau • Databricks • JIRA • Confluence

Got a messy dataset, a slippery KPI, or a dashboard no one opens?
Let’s turn it into something people use. 
I’m open to smart collabs—audits, exec dashboard makeovers, KPI/glossary tune-ups, data migrations, or quick BI strategy sparring. 
📩 DM me and let’s make data sing—taking decision-making to the next level and compounding your org’s prosperity.

Still learning every day, still curious. 
If you like data that changes behavior, let’s connect.

---

## What’s inside
- **Case studies**: Problem → Decision → Approach → Impact → Reusable pattern
- **Analytics-ready models**: dbt/SQL marts with tests & docs
- **Dashboard specs**: Executive Pulse, Financial Performance, Acquisition Overview (design, RLS, calc catalog)
- **Governance**: KPI glossary, QA gates, RLS patterns, naming conventions
- **Synthetic data**: generators + CSV/Parquet so you can reproduce locally

## Screens (teaser)
<img src="assets/exec_pulse.png" width="420"> <img src="assets/financial_perf.png" width="420">

---

## Quickstart (local)
```bash
# 1) spin up Postgres + dbt docs
docker compose up -d

# 2) seed + build
make db-seed    # or: psql -f ops/init.sql
make dbt-build  # dbt build && dbt docs generate

# 3) open docs
make dbt-docs   # opens dbt lineage/docs in your browser
