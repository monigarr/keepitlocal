# Keep It Local — Sovereignty Model

**Framework version:** 1.0
**Status:** Canonical model
**Component:** Meaningful control
**Related principle:** [`../principles/DATA_SOVEREIGNTY.md`](../principles/DATA_SOVEREIGNTY.md)

---

## 1. Definition

> Sovereignty, in this framework, means **meaningful control** — not isolation, and not a claim of legal jurisdiction.

Sovereignty is the capacity of a person, organization, or community to exercise meaningful control over the systems and dependencies that matter to it. Control is assessed per capability, per layer, and per dependency.

## 2. Sovereignty is layered

Control can exist at many levels, and control at one level does not guarantee control at another:

```text
PHYSICAL
  ↓
INFRASTRUCTURE
  ↓
COMPUTE
  ↓
SOFTWARE
  ↓
DATA
  ↓
MODEL
  ↓
KNOWLEDGE
  ↓
LANGUAGE
  ↓
GOVERNANCE
```

A community that owns an AI model but not the data, or that owns the hardware but not the means to operate it, has only partial sovereignty. The model asks: **which layers do you control, and what would it take to control more of them?**

## 3. Control dimensions

When analyzing sovereignty over a dependency, consider:

| Dimension | Question |
| --- | --- |
| Ownership | Who owns the asset or service? |
| Access | Who can access it, and under what terms? |
| Governance | Who decides how it is changed, operated, and retired? |
| Data control | Who controls the data — export, deletion, custody? |
| Model control | Who controls the models — weights, behavior, deployment? |
| Infrastructure control | Who controls the physical and digital infrastructure? |
| Operational control | Who operates it day to day and during incidents? |
| Portability | Can it move to another owner or location? |
| Jurisdiction | Which jurisdiction governs it, and what does that mean? |
| Language / knowledge control | Who controls the language, knowledge, and culture encoded in the system? |

## 4. Reading sovereignty

Sovereignty questions are answered per layer of the [Infrastructure Stack](infrastructure-stack.md) and per dimension:

| Layer (stack) | Sovereign question |
| --- | --- |
| Knowledge / Data | Can the data be exported, deleted, and recovered locally? |
| Software / Models | Can the software and models be inspected, modified, and self-hosted? |
| Compute | Can compute be operated locally — own hardware, own operator? |
| Storage | Where does data physically live, and who holds the keys? |
| Network | Who provides connectivity, and what happens in an outage? |
| Facility / Power | Who controls the facility and its energy supply? |
| Governance | Who decides, and who bears the consequences? |

## 5. Sovereignty is per dependency

Meaningful control is assessed for each dependency in the [Dependency Model](dependency-model.md):

- who owns it;
- who operates it;
- who governs it;
- what data or capability could be lost;
- what local alternative exists;
- what is needed to recover, substitute, or export.

Sovereignty is therefore a **derived view over the Dependency Model** rather than a separate list of entitlements.

## 6. Cautions

- **Do not make unsupported legal claims.** This model describes meaningful control; it does not assert legal sovereignty or jurisdiction over any system, territory, or community.
- **Ownership is not control.** Legal ownership alone does not guarantee the ability to operate, export, or decide. Operational and governance control matter separately.
- **Control is not isolation.** Using external services is compatible with sovereignty when the dependency is deliberate, recoverable, and substitutable.

## 7. Relationship to the rest of the framework

- [Dependency Model](dependency-model.md) — the dependencies whose control is assessed.
- [Infrastructure Stack](infrastructure-stack.md) — the layers at which control is analyzed.
- [Resilience Model](resilience-model.md) — recovery and substitution are expressions of control.
- [Infrastructure Data Model](infrastructure-data-model.md) — owner/operator/jurisdiction recorded per asset and service.
- Principle: [Data Sovereignty](../principles/DATA_SOVEREIGNTY.md), [Sovereign AI](../principles/SOVEREIGN_AI.md).