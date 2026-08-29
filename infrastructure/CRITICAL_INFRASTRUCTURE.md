# Keep It Local — Critical Infrastructure

**Layer:** Infrastructure · **Component:** Digital / Physical / Energy
**Research application:** [`research/EO_14420_14421/`](../research/EO_14420_14421/)

## What this document is

Critical infrastructure is a **lens**, not a conclusion. This document explains how Keep It Local treats critical infrastructure for analysis: which kinds of systems are commonly involved, what questions to ask, and what discipline to maintain.

It is a framework-level reference. It does not make findings about any specific facility, vendor, technology, or project.

## Systems often considered critical infrastructure

- electrical power generation, transmission, and distribution;
- water and wastewater systems;
- telecommunications and internet;
- data centers and cloud services;
- transportation;
- emergency services;
- financial services;
- government and digital government services;
- supply chains for the above.

A system being "critical" is a **classification concern**, not a legal status. Whether a specific asset is legally classified as critical infrastructure depends on the applicable law and designations.

## The critical-infrastructure question set

For any candidate system, ask:

1. What essential function does it serve?
2. What depends on it?
3. What does it depend on (its own dependencies)?
4. Where does it sit in the [Infrastructure Stack](../models/infrastructure-stack.md)?
5. What happens when it fails? How long is recovery?
6. Who owns and operates it?
7. Who governs it, and who bears the consequences when it fails?
8. What alternatives or substitutes exist?

## Discipline

Critical infrastructure topics attract strong claims. Keep It Local applies the [Evidence Standard](../methodology/EVIDENCE_STANDARD.md) strictly:

- **Large dependency** ≠ **danger**.
- **Unknown information** ≠ **evidence of wrongdoing**.
- **Foreign origin or ownership** ≠ **malicious intent**.
- **Potential vulnerability** ≠ **documented vulnerability**.
- **Critical classification** ≠ **security finding**.

## Relationship to the framework

- [Infrastructure Stack](../models/infrastructure-stack.md) — positions critical assets in layers.
- [Dependency Model](../models/dependency-model.md) — records dependencies of critical systems.
- [Resilience Model](../models/resilience-model.md) — analyzes failure and recovery.
- [Evidence Standard](../methodology/EVIDENCE_STANDARD.md) — governs all claims.
- Research case: [EO 14420/14421 bulk-power analysis](../research/EO_14420_14421/README.md).