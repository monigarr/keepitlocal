# Keep It Local — Dependency Model

**Framework version:** 1.0
**Status:** Canonical model
**Component:** Core model of the framework
**Machine-readable reference:** [`schemas/dependency.schema.json`](schemas/dependency.schema.json)

---

## 1. Definition

> A **dependency** is a relationship in which the operation, availability, integrity, recovery, or continuity of one system depends upon another asset, service, organization, infrastructure component, resource, or external condition.

The Dependency Model is the **core model of Keep It Local**. Every other model supports it: the Infrastructure Stack shows where dependencies sit, the Infrastructure Data Model shows how to record them, the Resilience Model asks what happens when they fail, and the Sovereignty Model asks who controls them.

The model identifies dependency. It does not automatically judge it.

Dependency may be:

- appropriate;
- efficient;
- economically rational;
- unavoidable;
- temporary;
- or unnecessary.

## 2. Dependency dimensions

Each dependency is described along the following dimensions. **UNKNOWN is a valid value** for any dimension — do not fill gaps with assumptions.

| Dimension | Question |
| --- | --- |
| Dependent system | What depends on this? |
| Dependency | What is depended upon? |
| Dependency type | Service, software, hardware, compute, etc. (see §3) |
| Owner | Who owns the dependency? |
| Operator | Who operates it? |
| Geographic location | Where is it located? |
| Jurisdiction | Which jurisdiction governs it? |
| Purpose | What does it provide? |
| Data involved | What data flows through or resides in it? |
| Upstream dependencies | What does the dependency itself depend on? |
| Downstream dependencies | What depends on this dependency downstream? |
| Physical infrastructure | What physical infrastructure is required? |
| Software | What software is involved? |
| Network | What network is involved? |
| Energy | What energy infrastructure is required? |
| Water / cooling | What water or cooling is required? |
| Supply chain | What supply chain supports it? |
| Criticality | LOW / MODERATE / HIGH / CRITICAL ($5) |
| Failure modes | How can it fail? What happens if it fails? |
| Recovery requirements | What is needed to recover? |
| Recovery options | What recovery paths exist? |
| Replaceability | Can it be replaced? With what? |
| Portability | Can the function move to another provider or location? |
| Exportability | Can the data or capability be exported? |
| Local alternatives | What local alternatives exist? |
| Evidence | What source supports the record? |
| Evidence classification | CONFIRMED / REPORTED / INFERRED / HYPOTHESIS / UNKNOWN |
| Confidence | How confident is the record? |
| Unknowns | What remains unknown? |

## 3. Dependency types

Dependencies are categorized by type. A single dependency may involve more than one type (for example, a cloud storage service is both a *service* and *storage*, with an *energy* and *network* component).

```text
service            software           hardware
compute            storage            network
energy             water              cooling
data               model              identity
authentication     payment            communications
human expertise    supplier           geographic
regulatory         governance         supply-chain
```

| Type | Meaning |
| --- | --- |
| Service | A delivered capability (SaaS, API, hosted platform) |
| Software | Software, libraries, operating systems, firmware |
| Hardware | Physical devices and components |
| Compute | Processing resources — CPU, GPU, memory |
| Storage | Persistent data storage |
| Network | Connectivity between systems |
| Energy | Electrical supply and related infrastructure |
| Water | Water supply for cooling or operations |
| Cooling | Cooling systems and their dependencies |
| Data | Datasets and information |
| Model | AI/ML models and their serving infrastructure |
| Identity | Identity systems |
| Authentication | Authentication and access control |
| Payment | Payment, billing, and financial settlement |
| Communications | Voice, messaging, and conferencing services |
| Human expertise | Specialized people and skills |
| Supplier | Organizations supplying goods or services |
| Geographic | Physical location constraints |
| Regulatory | Licenses, permits, and regulatory conditions |
| Governance | Organizational or community governance |
| Supply-chain | The upstream chain that produces and delivers components |

## 4. Dependency relationship

Dependencies are recorded as directed relationships.

```text
SYSTEM A
   │
   │ depends on
   ▼
SYSTEM B
   │
   ├── controlled by
   ├── located at
   ├── supplied by
   ├── powered by
   ├── cooled by
   ├── connected to
   └── recovered through
```

Dependencies can be **direct** or **transitive** (A depends on B, and B depends on C, so A transitively depends on C). The model always records the direct relationship; transitive chains are discovered by following links.

## 5. Dependency criticality

Criticality is a **framework classification**, not a regulatory designation.

| Level | Meaning |
| --- | --- |
| **LOW** | Failure causes minor inconvenience; alternatives are easy. |
| **MODERATE** | Failure causes meaningful disruption; recovery is possible but not trivial. |
| **HIGH** | Failure threatens core operation; recovery is difficult or slow. |
| **CRITICAL** | Failure prevents essential operation; the system cannot function without it. |

Criticality depends on the system under analysis. A dependency that is CRITICAL for one system may be LOW for another.

## 6. Evidence discipline

Every recorded dependency should state what supports it. Classification follows the [Evidence Standard](../methodology/EVIDENCE_STANDARD.md):

- **CONFIRMED** — supported by a primary or authoritative source.
- **REPORTED** — reported by a credible secondary source.
- **INFERRED** — derived by reasonable technical reasoning (label the reasoning).
- **HYPOTHESIS** — plausible but unverified (turns into a research question).
- **UNKNOWN** — not established by available evidence.

> **Potential risk must never be automatically represented as documented risk.**

## 7. Worked mini-example

**System:** A small design studio's file library.

| Dependency | Type | Owner/Operator | Location | Criticality | Failure mode | Recovery option | Evidence |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Cloud file-sync service | Service + storage + network | Vendor | Data center (documented region) | HIGH | Account suspension / service shutdown | Local copy + offline backup | REPORTED (vendor docs) |
| Local NAS | Storage + hardware | Studio | Studio office | CRITICAL | Disk failure | RAID + second backup | CONFIRMED (owned) |
| Internet connection | Network | ISP | Local area | HIGH | Outage | Offline access to working files | CONFIRMED (contract) |
| Power supply | Energy | Utility | Local grid | CRITICAL | Outage | UPS + generator | INFERRED (grid documentation) |

## 8. Relationship to the rest of the framework

- [Infrastructure Stack](infrastructure-stack.md) — where each dependency sits in the layered stack.
- [Infrastructure Data Model](infrastructure-data-model.md) — how to record dependencies as data.
- [Resilience Model](resilience-model.md) — what happens when a dependency fails.
- [Sovereignty Model](sovereignty-model.md) — who controls each dependency.
- [Evidence Standard](../methodology/EVIDENCE_STANDARD.md) — how each record is classified.