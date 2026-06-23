# 🗺️ Chain Map

A visual map of all chains and their dependencies. **Solid arrows (`──▶`) are code dependencies** (one repo's output feeds the next). **Dashed arrows (`╌╌▶`) are skill dependencies** (no shared code, just assumed knowledge).

```
CHAIN A — Java Mastery (skill chain)
  Farmer-Froilan-Java ╌╌▶ Farmer-Froilan-Python ╌╌▶ Spring-Boot-REST-API ╌╌▶ Entrada-Clone
        (OOP/interfaces)      (ABCs/Protocols)        (Spring/JPA/JWT)        (full-stack capstone,
                                                                              also Chain G capstone)

CHAIN B — Banking + FinTech (CODE dependency chain)
  Web-Scraper-Postgres-Pipeline ──▶ Banking-Data-Platform ──▶ Banking-Interface-Fraud-UI
        (ETL → Postgres)               (dbt medallion: Bronze       (Spring @Entity maps the
                                        → Silver → Gold)             Gold tables; React renders them)

CHAIN C — Full-Stack + Infrastructure (CODE dependency chain)
  Full-Stack-Job-Board ──▶ Dockerized-Microservices ──▶ Ops-Management-Dashboard ──▶ Kubernetes-IaC-Deployment
        (FastAPI+React)         (containerize it)            (add WebSockets/RBAC)        (ship to K8s, from scratch)

CHAIN I — Data Engineering Deep Dives (independent skill repos)
  SQL ─ ETL/ELT ─ dbt ─ Snowflake ─ Azure ─ Spark ─ Kafka ─ Airflow ─ Teradata ─ Tableau ─ Django/Flask
        (each stands alone; recommended grouping: SQL→ETL→dbt, then Spark→Kafka→Airflow)

CHAIN J — Just Enough to Qualify (skill + mini-projects)
  DSA-OOP ─ Git-Workflow ─ AI-Augmented-Dev ─ Cloud-AWS ─ Cloud-Azure ─ Networking ─ IaC-Terraform
        Cloud-AWS ╌╌▶ Networking ╌╌▶ IaC-Terraform  (Terraform capstone ties the chain together)

CROSS-CHAIN REINFORCEMENT
  J-06 IaC-Terraform        ╌╌▶ C-4 Kubernetes-IaC-Deployment   (fundamentals → real cluster)
  J-04b Cloud-Azure  +  I-05 Azure-Data-Stack                  (platform ↔ data services)
  I-01 SQL + I-03 dbt       ╌╌▶ B-2 Banking-Data-Platform        (theory → applied)

RESERVED
  #30 (to be selected)  +  Chains D–H  ── drawn from: CLI Task Manager, HTTP Server,
  ML Serving API, Custom Language Interpreter, BD/Marketing CRM, Streaming Pipeline,
  Databricks ETL, AI TTS+Notes, Social Media Manager, Leasing App, AI Agent
```

## Build-Order Quick Reference

| Phase | Months | Projects |
|-------|--------|----------|
| 1 — Foundations | 1–2 | A-1, A-2, B-1, J-01 |
| 2 — Core Stack | 3–5 | A-3, C-1, C-2, J-02 |
| 3 — Data Engineering | 5–8 | B-2, B-3, I-01→I-03, I-06→I-08 |
| 4 — Infrastructure | 7–10 | C-3, C-4, J-04a/b, J-05, J-06 |
| 5 — Capstones | 9–12 | A-4, I-04/05/09/10/11, J-03 |
