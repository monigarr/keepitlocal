# EO 14420 / 14421 — Case Study Index

**Status:** First formal implementation of the Keep It Local framework
**Date:** August 28, 2026

---

## What this case study is

This case study is the **first formal implementation of the Keep It Local systems framework**. It applies the repository's canonical methodology and models to the August 26, 2026 U.S. bulk-power emergency and the Akwesasne / Massena data-center context.

It applies, together:

```text
Evidence Standard
        +
Dependency Model
        +
Infrastructure Stack
        +
Infrastructure Data Model
        +
Resilience Model
        +
Sovereignty Model
```

## Framework mapping

| Framework component | Canonical reference | Case-study implementation |
| --- | --- | --- |
| Evidence Standard | [`methodology/EVIDENCE_STANDARD.md`](../../methodology/EVIDENCE_STANDARD.md) | Classifies every claim in the folder; folder pointer in `EVIDENCE_STANDARD.md` |
| Source Ranking | [`methodology/SOURCE_RANKING.md`](../../methodology/SOURCE_RANKING.md) | Primary-source discipline in docs 04, 05, 07 |
| Research Method | [`methodology/RESEARCH_METHOD.md`](../../methodology/RESEARCH_METHOD.md) | 13-step process applied in docs 03–05 |
| Dependency Model | [`models/dependency-model.md`](../../models/dependency-model.md) | Electrical/data-center dependency inventory in docs 01–04 |
| Infrastructure Stack | [`models/infrastructure-stack.md`](../../models/infrastructure-stack.md) | Grid → facility → compute chain in docs 01, 03, 04 |
| Infrastructure Data Model | [`models/infrastructure-data-model.md`](../../models/infrastructure-data-model.md) | Equipment register in doc 04; evidence log in doc 05 |
| Resilience Model | [`models/resilience-model.md`](../../models/resilience-model.md) | Outage, cyber, supply-chain scenarios in docs 02, 03 |
| Sovereignty Model | [`models/sovereignty-model.md`](../../models/sovereignty-model.md) | Control / ownership / governance questions in docs 02, 06 |

## Mapping the research problem into the framework

```text
POLICY
  ↓
CRITICAL INFRASTRUCTURE
  ↓
ELECTRICAL SYSTEM
  ↓
DATA CENTER
  ↓
AI COMPUTE
  ↓
COMMUNITY DEPENDENCIES
```

For each component, the case study identifies:

- documented facts — classified per the Evidence Standard;
- dependencies — recorded per the Dependency Model;
- infrastructure layer — per the Infrastructure Stack;
- known operators/owners — only where documented;
- unknowns — explicitly listed and left as **UNKNOWN**;
- failure questions — per the Resilience Model;
- resilience questions — per the Resilience Model;
- governance questions — per the Sovereignty Model and the jurisdictional notes in doc 07.

No infrastructure detail is invented. If a component, operator, or relationship is not established, it is recorded as **UNKNOWN** ([Evidence Standard](../../methodology/EVIDENCE_STANDARD.md)).

## Documents in this case study

| Document | Purpose |
| --- | --- |
| [`README.md`](README.md) | Case-study overview and position |
| [`01_EXECUTIVE_ORDER_ANALYSIS.md`](01_EXECUTIVE_ORDER_ANALYSIS.md) | Technical reading of the August 26, 2026 action |
| [`02_AKWESASNE_IMPLICATIONS.md`](02_AKWESASNE_IMPLICATIONS.md) | Akwesasne / Massena context and jurisdiction |
| [`03_CRITICAL_INFRASTRUCTURE_CHECKLIST.md`](03_CRITICAL_INFRASTRUCTURE_CHECKLIST.md) | Reusable checklist for major AI/data-center infrastructure |
| [`04_MASSENA_RESEARCH_FRAMEWORK.md`](04_MASSENA_RESEARCH_FRAMEWORK.md) | Neutral research framework for the Massena context |
| [`05_IMPLEMENTATION_WATCHLIST.md`](05_IMPLEMENTATION_WATCHLIST.md) | Living watchlist for authoritative developments |
| [`06_KEEP_IT_LOCAL_POSITION.md`](06_KEEP_IT_LOCAL_POSITION.md) | Connection to Keep It Local principles |
| [`07_SOURCES_AND_TERMINOLOGY.md`](07_SOURCES_AND_TERMINOLOGY.md) | Sources, terminology, research cautions |
| [`EVIDENCE_STANDARD.md`](EVIDENCE_STANDARD.md) | Pointer to the canonical Evidence Standard |

## Discipline statement

This case study distinguishes:

- Mohawk Council of Akwesasne positions;
- individual community opinions;
- Massena / local government positions;
- New York State policy;
- U.S. federal policy;
- Canadian policy;
- project/developer claims;
- utility information;
- independent analysis.

It does not present these as one unified position. It does not claim that the Executive Order establishes that the Massena-area project is a national-security threat, and it does not imply that the order automatically creates authority over Canadian portions of Akwesasne.