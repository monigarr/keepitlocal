# Keep It Local — Energy Dependency

**Layer:** Infrastructure · **Component:** Energy
**Dependency type:** `energy`
**Research application:** [`research/EO_14420_14421/`](../research/EO_14420_14421/) · [Data Center Checklist](DATA_CENTER_CHECKLIST.md)

## What this document is

A framework-level reference for analyzing **energy as a dependency**: how digital systems depend on electricity, and how that dependence runs down the stack to generation, transmission, and supply chains.

## The energy chain

Energy dependencies run from the load down to the source:

```text
FACILITY / WORKLOAD
   ↓
FACILITY POWER DISTRIBUTION (feeders, switchgear, UPS, battery)
   ↓
SUBSTATION
   ↓
TRANSMISSION
   ↓
GENERATION
   ↓
FUEL / SUPPLY CHAIN
```

An AI workload depends on compute; compute depends on the facility; the facility depends on power distribution; power distribution depends on the substation, transmission, and generation.

## Dependency questions

For any system that consumes power:

1. What is the electrical load (average, peak, phased)?
2. Which utility serves it?
3. Which substations and transmission facilities are involved?
4. What voltage levels apply?
5. What generation backs the system, and under what conditions?
6. What backup power exists — UPS, battery, generator — and for how long?
7. What fuel does backup power require, and who supplies it?
8. How is the load expected to grow over time?
9. Who owns and operates each element of the chain?
10. Who bears the consequences when power fails?

## Bulk-power relevance

For very large loads — such as hyperscale data centers — portions of the serving chain may intersect the **bulk-power system** (in the United States, transmission rated at 69 kV and higher, plus related generation and control systems).

Whether any specific facility or component falls within the bulk-power definition is a question of the applicable rules and records. Per the [Evidence Standard](../methodology/EVIDENCE_STANDARD.md), do not assume a classification that has not been documented.

## Discipline reminders

- A large electricity load is **not**, by itself, evidence of an unsafe grid condition.
- An inference about required grid upgrades is **not** a documented transmission study.
- Energy dependency is recorded; whether it is appropriate, risky, or unnecessary is determined per case with evidence.

## Relationship to the framework

- [Infrastructure Stack](../models/infrastructure-stack.md) — the power layer and its dependencies.
- [Dependency Model](../models/dependency-model.md) — the `energy` dependency type.
- [Resilience Model](../models/resilience-model.md) — outage and recovery analysis.
- [Sovereignty Model](../models/sovereignty-model.md) — who controls generation, transmission, and backup.