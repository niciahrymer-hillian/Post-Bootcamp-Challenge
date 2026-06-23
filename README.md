# 🎯 Post-Bootcamp-Challenge
### A self-directed 30-project engineering portfolio — built like a real team builds, organized into dependency chains.

[![Projects](https://img.shields.io/badge/Projects-40-8A2BE2?style=for-the-badge)](#-the-full-project-map)
[![Chains](https://img.shields.io/badge/Chains-A–J-378ADD?style=for-the-badge)](docs/CHAIN_MAP.md)
[![Languages](https://img.shields.io/badge/Languages-Java%20|%20Python%20|%20Go%20|%20TypeScript%20|%20SQL-0EA5E9?style=for-the-badge)](#-skills-matrix)
[![Status](https://img.shields.io/badge/Status-In%20Progress-F59E0B?style=for-the-badge)](#-the-full-project-map)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue?style=for-the-badge)](LICENSE-GPL)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPLv3-blue?style=for-the-badge)](LICENSE-AGPL)

[📖 Learning Plan](docs/LEARNING_PLAN.md) · [🗺️ Chain Map](docs/CHAIN_MAP.md) · [🔗 GitHub Profile](https://github.com/niciahrymer-hillian)

---

## What This Is

This is the index repo for a self-built, post-bootcamp engineering challenge: **30 real projects**, each its own GitHub repository, organized into **dependency chains** (A–J). Some chains share code (one project's database literally feeds the next); others share skills (each project assumes you mastered the one before). Every repo ships with a recruiter-facing README, a full bootcamp-style lesson plan, an interactive split-panel tour, skeleton code with `TODO`s to implement, and dual GPL/AGPL licensing.

```
                          POST-BOOTCAMP-CHALLENGE
                          (this index repo)
                                  │
    ┌───────────┬───────────┬─────┴─────┬─────────────┬─────────────┐
    ▼       ▼       ▼       ▼       ▼       ▼       ▼       ▼       ▼       ▼
  CHAIN   CHAIN   CHAIN   CHAIN   CHAIN   CHAIN   CHAIN   CHAIN   CHAIN   CHAIN
    A       B       C       D       E       F       G       H       I       J
  Java   Banking Full-   Data &   AI    Systems Prop-  Business Data    Qualify
  Mastery +Fin-  Stack   ML Pipe- Prod-  & Lang  Tech   & Found- Eng.    -the
         Tech   +Infra   lines   ucts  (scratch)        ations  Deep    Resume
    │       │       │       │       │       │       │       │     Dives    │
  4 repo  3 repo  4 repo  3 repo  3 repo  2 repo  1 repo  2 repo 11 repo 7 repo

  Total: 40 project repos + this index repo.
  Code-dependency chains: B (B-1→B-2→B-3), C (C-1→C-2→C-3→C-4).
```

<!-- SCREENSHOT PLACEHOLDER:
     docs/screenshots/profile-grid.png  — GitHub profile showing the repo grid
     docs/screenshots/chain-map.png     — rendered chain dependency map
-->

## 🧭 Why This Was Built

Recruiters and engineers don't hire on topic — they hire on **how you write and document code**. This portfolio is engineered to show exactly that:

- **Substantial full-stack apps** with real databases, auth, and deployed APIs (Chains A, C).
- **Recreated technologies from scratch** — an HTTP server, a custom language interpreter, IaC from the ground up — to prove deep technical understanding (Chain J, scratch projects).
- **Data & ML pipelines** that train, evaluate, and serve — not just notebooks (Chains B, I).
- **Infrastructure & automation** — Docker, Kubernetes, Terraform, CI/CD (Chains C, J).
- **Domain advantage** — real estate / occupancy / leasing expertise baked into the data models (Entrada Clone), a moat most engineers can't replicate.

It is also a **learning system**: every repo teaches the concepts it uses, so the portfolio doubles as a curriculum I can revisit and others can learn from.

## 🗺️ The Full Project Map

> Status legend: ✅ complete · 🟡 in progress · ⬜ scaffolded · 🔒 reserved

### Chain A — Java Mastery
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| A-1 | Farmer-Froilan-Java | Interfaces, multi-inheritance, JUnit | 🟡 | [↗](https://github.com/niciahrymer-hillian/Farmer-Froilan-Java) |
| A-2 | Farmer-Froilan-Python | ABCs, Protocols, MRO, Java↔Python | 🟡 | [↗](https://github.com/niciahrymer-hillian/Farmer-Froilan-Python) |
| A-3 | Spring-Boot-REST-API | Spring Boot, JPA, JWT, Swagger | ⬜ | [↗](https://github.com/niciahrymer-hillian/Spring-Boot-REST-API) |
| A-4 | Entrada-Clone | Full-stack leasing platform (also Chain G capstone) | ⬜ | [↗](https://github.com/niciahrymer-hillian/Entrada-Clone) |

### Chain B — Banking + FinTech (code-dependency chain)
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| B-1 | Web-Scraper-Postgres-Pipeline | ETL, Pydantic, idempotency, CI cron | 🟡 | [↗](https://github.com/niciahrymer-hillian/Web-Scraper-Postgres-Pipeline) |
| B-2 | Banking-Data-Platform | Polars, dbt medallion, IsolationForest | 🟡 | [↗](https://github.com/niciahrymer-hillian/Banking-Data-Platform) |
| B-3 | Banking-Interface-Fraud-UI | Spring Boot + React, reads B-2 Gold tables | 🟡 | [↗](https://github.com/niciahrymer-hillian/Banking-Interface-Fraud-UI) |

### Chain C — Full-Stack + Infrastructure (code-dependency chain)
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| C-1 | Full-Stack-Job-Board | FastAPI + React + JWT, deployed | ⬜ | [↗](https://github.com/niciahrymer-hillian/Full-Stack-Job-Board) |
| C-2 | Dockerized-Microservices | Docker Compose, Nginx, Celery, GHCR | ⬜ | [↗](https://github.com/niciahrymer-hillian/Dockerized-Microservices) |
| C-3 | Ops-Management-Dashboard | WebSockets, RBAC, real-time UI | ⬜ | [↗](https://github.com/niciahrymer-hillian/Ops-Management-Dashboard) |
| C-4 | Kubernetes-IaC-Deployment | Terraform + K8s + Helm (from scratch) | ⬜ | [↗](https://github.com/niciahrymer-hillian/Kubernetes-IaC-Deployment) |

### Chain D — Data & ML Pipelines
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| D-1 | ML-Model-Serving-API | Train, evaluate, serve behind FastAPI | ⬜ | [↗](https://github.com/niciahrymer-hillian/ML-Model-Serving-API) |
| D-2 | Streaming-Data-Pipeline | Real-time ingest + processing | ⬜ | [↗](https://github.com/niciahrymer-hillian/Streaming-Data-Pipeline) |
| D-3 | Databricks-Medallion-ETL | Bronze→Silver→Gold on Delta Lake | ⬜ | [↗](https://github.com/niciahrymer-hillian/Databricks-Medallion-ETL) |

### Chain E — AI Products
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| E-1 | AI-TTS-Notes | Natural-voice TTS + note-taking | ⬜ | [↗](https://github.com/niciahrymer-hillian/AI-TTS-Notes) |
| E-2 | AI-Social-Media-Manager | Schedule/auto-post, notifications, analytics | ⬜ | [↗](https://github.com/niciahrymer-hillian/AI-Social-Media-Manager) |
| E-3 | AI-Agent-Assistant | Tool-using agent with memory | ⬜ | [↗](https://github.com/niciahrymer-hillian/AI-Agent-Assistant) |

### Chain F — Systems & Languages (from scratch)
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| F-1 | HTTP-Server-From-Scratch | Raw sockets → Go core loop | ⬜ | [↗](https://github.com/niciahrymer-hillian/HTTP-Server-From-Scratch) |
| F-2 | Custom-Language-Interpreter | Lexer, parser, AST, REPL | ⬜ | [↗](https://github.com/niciahrymer-hillian/Custom-Language-Interpreter) |

### Chain G — PropTech
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| G-1 | Leasing-Agent-App | Renter↔apartment matching (HomeMatch-style) | ⬜ | [↗](https://github.com/niciahrymer-hillian/Leasing-Agent-App) |
| G-2 | Entrada-Clone | Full leasing/occupancy platform (shared with Chain A) | ⬜ | [↗](https://github.com/niciahrymer-hillian/Entrada-Clone) |

### Chain H — Business & Foundations
| # | Project | Focus | Status | Repo |
|---|---------|-------|--------|------|
| H-1 | CLI-Task-Manager | Foundations: clean Python + SQLite CLI | ⬜ | [↗](https://github.com/niciahrymer-hillian/CLI-Task-Manager) |
| H-2 | BD-Marketing-CRM | BD + marketing CRM with AI email drafts | ⬜ | [↗](https://github.com/niciahrymer-hillian/BD-Marketing-CRM) |

### Chain I — Data Engineering Deep Dives (skill chain)
| # | Project | Status | Repo |
|---|---------|--------|------|
| I-01 | SQL-Deep-Dive | ⬜ | [↗](https://github.com/niciahrymer-hillian/SQL-Deep-Dive) |
| I-02 | ETL-ELT-Deep-Dive | ⬜ | [↗](https://github.com/niciahrymer-hillian/ETL-ELT-Deep-Dive) |
| I-03 | DBT-Deep-Dive | ⬜ | [↗](https://github.com/niciahrymer-hillian/DBT-Deep-Dive) |
| I-04 | Snowflake-Deep-Dive | ⬜ | [↗](https://github.com/niciahrymer-hillian/Snowflake-Deep-Dive) |
| I-05 | Azure-Data-Stack | ⬜ | [↗](https://github.com/niciahrymer-hillian/Azure-Data-Stack) |
| I-06 | Apache-Spark | ⬜ | [↗](https://github.com/niciahrymer-hillian/Apache-Spark) |
| I-07 | Apache-Kafka | ⬜ | [↗](https://github.com/niciahrymer-hillian/Apache-Kafka) |
| I-08 | Apache-Airflow | ⬜ | [↗](https://github.com/niciahrymer-hillian/Apache-Airflow) |
| I-09 | Teradata-Intro | ⬜ | [↗](https://github.com/niciahrymer-hillian/Teradata-Intro) |
| I-10 | Tableau-BI-Dashboards | ⬜ | [↗](https://github.com/niciahrymer-hillian/Tableau-BI-Dashboards) |
| I-11 | Django-Flask-Review | ⬜ | [↗](https://github.com/niciahrymer-hillian/Django-Flask-Review) |

### Chain J — Just Enough to Qualify (skill + mini-projects)
| # | Project | Status | Repo |
|---|---------|--------|------|
| J-01 | DSA-OOP-Fundamentals | ⬜ | [↗](https://github.com/niciahrymer-hillian/DSA-OOP-Fundamentals) |
| J-02 | Git-Collaboration-Workflow | ⬜ | [↗](https://github.com/niciahrymer-hillian/Git-Collaboration-Workflow) |
| J-03 | AI-Augmented-Development | ⬜ | [↗](https://github.com/niciahrymer-hillian/AI-Augmented-Development) |
| J-04a | Cloud-Fundamentals-AWS | ⬜ | [↗](https://github.com/niciahrymer-hillian/Cloud-Fundamentals-AWS) |
| J-04b | Cloud-Fundamentals-Azure | ⬜ | [↗](https://github.com/niciahrymer-hillian/Cloud-Fundamentals-Azure) |
| J-05 | Networking-Basics | ⬜ | [↗](https://github.com/niciahrymer-hillian/Networking-Basics) |
| J-06 | IaC-Terraform | ⬜ | [↗](https://github.com/niciahrymer-hillian/IaC-Terraform) |

> All ten chains (A–J) are now defined — **40 project repos** in total. Chains D–H were scaffolded from the original roadmap's parked candidate pool. Entrada-Clone is shared between Chain A (Java capstone) and Chain G (PropTech) as a single repo.

## 🧰 Skills Matrix

| Category | Covered by |
|----------|-----------|
| **Languages** | Java 17, Python 3.11+, Go, TypeScript, SQL |
| **Frameworks** | Spring Boot, FastAPI, React, Django, Flask |
| **Databases** | PostgreSQL, SQLite, Snowflake, Teradata, Delta Lake |
| **Infrastructure** | Docker, Kubernetes, Helm, Terraform, AWS, Azure, Nginx |
| **Data Tools** | dbt, Polars, Apache Spark, Kafka, Airflow, Tableau |
| **Practices** | TDD, CI/CD, Git Flow, conventional commits, RBAC, WCAG 2.1 AA, IaC |

## 🚀 How to Use This Portfolio

```bash
# Each project is its own repo. Clone any one to start:
git clone https://github.com/niciahrymer-hillian/Farmer-Froilan-Java.git
cd Farmer-Froilan-Java

# Read the lesson plan, then open the interactive tour in a browser:
open docs/interactive/index.html     # macOS  (xdg-open on Linux)

# Build from the skeleton — every TODO is a step in the lesson plan.
```

Each repo's interactive tour is also served free via **GitHub Pages** from its `docs/` folder.

---

Dual licensed — [GPL v3](LICENSE-GPL) and [AGPL v3](LICENSE-AGPL).
