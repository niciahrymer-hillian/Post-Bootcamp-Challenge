# 📖 Learning Plan — Post-Bootcamp-Challenge

This document explains **why each chain exists**, **what order to build in**, and **how the chains reinforce each other**. The README is the storefront; this is the curriculum.

---

## The Philosophy

Companies hire on *how you write and document code*, not on the topic. So every project here is engineered to demonstrate professional habits:

- **Robust documentation** — every repo has a recruiter-facing README, a lesson plan, and an interactive tour.
- **Clean git history** — conventional commits, one feature per commit, real branches.
- **Live demos** — deployable apps with a public URL where it makes sense.
- **From-scratch depth** — a few projects forbid scaffolding on purpose, to prove understanding.

There are two kinds of "building on" in this plan:

1. **Code dependency** — one project's output literally feeds the next (e.g. the Banking Data Platform's Gold tables are read by the Banking UI). These are noted explicitly.
2. **Skill dependency** — no shared code, but each project assumes the skills the previous one taught. You don't import the old project; you're just a more capable engineer when you start.

---

## Recommended Build Order

> The chains can overlap. Code-dependency chains (B, C) must be built in order. Skill chains (I, J) can be sampled in any order once their prerequisites are met.

### Phase 1 — Foundations (Months 1–2)
- **A-1 Farmer-Froilan-Java** → locks in Java OOP, interfaces, multi-inheritance. *Verify: JUnit suite green, UML generated.*
- **A-2 Farmer-Froilan-Python** → port the same model to ABCs/Protocols; write the Java↔Python comparison. *Verify: pytest green, COMPARISON.md complete.*
- **B-1 Web-Scraper-Postgres-Pipeline** → first automated pipeline + scheduled GitHub Action. *Verify: CI cron runs, idempotent loader proven by running twice.*
- **J-01 DSA-OOP-Fundamentals** → algorithmic baseline (good in parallel, evenings). *Verify: all sorting/structure tests pass.*

### Phase 2 — Core Stack (Months 3–5)
- **A-3 Spring-Boot-REST-API** → Java meets a real web server; JPA, JWT, Swagger. *Verify: MockMvc tests pass, Swagger UI lists every endpoint.*
- **C-1 Full-Stack-Job-Board** → FastAPI + React + JWT, deployed. *Verify: deployed URL reachable, auth round-trips.*
- **C-2 Dockerized-Microservices** → containerize C-1's patterns; Compose, Nginx, Celery, GHCR. *Verify: `docker compose up` brings the whole stack online.*
- **J-02 Git-Collaboration-Workflow** → professional git habits (parallel). *Verify: pre-commit hooks fire, PR template in use.*

### Phase 3 — Data Engineering (Months 5–8)
- **B-2 Banking-Data-Platform** → Polars + dbt medallion + IsolationForest. *Verify: `dbt build` passes all tests, Gold tables materialized.*
- **B-3 Banking-Interface-Fraud-UI** → Spring Boot + React reading B-2's Gold tables. *Verify: UI renders live Gold data, axe audit passes.*
- **I-01 → I-03** SQL / ETL-ELT / dbt deep dives → the theory behind B. *Verify: every exercise solved.*
- **I-06 → I-08** Spark / Kafka / Airflow → distributed + orchestration concepts.

### Phase 4 — Infrastructure (Months 7–10)
- **C-3 Ops-Management-Dashboard** → WebSockets + RBAC + real-time UI. *Verify: two clients see live updates.*
- **C-4 Kubernetes-IaC-Deployment** (from scratch) → Terraform + K8s + Helm. *Verify: `helm upgrade` does a zero-downtime rollout.*
- **J-04a/J-04b/J-05/J-06** Cloud + Networking + Terraform → IaC fluency. *Verify: `terraform apply` provisions, `destroy` tears down cleanly.*

### Phase 5 — Capstones (Months 9–12)
- **A-4 Entrada-Clone** → full-stack leasing platform; domain advantage + Java depth + PDF generation. *Verify: lease PDF generates, occupancy analytics correct.*
- **I-04/I-05/I-09/I-10/I-11** → enterprise data tools (Snowflake, Azure, Teradata, Tableau, Django/Flask) to round out breadth.
- **J-03 AI-Augmented-Development** → reflect on the AI workflow used throughout.

---

## How the Chains Connect

- **B-1 → B-2 → B-3** is a single FinTech system split across three repos: scraped/ingested data → cleaned + modeled → served in a UI.
- **C-1 → C-2 → C-3 → C-4** is one app maturing: build it → containerize it → make it real-time → ship it to Kubernetes.
- **J-06 IaC-Terraform reinforces C-4** — both teach Terraform; do J-06 first for fundamentals, then C-4 applies them to a real cluster.
- **I-05 Azure-Data-Stack + J-04b Cloud-Fundamentals-Azure** reinforce each other — one is the data services, the other the core platform.
- **A-1 → A-2 → A-3 → A-4** is the Java spine: OOP fundamentals → language comparison → framework → full-stack capstone.

---

## The "30th Project" and Chains D–H

The numbering reserves room for a 30th project and Chains D–H, drawn from the parked candidates: CLI Task Manager, HTTP Server from scratch, ML Model Serving API, Custom Language Interpreter, BD/Marketing CRM, Streaming Pipeline, Databricks ETL, AI TTS + Notes, Social Media Manager, Leasing App, AI Agent. These will be specified after the core A/B/C/I/J chains are underway.
