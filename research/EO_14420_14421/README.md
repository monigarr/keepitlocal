# EO_14420_14421 — Bulk-Power Security, AI Infrastructure & Keep It Local

> **Research case study:** Critical infrastructure, AI/data-center growth, resilience, supply-chain security, and community infrastructure literacy.

> **Framework component:** This folder is the **first formal case study** of the Keep It Local systems framework. It applies the [Evidence Standard](../../methodology/EVIDENCE_STANDARD.md), [Dependency Model](../../models/dependency-model.md), [Infrastructure Stack](../../models/infrastructure-stack.md), [Infrastructure Data Model](../../models/infrastructure-data-model.md), [Resilience Model](../../models/resilience-model.md), and [Sovereignty Model](../../models/sovereignty-model.md) to a real infrastructure-policy question. Start at [`00_CASE_STUDY_INDEX.md`](00_CASE_STUDY_INDEX.md).

This folder is a research case study examining how recent U.S. critical-infrastructure policy intersects with the rapid expansion of artificial intelligence and large-scale data-center infrastructure.

It is **not an advocacy document** and does not make findings about the security of any particular facility, vendor, country, technology, or project.

## Purpose

This folder documents the relationship between the **August 26, 2026 U.S. presidential action declaring a national emergency concerning the U.S. bulk-power system** and the broader principles of the **Keep It Local** project.

Keep It Local is not anti-AI, anti-cloud, or anti-data-center.

It is concerned with:

* infrastructure literacy;
* community resilience;
* data sovereignty;
* technology independence;
* understanding infrastructure dependencies;
* identifying unnecessary points of centralized dependency;
* and helping people make informed decisions about the systems on which they rely.

The Executive Order explicitly identifies the rapid growth of advanced manufacturing, data centers, artificial intelligence, and defense production as factors increasing dependence on reliable electricity and magnifying the consequences of disruption to the U.S. bulk-power system.

## Core Thesis

> **AI infrastructure is physical infrastructure.**

Artificial intelligence is often discussed as software, models, applications, and data. At scale, however, AI depends upon a substantial physical infrastructure stack.

A responsible assessment of large-scale AI and data-center development therefore requires looking beyond buildings, servers, employment, tax revenue, and electricity consumption.

Relevant infrastructure can include:

```text
ENERGY
  ↓
GENERATION
  ↓
TRANSMISSION
  ↓
SUBSTATIONS
  ↓
TRANSFORMERS / SWITCHGEAR / PROTECTION
  ↓
CONTROL SYSTEMS
  ↓
UPS / BATTERY / BACKUP POWER
  ↓
NETWORKING
  ↓
COMPUTE
  ↓
STORAGE
  ↓
SOFTWARE
  ↓
DATA
```

Depending on the project, assessment may therefore need to consider:

* transmission infrastructure;
* substations;
* transformers;
* generation;
* grid-connected inverters;
* battery energy storage;
* UPS systems;
* protective relaying;
* metering;
* circuit breakers;
* industrial control systems;
* software;
* firmware;
* remote-access capabilities;
* maintenance and update mechanisms;
* supply-chain dependencies;
* cybersecurity;
* resilience and recovery;
* water and cooling infrastructure;
* and who bears the consequences when infrastructure fails.

## Why This Matters to Akwesasne

The proposed large-scale data-center development near Massena is geographically close to Akwesasne.

The **Mohawk Council of Akwesasne** has publicly raised concerns regarding matters including energy and water demand, local power-system strain, environmental impacts, health and safety, consultation, and protection of Akwesasne lands and waters.

This repository does **not** claim that the Executive Order:

* gives Akwesasne new jurisdiction over the Massena project;
* automatically applies to Canadian portions of Akwesasne;
* determines that the Massena project presents a national-security threat;
* establishes that any particular vendor or technology is unsafe;
* or prohibits the development of a particular data center.

Instead, the Executive Order provides an additional **critical-infrastructure and supply-chain security lens** through which major AI infrastructure can be examined.

That lens can complement, but does not replace:

* Indigenous governance and consultation;
* environmental review;
* municipal and state regulatory processes;
* utility and grid planning;
* public-interest analysis;
* cybersecurity analysis;
* and community decision-making.

## Research Approach

The research in this folder follows a simple principle:

> **Understand the infrastructure before drawing conclusions about it.**

Each research question should distinguish between:

1. **What is documented**
2. **What is reported**
3. **What can reasonably be inferred**
4. **What remains unknown**
5. **What evidence would resolve the uncertainty**

This distinction is particularly important when discussing critical infrastructure, cybersecurity, national security, Indigenous communities, and specific commercial projects.

## Evidence Standard

The repository's canonical evidence standard lives at [`methodology/EVIDENCE_STANDARD.md`](../../methodology/EVIDENCE_STANDARD.md). The local `EVIDENCE_STANDARD.md` is a pointer to it.

The standard is intentionally conservative.

A missing document is not evidence of wrongdoing.

A foreign manufacturer is not, by itself, evidence of a security threat.

A large electricity load is not, by itself, evidence of an unsafe grid condition.

A technical possibility is not the same thing as a documented vulnerability.

The purpose of this research is to make those distinctions visible.

## Documents in This Folder

### `00_CASE_STUDY_INDEX.md`

The case-study index. Maps every framework component (Evidence Standard, Dependency Model, Infrastructure Stack, Infrastructure Data Model, Resilience Model, Sovereignty Model) to how this case study uses it. Start here.

### `01_EXECUTIVE_ORDER_ANALYSIS.md`

Technical reading of the August 26, 2026 presidential action, including its stated purpose, scope, covered infrastructure, implementation mechanisms, and limitations.

### `02_AKWESASNE_IMPLICATIONS.md`

Examines how the federal critical-infrastructure framework may intersect with the existing Akwesasne/Massena context while distinguishing U.S. federal authority from Indigenous, Canadian, New York State, municipal, and other jurisdictions.

### `03_CRITICAL_INFRASTRUCTURE_CHECKLIST.md`

A reusable checklist for examining major AI and data-center infrastructure, including electrical systems, supply chains, cybersecurity, resilience, environmental dependencies, and governance.

### `04_MASSENA_RESEARCH_FRAMEWORK.md`

A neutral research framework for documenting the infrastructure dependencies and community implications of large-scale data-center development in the Massena area.

### `05_IMPLEMENTATION_WATCHLIST.md`

A living research document for monitoring subsequent federal, New York State, utility, municipal, and other authoritative developments that may clarify implementation of the Executive Order and related data-center policy.

### `06_KEEP_IT_LOCAL_POSITION.md`

Connects the critical-infrastructure discussion to the broader Keep It Local principles of local capability, sovereignty, resilience, and reduced unnecessary dependency.

### `07_SOURCES_AND_TERMINOLOGY.md`

Primary sources, terminology, jurisdictional considerations, research cautions, and definitions used throughout this case study.

## What This Research Is — and Is Not

### This research is:

* infrastructure research;
* technical documentation;
* public-interest technology research;
* an exploration of resilience and dependency;
* an attempt to make complex infrastructure understandable;
* a case study in the relationship between AI and physical infrastructure.

### This research is not:

* a legal opinion;
* an engineering certification;
* a cybersecurity assessment of a specific facility;
* a finding of national-security risk;
* a regulatory determination;
* an environmental assessment;
* or a substitute for official government, utility, Indigenous-government, or professional analysis.

## Keep It Local Principle

The central question is not:

> **"Should we use AI?"**

It is:

> **"What infrastructure does AI require, who controls that infrastructure, what do we depend upon, and what alternatives or resilience mechanisms do we have?"**

That question applies at many scales:

* an individual;
* a family;
* an artist;
* a small business;
* a community;
* a region;
* a nation.

The same principle applies whether the dependency involves a cloud account, an AI service, a data center, a utility, a transmission system, or a critical supply chain.

> **Use technology where it creates value. Understand the dependencies it creates. Keep what is essential close to home when practical. Build resilience before you need it.**

## Date

Initial research package: **August 28, 2026**

This folder is intended to evolve as authoritative information becomes available.
