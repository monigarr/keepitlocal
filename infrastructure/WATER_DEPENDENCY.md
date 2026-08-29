# Keep It Local — Water Dependency

**Layer:** Infrastructure · **Component:** Water / Cooling
**Dependency types:** `water` · `cooling`
**Research application:** [`research/EO_14420_14421/`](../research/EO_14420_14421/) · [Data Center Checklist](DATA_CENTER_CHECKLIST.md)

## What this document is

A framework-level reference for analyzing **water and cooling as dependencies**. Large digital facilities depend on water for cooling; cooling, in turn, depends on water supply, treatment, discharge, and the energy to pump it.

## The water / cooling chain

```text
FACILITY
   ↓
COOLING SYSTEM (technology: air, evaporative, liquid/direct, recirculating)
   ↓
WATER SUPPLY (source, volume, rates)
   ↓
WATER TREATMENT
   ↓
DISCHARGE / RECYCLING
   ↓
ENVIRONMENTAL CONSTRAINTS (supply availability, temperature, droughts, permits)
```

Cooling technology determines how directly a facility depends on water. Air-cooled designs depend less directly on water than evaporative or liquid-cooled designs. The specific technology is a **documented fact to be established**, not assumed.

## Dependency questions

For any facility or workload with water dependencies:

1. What cooling technology is used?
2. How much water is required (average, peak, annual)?
3. Where does the water come from — municipal supply, surface water, groundwater?
4. What is the source's actual availability and capacity?
5. How is water treated before use and after discharge?
6. What discharge permits or limits apply?
7. How does seasonal or drought conditions affect supply?
8. Who holds the water rights or supply agreements?
9. What are the cumulative effects of all demands on the same source?
10. Who bears the consequences if water is unavailable during a drought or supply failure?

## Accountability question

For water, as for power:

> **Who benefits, who controls the infrastructure, who pays for it, and who bears the consequences when it fails?**

## Discipline reminders

- Cooling technology is established by evidence, not assumed.
- Water demand figures are time-sensitive and should carry dates and classifications per the [Evidence Standard](../methodology/EVIDENCE_STANDARD.md).
- A proposed demand is **not** the same as a confirmed consumption figure.

## Relationship to the framework

- [Infrastructure Stack](../models/infrastructure-stack.md) — the cooling/water layer.
- [Dependency Model](../models/dependency-model.md) — the `water` and `cooling` dependency types.
- [Resilience Model](../models/resilience-model.md) — drought and supply-failure analysis.
- [Community Infrastructure](../community-infrastructure/README.md) — water is a community-level dependency.