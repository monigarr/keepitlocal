# Keep It Local — Resilience Model

**Framework version:** 1.0
**Status:** Canonical model
**Component:** Failure and recovery
**Application guide:** Data-center checklist in [`../infrastructure/DATA_CENTER_CHECKLIST.md`](../infrastructure/DATA_CENTER_CHECKLIST.md)

---

## 1. Purpose

The Resilience Model defines how to analyze whether a system can fail, degrade, recover, substitute, and continue operating. It supports the [Dependency Model](dependency-model.md) by asking what happens when a dependency fails.

## 2. Definition of resilience

A system is resilient when it can meaningfully answer:

- Can it fail?
- Can it degrade safely?
- Can it recover?
- Can it operate temporarily without the dependency?
- Can the dependency be replaced?
- Can data be exported?
- Can users continue operating?

> **A system is not resilient merely because it has backups.** Backups that depend on the same infrastructure, that cannot be restored, or that leave no way to keep operating are weak resilience.

## 3. Resilience mechanisms

| Mechanism | Question | Example |
| --- | --- | --- |
| Prevention | Can the failure be prevented or its probability reduced? | UPS, surge protection, maintenance, monitoring |
| Redundancy | Is there a parallel component that can take over? | RAID, dual power feeds, second internet link |
| Backup | Is there a copy that can restore state? | Local backup independent of primary provider |
| Recovery | Can the system be restored after failure? | Restore procedure, tested disaster recovery |
| Substitution | Can a different component replace the failed one? | Replace a vendor with an alternative service |
| Portability | Can the function move to another provider or location? | Open formats, exportable data, standard APIs |
| Graceful degradation | Can functionality reduce instead of stopping? | Offline mode, lower-quality fallback, read-only access |
| Offline operation | Can the system operate without external connectivity? | Local files, local inference, local services |
| Local fallback | Is there a local option when remote capability is unavailable? | Local NAS, local compute, local backups |
| Time-to-recovery | How long does recovery take? | Restore-time estimates, replacement lead times |
| Operational continuity | Can essential operations continue through the outage? | Continuity plan, trained staff, offline procedures |

## 4. The resilience question set

For each critical dependency, work through the structure:

1. **Failure modes.** What are the realistic ways this dependency fails? (outage, account loss, vendor change, supply-chain disruption, weather, cyber incident)
2. **Consequence.** What actually stops or degrades if it fails?
3. **Detection.** How would I know it failed?
4. **Recovery path.** How do I get back to normal, and how long does it take?
5. **Interim operation.** Can I keep essential operations running meanwhile — even at reduced function?
6. **Replacement.** Can the dependency be replaced permanently, and with what?
7. **Data continuity.** Can data be exported, retrieved, and restored regardless of the vendor?
8. **Independence of measures.** Does each resilience measure depend on a different system than the one being protected? (A backup in the same cloud is not independent.)

## 5. Degradation levels

A useful shorthand models levels of operational capability:

| Level | Meaning |
| --- | --- |
| **Full** | All functions available, normal performance |
| **Degraded** | Core functions available; some features, performance, or capacity reduced |
| **Minimal** | Only essential functions available; non-essential operations stopped |
| **None** | System cannot operate |

Resilience planning is about which levels are acceptable and how the system moves between them.

## 6. Independent measures

Resilience measures must be **independent** of the failure they protect against. Common hidden dependencies:

- backup stored in the same cloud account as the primary data;
- recovery that requires the same vendor's software;
- backup power sharing the same fuel supply as the grid generator;
- a second network link sharing the same physical route.

Each measure should be checked against the dependency it protects.

## 7. Resilience for infrastructure layers

Because dependencies cross layers of the [Infrastructure Stack](infrastructure-stack.md), resilience analysis should include:

- digital layers (services, software, data);
- facility layers (power, cooling, water);
- physical layers (transmission, generation, supply chain);
- governance layers (who decides, who is accountable, who bears consequences).

A facility's resilience depends as much on its transformer and fuel supply as on its software.

## 8. Relationship to the rest of the framework

- [Dependency Model](dependency-model.md) — the dependencies being analyzed.
- [Infrastructure Stack](infrastructure-stack.md) — where each failure sits in the stack.
- [Infrastructure Data Model](infrastructure-data-model.md) — how failure modes and recovery options are recorded.
- [Sovereignty Model](sovereignty-model.md) — recovery and substitution often depend on who controls the dependency.