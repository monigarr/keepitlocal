# Keep It Local — Research Method

**Framework component:** Methodology
**Applies to:** any system — personal, organizational, technical, AI workload, infrastructure, community, or regional.

---

## Purpose

The research method is a repeatable process for answering the Keep It Local question:

> **What does this system depend on, who controls those dependencies, what happens when they fail, and what alternatives exist?**

It is deliberately scale-neutral. The same process works for a personal photo library, a small business's accounting system, an AI workload, or regional electrical infrastructure. The difference is the system boundary and the depth of evidence, not the method.

This method is governed by the [Evidence Standard](EVIDENCE_STANDARD.md) and the [Source Ranking](SOURCE_RANKING.md).

## The 13 steps

### 1. Define the question

State clearly what you want to understand. A good question is specific and answerable with evidence.

Examples:

- "What does my photo library depend on, and can I access it if a cloud service disappears?"
- "Which electrical and supply-chain dependencies does the proposed high-load facility introduce?"
- "Which external services does this business require to keep operating, and what are the alternatives?"

### 2. Establish the system boundary

Define what is inside the system and what is outside it.

Record:

- the system under analysis;
- its purpose;
- what counts as a failure of the system;
- what is explicitly out of scope.

### 3. Identify dependencies

List the assets, services, organizations, infrastructure components, resources, and external conditions the system depends on. Use the [Dependency Model](../models/dependency-model.md) to structure the list.

For each dependency capture what is known about its type, owner, operator, location, jurisdiction, purpose, and data involved — marking unknowns as **UNKNOWN** rather than guessing.

### 4. Identify primary sources

For each significant dependency, find the best available source. Prefer the highest-ranking source practical per the [Source Ranking](SOURCE_RANKING.md).

### 5. Classify evidence

Classify each significant claim using the [Evidence Standard](EVIDENCE_STANDARD.md):

- **CONFIRMED** — supported by a primary or authoritative source.
- **REPORTED** — reported by a credible secondary source.
- **INFERRED** — derived by reasonable technical reasoning; label the reasoning.
- **HYPOTHESIS** — plausible but unverified; generate a research question.
- **UNKNOWN** — not established by available evidence.

### 6. Build the infrastructure model

Represent the system using the [Infrastructure Stack](../models/infrastructure-stack.md) and the [Infrastructure Data Model](../models/infrastructure-data-model.md). Map where the system and its dependencies sit in the stack and which dependencies cross layers.

### 7. Identify failure modes

For each critical dependency, ask: what happens if this dependency degrades or disappears? Consider outages, security incidents, supply-chain disruption, weather, and regulatory change. Use the [Resilience Model](../models/resilience-model.md).

### 8. Identify resilience options

For each failure mode, document existing and possible resilience mechanisms: prevention, redundancy, backup, recovery, substitution, portability, graceful degradation, offline operation, and local fallback.

### 9. Identify control / sovereignty dimensions

Ask who owns, operates, governs, and can export or recover the system's components. Use the [Sovereignty Model](../models/sovereignty-model.md).

### 10. Identify unknowns

Explicitly record what is not known and what evidence would resolve each unknown. **UNKNOWN is a valid research result**; it is not a gap to be filled by assumption.

### 11. Document limitations

State the boundaries of the analysis: source availability, date sensitivity, jurisdiction limits, and anything this analysis does not establish.

### 12. Publish findings

Present the result in the structure:

- claim / evidence / classification / scope / limitations / open questions.

Use relative links back to the canonical models. Do not present the analysis as regulatory, legal, engineering-certification, or security-findings work unless it actually is.

### 13. Revisit when new evidence appears

Treat the analysis as living. When authoritative sources change, update:

- the evidence classification;
- the affected dependencies and models;
- the unknowns list;
- any conclusions that depended on the changed evidence.

## Scale guidance

| Scale | Typical boundary | Typical evidence depth |
| --- | --- | --- |
| Personal | Devices, accounts, files, subscriptions | Light — personal records + service documentation |
| Organizational | Business-critical systems and workflows | Medium — contracts, APIs, exports, recovery tests |
| AI workload | Model, data, compute, serving stack | Medium — architecture and vendor documentation |
| Infrastructure | Facilities, grid, water, transport, supply chain | Deep — utility filings, regulatory records, engineering docs |
| Community / regional | Essential community services and dependencies | Deep — official records, government and Indigenous-government sources |

The method steps do not change across scales; only depth and rigor change.

## Relationship to other methodology

- [Evidence Standard](EVIDENCE_STANDARD.md) — how claims are classified.
- [Source Ranking](SOURCE_RANKING.md) — which sources to prefer.
- [Research Method](RESEARCH_METHOD.md) — this document.