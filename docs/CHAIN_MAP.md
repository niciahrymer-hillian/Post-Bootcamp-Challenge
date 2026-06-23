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

CHAIN D — Data & ML Pipelines (skill chain)
  ML-Model-Serving-API ╌╌▶ Streaming-Data-Pipeline ╌╌▶ Databricks-Medallion-ETL

CHAIN E — AI Products (skill chain)
  AI-TTS-Notes ╌╌▶ AI-Social-Media-Manager ╌╌▶ AI-Agent-Assistant

CHAIN F — Systems & Languages (from scratch, no scaffolding)
  HTTP-Server-From-Scratch ╌╌▶ Custom-Language-Interpreter

CHAIN G — PropTech
  Leasing-Agent-App   +   Entrada-Clone (shared capstone, lives in Chain A)

CHAIN H — Business & Foundations
  CLI-Task-Manager (foundations starter)   +   BD-Marketing-CRM
```

## Build-Order Quick Reference

| Phase | Projects |
|-------|----------|
| 1 — Foundations | A-1, A-2, B-1, J-01 |
| 2 — Core Stack | A-3, C-1, C-2, J-02 |
| 3 — Data Engineering | B-2, B-3, I-01→I-03, I-06→I-08 |
| 4 — Infrastructure | C-3, C-4, J-04a/b, J-05, J-06 |
| 5 — Capstones | A-4, I-04/05/09/10/11, J-03 |
