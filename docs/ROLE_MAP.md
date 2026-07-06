# 🎯 Role Map — From Portfolio to Job Applications

This maps each **target entry-level role** to the exact chains and projects that prove the skill, plus resume-bullet starters, an interview-prep checklist, and a suggested build order. Use it to decide what to build next based on the role you're applying for — and to talk about your work in interviews.

> Legend: ✅ strongly covered · 🟡 partially covered · 🎯 the chain that most directly targets this role
> Chains: **A** Java · **B** Banking/FinTech · **C** Full-Stack+Infra · **D** Data & ML Pipelines · **E** AI Products · **F** Systems from Scratch · **G** PropTech · **H** Business & Foundations · **I** Data-Eng Deep Dives · **J** Foundations/Qualify · **K** Hardware & Systems · **L** Cybersecurity · **M** Prompt AI & LLMs · **N** PropTech Engineering · **O** System Design · **P** MLOps · **Q** Data Analytics · **R** Data Science & Stats · **S** FinTech Engineering · **T** Interview Prep

---

## Software Engineer ✅

**Proof chains:** A (Java/OOP), C (full-stack, APIs, auth, deployment), F (from-scratch systems), J-01 (DSA), J-02 (git), **O** (system design 🎯), **T** (interview prep).

| Skill area | Prove it with |
|---|---|
| Language + OOP | A-1/A-2 (interfaces, ABCs), A-3 (Spring Boot) |
| APIs & full-stack | C-1 (FastAPI+React+JWT), C-3 (WebSockets) |
| Fundamentals | F-1 (HTTP from scratch), F-2 (interpreter), J-01 (DSA) |
| Scale & design | O-1…O-5 (system design), C-2/C-4 (Docker/K8s) |

**Resume bullet starters**
- Built a full-stack app (FastAPI + React + JWT) deployed with CI/CD and containerized services.
- Implemented an HTTP server and a language interpreter from scratch to demonstrate systems depth.

**Interview checklist:** DSA drills (T-1) · system design (T-2/O) · git workflow (J-02) · behavioral (T-4).
**Build order:** J-01 → A-3 → C-1 → O-1 → F-1.

---

## Data Engineer ✅ (portfolio core)

**Proof chains:** B (ETL, dbt, fraud), D (streaming, medallion, warehouse, IaC 🎯), I (SQL/dbt/Snowflake/Spark/Kafka/Airflow deep dives 🎯), P (MLOps).

| Skill area | Prove it with |
|---|---|
| Pipelines & ETL/ELT | B-1 (ETL+idempotency), I-02 (ETL/ELT), D-3 (medallion) |
| SQL & modeling | I-01 (SQL deep dive), B-2 (dbt medallion) |
| Warehousing | D-4 (Snowflake+dbt), I-03/I-04 |
| Streaming | D-2 (Kafka→Spark), I-06/I-07 |
| Orchestration & IaC | I-08 (Airflow), D-5 (data-platform IaC) |

**Resume bullet starters**
- Designed idempotent ELT pipelines (Python, dbt, Snowflake) with medallion layering and data-quality tests.
- Built a Kafka→Spark streaming pipeline with windowed aggregations and an audit-log pattern.

**Interview checklist:** SQL (T-3/I-01) · pipeline idempotency & SCD · warehouse modeling · system design (O).
**Build order:** I-01 → B-1 → B-2 → D-2 → D-4.

---

## Data Analyst 🟡 → 🎯 Chain Q

**Proof chains:** Q (Data Analytics 🎯), I-01 (SQL), I-10 (Tableau), B (business-adjacent data).

| Skill area | Prove it with |
|---|---|
| SQL for analysis | Q-1, I-01 |
| Spreadsheets/Excel | Q-2 |
| EDA in Python | Q-3 (pandas) |
| Dashboards & storytelling | Q-4, I-10 (Tableau) |
| Experiments & metrics | Q-5 (A/B testing, KPIs) |

**Resume bullet starters**
- Turned raw data into executive dashboards (Tableau) and communicated findings to non-technical stakeholders.
- Ran A/B tests and defined KPIs to quantify business impact.

**Interview checklist:** SQL joins/windows (T-3) · "explain this metric" · dashboard critique · case study.
**Build order:** Q-1 → Q-3 → Q-4 → Q-5.

---

## Data Scientist 🟡 → 🎯 Chain R

**Proof chains:** R (Data Science & Stats 🎯), D-1 (model serving), P (MLOps), I-01 (SQL), M (LLMs).

| Skill area | Prove it with |
|---|---|
| Statistics & probability | R-1 |
| EDA & feature engineering | R-2, R-3 |
| Modeling & evaluation | R-4, R-5 |
| Experimentation | R-5, Q-5 |
| Productionizing | D-1 (serving), P (MLOps) |

**Resume bullet starters**
- Built and evaluated ML models (scikit-learn) with rigorous train/test methodology and clear metrics.
- Served a trained model behind a FastAPI endpoint with monitoring.

**Interview checklist:** stats fundamentals · bias/variance · model evaluation · SQL (T-3) · a portfolio predictive project (R-6).
**Build order:** R-1 → R-2 → R-4 → R-5 → R-6 → D-1.

---

## FinTech (Engineer / Analyst) 🟡 → 🎯 Chain S

**Proof chains:** S (FinTech Engineering 🎯), B (banking data + fraud 🎯), D (pipelines), R (risk modeling).

| Skill area | Prove it with |
|---|---|
| Payments & ledgers | S-1 (Stripe/ACH), S-2 (double-entry) |
| Market data & trading | S-3 (backtesting) |
| Risk & fraud | S-4, B-2/B-3 (fraud signals) |
| Compliance | S-5 (KYC/AML) |

**Resume bullet starters**
- Built a double-entry ledger and a Stripe payments integration with idempotent transaction handling.
- Implemented fraud-signal scoring over a banking data platform (dbt medallion + window functions).

**Interview checklist:** money-handling correctness (idempotency, decimals) · fraud/risk reasoning · SQL · system design (O).
**Build order:** B-1 → B-2 → S-1 → S-2 → S-4.

---

## Adjacent roles (already well-covered)

| Role | Proof chains |
|---|---|
| **DevOps / Platform Engineer** | C-2 (Docker/Compose), C-4 (K8s+Terraform+Helm), J (cloud/IaC), K-6 (networking/firewalls), P (model CI/CD) |
| **ML Engineer** | D-1 (serving), P (MLOps 🎯), M (LLM apps/agents), R (modeling) |
| **Security Analyst (entry)** | L (defensive, simulation-based 🎯) |
| **AI/LLM Engineer** | M (🎯), E (AI products), P (ML infra) |

---

## How to use this map

1. **Pick a target role** for your next applications.
2. Build (or backfill) the 🎯 chain and the top 2–3 proof projects for that role first.
3. Pull the **resume bullets** into your CV, tailored to the job description.
4. Run the **Interview Prep chain (T)** track for that role before applying.
5. Every project already ships a lesson plan, an interactive tour + quiz, and a "Why This Matters (Industry Application)" section — use those as your talking points.

> This is a living document — update proof-project links as chains get built.
