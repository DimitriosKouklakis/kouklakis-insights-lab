# Kouklakis — Insights Lab

I turn messy data into stories people can act on.  
Think of this repo as my **BI & Analytics atelier**: blueprints, dbt/SQL models, and Tableau designs that turn **KPIs → decisions**.

> 🎨 Data artist with a product mindset — equal parts SQL/Python/Tableau and clarity, coaching, and calm under pressure.

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
