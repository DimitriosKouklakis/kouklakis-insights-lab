# Welcome to Kouklakis — Insights Lab!

[<img width="30" height="30" alt="image" src="https://github.com/user-attachments/assets/9f871b3e-56bd-46e1-b355-09e16283346f" />
](https://www.linkedin.com/in/dimitris-kouklakis/)\[<img width="30" height="30" alt="image" src="https://github.com/user-attachments/assets/fb0ea658-f3d3-460f-a0a9-e561f080a123" />](https://public.tableau.com/app/profile/dimitrios.kouklakis/vizzes)


>I turn messy data into stories people can act on.  
>Think of this repo as my **BI & Analytics atelier**: blueprints, SQL models, and Tableau designs that turn **KPIs → decisions**.

🎨 Data artist with a product mindset — equal parts SQL/Python/Tableau and clarity, coaching, and calm under pressure.

**What I love**

+ ✅ Designing KPIs as a shared language (so Finance, Product & Ops finally agree 😉)
+ 📊 Building reliable dashboards that execs actually use
+ 🔁 Moving teams from “ad-hoc” to repeatable: templates, QA gates, RLS, clear SLAs

**How I work**

+ **🎯 Outcomes > outputs**: I start with the decision, not the chart
+ **🍸 Governance with taste:**
+ - One source of truth
+ - RLS
+ - Data Governance & Security Protocols
+ - Group Permissions
+ - Clean Reporting Repo
+ **🤝 Human first**: I coach, unblock, and give people room to grow, building elite professional squads

>**Stack:**
Tableau • SQL • Python • Databricks • PostgreSQL • JIRA • Confluence • Figma

Got a messy dataset, a slippery KPI, or a dashboard no one opens?
Let’s turn it into something people use. 
I’m open to smart collabs—audits, exec dashboard makeovers, KPI/glossary tune-ups, data migrations, or quick BI strategy sparring. 
Contact me today and let’s make your data sing, taking decision-making to the next level and compounding your org’s prosperity.

📩 dim.kouklakis@gmail.com

---

## What’s inside
- **Case studies**: Problem → Decision → Approach → Impact → Reusable pattern
- **Analytics-ready models**: dbt/SQL marts with tests & docs
- **Dashboard specs**: Executive Pulse, Financial Performance, Acquisition Overview (design, RLS, calc catalog)
- **Governance**: KPI glossary, QA gates, RLS patterns, naming conventions
- **Synthetic data**: generators + CSV/Parquet so you can reproduce locally

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
