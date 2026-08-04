# 🎯 Post-Bootcamp Challenge

### My self-directed engineering curriculum — the learning journey I built to grow from bootcamp graduate into a well-rounded software, data, and AI engineer.

[![Projects](https://img.shields.io/badge/Projects-106_across_20_chains-8A2BE2?style=for-the-badge)](#-the-curriculum)
[![Chains](https://img.shields.io/badge/Chains-A–T-378ADD?style=for-the-badge)](docs/CHAIN_MAP.md)
[![Roles](https://img.shields.io/badge/Role_Map-SWE_·_Data_·_FinTech-0EA5E9?style=for-the-badge)](docs/ROLE_MAP.md)
[![Status](https://img.shields.io/badge/Status-Learning_in_public-F59E0B?style=for-the-badge)](#-the-curriculum)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue?style=for-the-badge)](LICENSE-GPL)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPLv3-blue?style=for-the-badge)](LICENSE-AGPL)

[📖 Learning Plan](docs/LEARNING_PLAN.md) · [🗺️ Chain Map](docs/CHAIN_MAP.md) · [🎯 Role Map](docs/ROLE_MAP.md) · [🔗 GitHub Profile](https://github.com/niciahrymer-hillian)

---

## What this is, in one minute

**The exercise:** I set myself a multi-year, self-designed engineering curriculum and I build it in
public. Every subject I want to learn becomes a **project**; every project becomes **its own
repository** with a lesson plan, an interactive tour, and skeleton code I have to actually fill in.
Related projects are grouped into **chains** (A–T), where each project assumes the one before it.

**This repository is the index, not the code.** It explains the plan and links out to the ~106
project repos. Nothing here is a tutorial I followed — the curriculum, the lesson plans, and the
build order are mine, which is the point of the exercise.

**How to read it**

| If you want to… | Go to |
|---|---|
| See the whole plan and its phases | [Learning Plan](docs/LEARNING_PLAN.md) |
| See how projects depend on each other | [Chain Map](docs/CHAIN_MAP.md) |
| See how this maps to real job roles | [Role Map](docs/ROLE_MAP.md) |
| Jump straight to code | [The project map](#-the-full-project-map-built-so-far) below |

**Status legend used throughout:** ✅ complete · 🟡 in progress · ⬜ scaffolded (lesson plan and
skeleton written, build not started).

> Some chains are deliberately **closed-source** and have no public link — noted where they appear.

## Why I built this

When I finished my bootcamp, I knew the pace of my learning shouldn't slow down. I wanted a way to keep growing that was structured, honest, and something I could show — so I designed my own curriculum and built it in public.

This is that curriculum. It's organized into **dependency chains** (A–T): each chain is a theme, and the projects inside it build on one another. Some chains share code (one project's database literally feeds the next); others share skills (each project assumes I've learned the one before). I add a chain when there's a subject I want to genuinely understand, not just list on a résumé.

I learn best by building and by teaching, so every project is set up to do both.

## What every project includes

Each project is its own repository, and every one ships with the same learning scaffolding:

- **A lesson plan** — what I set out to learn, the concepts behind it, and a step-by-step build order.
- **An interactive tour** — a split-panel, in-browser walkthrough where I can run real code (Python, SQL, Java) or work through concepts, plus a **"Check Your Understanding" quiz** to test myself.
- **A "Why This Matters" note** — why I added this to my curriculum and how the skill applies to the work I want to do.
- **Skeleton code with `TODO`s** — so the project is something I actively build, not just read.
- **Dual GPL / AGPL licensing** so the work is open.

## 🧭 The curriculum

I think about the chains in five groups — roughly the order I'm growing through them.

### Foundations — getting the fundamentals clean
> *Why I'm learning this: before anything advanced, I want disciplined habits — clean code, tests, git, the shape of a computer, and just-enough of every core topic.*

- **Chain H — Business & Foundations** · a well-tested CLI + a CRM, plus **Agile delivery** — playable **Scrum** and **Jira** lessons (sprint simulator, burndown, live JQL) — to get structure, testing, and *how teams ship* right.
- **Chain J — Just Enough to Qualify** · DSA, git workflow, cloud, networking, IaC, AI-augmented development — the baseline every role expects.
- **Chain F — Systems & Languages, From Scratch** · an HTTP server and a language interpreter, because I understand a thing best when I've rebuilt it.
- **Chain K — Hardware & Systems Foundations** *(planned)* · Linux on old hardware, circuits, Raspberry Pi, firewalls and home networking, a **cyberdeck** build (with cellular calling/SMS + music) and a **VPN simulator** — understanding the machine from the metal up.

### Core engineering — building and shipping real software
> *Why I'm learning this: I want to take an idea all the way to a deployed, maintainable application.*

- **Chain A — Java Mastery** · OOP and interfaces through to a full Spring Boot app.
- **Chain C — Full-Stack + Infrastructure** · FastAPI + React apps, Docker, Kubernetes, and a scheduled AI job-search agent.
- **Chain O — System Design & Architecture** *(planned)* · designing for scale — the reasoning behind large systems.

### Data — the center of gravity
> *Why I'm learning this: data engineering is where I most want to work, so I'm going both wide and deep.*

- **Chain B — Banking + FinTech** · an end-to-end pipeline: scrape → validate → transform → load → serve, with fraud signals.
- **Chain D — Data & ML Pipelines** *(planned)* · applied streaming, medallion ETL, warehousing, and data-platform IaC.
- **Chain I — Data Engineering Deep Dives** *(planned)* · focused study of the exact tools data teams use (SQL, dbt, Snowflake, Spark, Kafka, Airflow, and more).
- **Chain Q — Data Analytics** · deeper SQL, EDA + data cleaning, BI dashboards & data viz, and telling a clear story — several with **built interactive tours** (a live SQL query builder, a chart builder, a dirty-dataset cleaner) + Jupyter exercises.
- **Chain R — Data Science & Statistics** · the statistics and modeling foundation, ending in a **predictive capstone** with a live threshold/confusion-matrix evaluation tour + Jupyter exercises.
- **Chain P — MLOps & Applied ML** *(planned)* · taking models to production — tracking, registries, monitoring, and serving.

### AI — understanding and building with modern models
> *Why I'm learning this: I want to use AI well and understand what's actually happening underneath.*

- **Chain E — AI Products** · a tool-using agent, a TTS note-taker, and a social-media manager.
- **Chain M — Prompt AI & LLMs** · **how LLMs work** (a live tokenizer + next-token + temperature playground) and **LLM apps & agents** (a step-through agent-loop simulator with guardrails) — both built interactive tours — plus prompting, a tiny LLM from scratch, a **non-invasive AI code reviewer**, and a **multi-agent dev system**.

### Specializations & role prep — turning learning into opportunities
> *Why I'm learning this: I want my domain background and my target roles to show up clearly in the work.*

- **Chain G — PropTech** · a property-management operations platform, a rental marketplace, and a leasing add-on — bringing my real-estate/leasing background into software.

> **Note:** the Chain G projects are **closed-source**, so there are no public links for them here. The
> engineering they exercise — multi-tenant data modeling, an accounting ledger, document generation
> and e-signature, background agents, and a React operator console — shows up in the open projects
> across Chains B, D, M, N, O and S, which are public and readable.

- **Chain N — PropTech & Real-Estate Engineering** *(planned)* · valuation models, geospatial analytics, and occupancy dashboards.
- **Chain S — FinTech Engineering** *(planned)* · payments, double-entry ledgers, market data, and risk.
- **Chain L — Cybersecurity** *(planned)* · recognizing and defending against threats — taught entirely through **safe, simulated** scenarios (no real malware).
- **Chain T — Interview Prep** *(planned)* · turning all of the above into offers, mapped role-by-role in the [Role Map](docs/ROLE_MAP.md).

## 🗺️ The full project map (built so far)

> Status: ✅ complete · 🟡 in progress · ⬜ scaffolded

### Chain A — Java Mastery
| # | Project | What I'm learning | Status | Repo |
|---|---------|-------------------|--------|------|
| A-1 | Farmer-Froilan-Java | Interfaces, multiple contracts, JUnit | 🟡 | [↗](https://github.com/niciahrymer-hillian/Farmer-Froilan-Java) |
| A-2 | Farmer-Froilan-Python | ABCs, Protocols, MRO; Java↔Python | 🟡 | [↗](https://github.com/niciahrymer-hillian/Farmer-Froilan-Python) |
| A-3 | Spring-Boot-REST-API | Spring Boot, JPA, JWT, Swagger | 🟡 | [↗](https://github.com/niciahrymer-hillian/Spring-Boot-REST-API) |
| A-4 | Real-Time-Chat-Service | Spring WebSocket/STOMP, rooms, presence, history (Java capstone) | ⬜ | [↗](https://github.com/niciahrymer-hillian/Real-Time-Chat-Service) |

### Chain B — Banking + FinTech ✅ *(tours complete)*
| # | Project | What I'm learning | Status | Repo |
|---|---------|-------------------|--------|------|
| B-1 | Web-Scraper-Postgres-Pipeline | ETL, Pydantic, idempotency, scheduled CI | 🟡 | [↗](https://github.com/niciahrymer-hillian/Web-Scraper-Postgres-Pipeline) |
| B-2 | Banking-Data-Platform | Polars, dbt medallion, window-function fraud signals | 🟡 | [↗](https://github.com/niciahrymer-hillian/Banking-Data-Platform) |
| B-3 | Banking-Interface-Fraud-UI | Spring Boot + React reading B-2's Gold tables | 🟡 | [↗](https://github.com/niciahrymer-hillian/Banking-Interface-Fraud-UI) |

### Chain C — Full-Stack + Infrastructure
| # | Project | What I'm learning | Status | Repo |
|---|---------|-------------------|--------|------|
| C-1 | Full-Stack-Job-Board | FastAPI + React + JWT, deployed | 🟡 | [↗](https://github.com/niciahrymer-hillian/Full-Stack-Job-Board) |
| C-2 | Dockerized-Microservices | Docker Compose, Nginx, Celery, GHCR | ⬜ | [↗](https://github.com/niciahrymer-hillian/Dockerized-Microservices) |
| C-3 | Ops-Management-Dashboard | WebSockets, RBAC, real-time UI | ⬜ | [↗](https://github.com/niciahrymer-hillian/Ops-Management-Dashboard) |
| C-4 | Kubernetes-IaC-Deployment | Terraform + K8s + Helm | ⬜ | [↗](https://github.com/niciahrymer-hillian/Kubernetes-IaC-Deployment) |
| C-5 | AI-Job-Search-Agent | Scheduled scraper + Claude résumé-match → emailed report | 🟡 | [↗](https://github.com/niciahrymer-hillian/AI-Job-Search-Agent) |
| C-6 | E-Commerce-Order-Backend | Catalog, cart, inventory, order state machine, payments (Java) | ⬜ | [↗](https://github.com/niciahrymer-hillian/E-Commerce-Order-Backend) |

### Chains D–J
The remaining built chains — **D** (Data & ML Pipelines), **E** (AI Products), **F** (Systems from Scratch), **G** (PropTech), **H** (Business & Foundations), **I** (Data-Engineering Deep Dives), and **J** (Foundations / Qualify) — are scaffolded and being filled in project by project. See [CHAIN_MAP.md](docs/CHAIN_MAP.md) for the full list, and each repo for its lesson plan and interactive tour.

### Chains K–T *(planned)*
Hardware, Cybersecurity, LLMs, PropTech engineering, System Design, MLOps, Data Analytics, Data Science, FinTech, and Interview Prep — designed and queued. The [Role Map](docs/ROLE_MAP.md) shows how they line up against the roles I'm working toward.

## 🎯 Built with real roles in mind

I keep a [Role Map](docs/ROLE_MAP.md) that connects each chain to the roles I'm preparing for — **Software Engineer, Data Engineer, Data Analyst, Data Scientist, and FinTech** — with the projects that demonstrate each skill and a study path for interviews. It keeps the curriculum honest: every chain earns its place by moving me toward work I actually want.

## 🧰 Skills this curriculum covers

| Category | Covered by |
|----------|-----------|
| **Languages** | Java 17, Python 3.11+, Go, TypeScript, SQL |
| **Frameworks** | Spring Boot, FastAPI, React, Django, Flask |
| **Databases** | PostgreSQL, SQLite, Snowflake, Teradata, Delta Lake |
| **Infrastructure** | Docker, Kubernetes, Helm, Terraform, AWS, Azure, Nginx |
| **Data Tools** | dbt, Polars, Apache Spark, Kafka, Airflow, Tableau |
| **AI** | LLM prompting, agents, RAG, model serving |
| **Practices** | TDD, CI/CD, git workflow, RBAC, WCAG 2.1 AA, IaC, defensive security |

## 🚀 How to explore this portfolio

```bash
# Each project is its own repo. Clone any one to start:
git clone https://github.com/niciahrymer-hillian/Banking-Data-Platform.git
cd Banking-Data-Platform

# Read the lesson plan, then open the interactive tour in a browser:
open docs/interactive/index.html     # macOS  (xdg-open on Linux)

# Build from the skeleton — every TODO is a step in the lesson plan.
```

Each repo's interactive tour is also served free via **GitHub Pages** from its `docs/` folder.

---

*Learning in public, one chain at a time.* — [niciahrymer-hillian](https://github.com/niciahrymer-hillian)

Dual licensed — [GPL v3](LICENSE-GPL) and [AGPL v3](LICENSE-AGPL).
