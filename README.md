# Keep It Local

### A practical guide to reducing your dependence on cloud services and data centers.

Keep It Local is where AI systems architecture, digital sovereignty, infrastructure resilience, and community technology meet.

You do **not** have to be a technology expert to have more control over your digital life or your small business.

Keep It Local works at two levels.

For individuals and organizations, it provides practical ways to understand
and reduce unnecessary digital dependency.

For technical practitioners, researchers, architects, and communities, it
provides a framework for modeling infrastructure dependencies, resilience,
sovereignty, and local control across the digital-to-physical stack.

This project provides simple, practical tools to help individuals, families, artists, community organizations, and small businesses understand what they depend on—and make thoughtful choices about what they can keep local, own, replace, or operate without the cloud.

---

## Start Here

### [Data Center Decision Checklist](./infrastructure/DATA_CENTER_CHECKLIST.md)

Print it. Share it. Use it with your family, business, organization, or community.

You do not have to change everything at once.

The goal is to **reduce unnecessary dependence one decision at a time.**

### [Data Center Freedom (PDF)](./docs/Data-Center-Freedom.pdf)

An essay framing local-first, human-centered digital infrastructure.

---

## How to Use This Repository

Pick the path that matches what you are trying to do. For the full framework map, see the [System Architecture](./architecture/KEEP_IT_LOCAL_SYSTEM_ARCHITECTURE.md).

### 1. You just want practical help (nontechnical)

- **Start with this README** — it is written for nontechnical readers.
- **Print the [Data Center Decision Checklist](./infrastructure/DATA_CENTER_CHECKLIST.md)** and work through it for your family, business, or community. It is the practical, single-decision-at-a-time entry point.

### 2. You want to analyze one specific system

Follow the [worked personal example](./examples/personal-photo-library.md) — a person-level example — or the [EO 14420/14421 case study](./research/EO_14420_14421/README.md) for a large infrastructure case:

1. **Define the question** — what do you want to know about the system?
2. **Read the method** — [methodology/RESEARCH_METHOD.md](./methodology/RESEARCH_METHOD.md) is the 13-step repeatable process. It works at any scale: personal, business, AI workload, community.
3. **Classify claims as you go** — use the [Evidence Standard](./methodology/EVIDENCE_STANDARD.md) labels: **CONFIRMED / REPORTED / INFERRED / HYPOTHESIS / UNKNOWN**. Remember, *UNKNOWN is a valid result.*

### 3. You want to model dependencies systematically

1. Read the core model: [models/dependency-model.md](./models/dependency-model.md) — dimensions, types, criticality (LOW → CRITICAL), evidence discipline.
2. Position things using the [Infrastructure Stack](./models/infrastructure-stack.md) (digital → physical layers).
3. Ask failure/recovery questions with the [Resilience Model](./models/resilience-model.md).
4. Ask control questions with the [Sovereignty Model](./models/sovereignty-model.md).
5. Record what you find as data using the [Infrastructure Data Model](./models/infrastructure-data-model.md):
   - [`models/infrastructure.json`](./models/infrastructure.json) and [`models/infrastructure.csv`](./models/infrastructure.csv) are working templates — copy them and adapt;
   - the schemas in [`models/schemas/`](./models/schemas/infrastructure.schema.json) validate your data (draft-07 JSON Schema).

### 4. You are a researcher doing a case study

1. Start from the [System Architecture](./architecture/KEEP_IT_LOCAL_SYSTEM_ARCHITECTURE.md) to understand how the layers connect.
2. Follow the EO case as the reference implementation: [research/EO_14420_14421/00_CASE_STUDY_INDEX.md](./research/EO_14420_14421/00_CASE_STUDY_INDEX.md) maps every framework component to how the case uses it.
3. When you add your own research, apply the same six components (Evidence Standard + Dependency / Stack / Data / Resilience / Sovereignty models) and put results in `research/`. The framework stays in `models/` and `methodology/`, unchanged.

### 5. You are a developer building tooling

- **Validated, consistent machine input:** [`models/infrastructure.json`](./models/infrastructure.json) plus [`models/schemas/*.schema.json`](./models/schemas/infrastructure.schema.json) are your contract. Model instances are JSON documents that validate against `infrastructure.schema.json`.
- **Enums you can rely on:** `criticality`, `evidenceClassification`, `dependencyType`, `layer`, and `status` are defined identically across every schema.
- The `principles/ → methodology/ → models/ → infrastructure/ → applications → research` layout is deliberately structured so documentation can grow into datasets and CLI tooling.

### Quick map

| Need | Go to |
| --- | --- |
| Nontechnical start | [`README.md`](./README.md) |
| Practical checklist | [`infrastructure/DATA_CENTER_CHECKLIST.md`](./infrastructure/DATA_CENTER_CHECKLIST.md) |
| How the pieces fit | [`architecture/KEEP_IT_LOCAL_SYSTEM_ARCHITECTURE.md`](./architecture/KEEP_IT_LOCAL_SYSTEM_ARCHITECTURE.md) |
| The repeatable process | [`methodology/RESEARCH_METHOD.md`](./methodology/RESEARCH_METHOD.md) |
| What counts as true | [`methodology/EVIDENCE_STANDARD.md`](./methodology/EVIDENCE_STANDARD.md) |
| The core model | [`models/dependency-model.md`](./models/dependency-model.md) |
| Record findings as data | [`models/`](./models/infrastructure-data-model.md) (+ [`schemas/`](./models/schemas/infrastructure.schema.json)) |
| Reference case study | [`research/EO_14420_14421/`](./research/EO_14420_14421/README.md) |

---

## What Does "Keep It Local" Mean?

It means asking a simple question:

> **"Do I really need this to live somewhere far away in someone else's data center?"**

Sometimes the answer will be **yes**.

Sometimes the answer will be **no**.

Sometimes there is a better middle ground.

The purpose of this project is not to tell you to stop using the internet, cloud services, or data centers.

It is to help you understand your choices.

---

## Three Scales of Digital Independence

Keep It Local can be applied at three interconnected scales:

### Personal
Can I access and control the information I depend on?

### Organizational
Can my business or community organization continue operating if an external service disappears?

### Community
What physical, electrical, network, water, computing, and supply-chain infrastructure does our region depend on—and what happens when those dependencies fail?

The same principle applies at every scale:

> Understand your dependencies. Keep what you can. Own what matters. Build alternatives.
---

## The Keep It Local Framework

Keep It Local uses a systems approach:

**Principles → Methodology → Models → Infrastructure → Applications → Research**

The framework can be applied to a personal digital system, a small
business, an AI workload, or community-scale infrastructure.

The question remains the same:

> What does this system depend on, who controls those dependencies,
> what happens when they fail, and what alternatives exist?

### The framework parts

- **[Architecture](./architecture/KEEP_IT_LOCAL_SYSTEM_ARCHITECTURE.md)** — how the whole system fits together.
- **[Principles](./principles/LOCAL_FIRST.md)** — what matters: local control, data sovereignty, community resilience, sovereign AI.
- **[Methodology](./methodology/EVIDENCE_STANDARD.md)** — how we know: the Evidence Standard, the Research Method, and Source Ranking.
- **[Models](./models/dependency-model.md)** — how systems are represented: the Dependency Model, Infrastructure Stack, Resilience Model, and Sovereignty Model.
- **[Infrastructure](./infrastructure/CRITICAL_INFRASTRUCTURE.md)** — practical tools for digital, physical, and energy systems.
- **[Community Infrastructure](./community-infrastructure/README.md)** — applying the framework at community scale.
- **[Examples](./examples/README.md)** — worked applications of the framework to real systems.
- **[Research](./research/EO_14420_14421/README.md)** — the first formal case study: bulk-power security, AI infrastructure, and the Akwesasne/Massena context.

---

## Start With What Matters Most

Consider the things you rely on every day:

* Your photos and personal files
* Your business records
* Your customer information
* Your creative work
* Your financial documents
* Your websites
* Your email
* Your software
* Your AI tools
* Your backups
* Your passwords and important accounts

Ask yourself:

**Could I still access this if the service disappeared tomorrow?**

If the answer is no, you have identified a dependency worth examining.

---

## The Goal

You don't need to eliminate every cloud service.

A more practical goal is:

**Keep what you can.
Own what matters.
Back up what you cannot lose.
Understand what you depend on.
Keep alternatives available.**

Cloud services can remain useful.

The difference is whether they are a **choice** or a **requirement for your ability to operate.**

---

## For Individuals

You can use this project to gradually increase your personal digital independence.

Examples include:

* Keeping local copies of important documents
* Maintaining local backups of photographs
* Downloading important records from online services
* Learning which subscriptions you actually need
* Keeping copies of your creative work outside a single platform
* Using software that allows you to export your information
* Maintaining important information that remains accessible when the internet is unavailable

See the worked example: [A Personal Photo Library](./examples/personal-photo-library.md).

---

## For Small Businesses

A small business can be particularly vulnerable when essential operations depend on a handful of outside services.

Consider:

* Customer records
* Accounting information
* Website content
* Product information
* Business documents
* Marketing materials
* Email
* Scheduling
* Creative assets
* AI services
* Cloud storage
* Business software

For each one, ask:

> **"What happens to my business if this service goes away?"**

Then decide whether you need a local copy, a backup, an alternative, or a different workflow.

---

## One Step at a Time

You do not need to buy expensive equipment.

You do not need to become a computer expert.

You do not need to disconnect from the internet.

Start with one important thing.

**Find it.
Back it up.
Understand it.
Learn your alternatives.**

Then do the next one.

---

## Why This Matters

Communities are increasingly surrounded by large digital infrastructure while many of the people living in those communities have little understanding of how dependent their own lives and businesses have become on distant computing infrastructure.

This project approaches the problem from the other direction:

**Before asking how much more infrastructure we need, let's understand what we already depend on—and what we can control ourselves.**

Local resilience begins with knowing what you have the ability to control.

---

## Share This

This resource is intended to be easy to print, share, discuss, and use.

Give the checklist to:

* A neighbor
* A family member
* A local business owner
* A small-business owner
* An artist
* A community organization
* A local elected representative
* Someone who simply wants to understand their digital dependence

You don't need to be technical to start.

---

## Keep It Local

**Understand your dependencies.
Keep what you can.
Own what matters.
Build alternatives.**

Small choices can create greater resilience.

---

### About This Project

**Keep It Local** is an independent community resource created by **MoniGarr.com** to help ordinary people make informed choices about digital infrastructure, cloud dependence, local computing, data ownership, and personal and business resilience.

The purpose is education—not fear.

The goal is **more choice, more understanding, and more control.**

Research disclaimer: Keep It Local is an independent community technology and infrastructure research project. The materials in this repository are intended to support public understanding, technical research, and informed discussion. They do not constitute legal, engineering, regulatory, cybersecurity, environmental, or financial advice. References to specific projects, organizations, jurisdictions, technologies, or potential risks should not be interpreted as findings of wrongdoing or security threats unless supported by authoritative evidence.