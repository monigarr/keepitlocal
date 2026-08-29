# Keep It Local — Principle: Local First

## What it means

"Keep It Local" does **not** mean disconnecting from the internet, refusing external infrastructure, or eliminating cloud services.

It means identifying which capabilities should remain **locally accessible, recoverable, exportable, or controllable** where practical.

## Why it matters

Every system depends on something. Some dependencies are appropriate, efficient, or unavoidable. Others become requirements for your ability to operate without being a deliberate choice.

The practical question is:

> **Do I really need this to live somewhere far away in someone else's data center?**

Sometimes the answer is **yes**. Sometimes it is **no**. Sometimes there is a better middle ground.

## What it shapes in the framework

- The [Dependency Model](../models/dependency-model.md) captures whether a dependency is replaceable, portable, exportable, or recoverable locally.
- The [Resilience Model](../models/resilience-model.md) asks whether a system can operate without the dependency.
- The [Sovereignty Model](../models/sovereignty-model.md) asks who controls the dependency.

## Guiding statement

> **Understand your dependencies. Keep what you can. Own what matters. Build alternatives.**

## Related

- [Data Sovereignty](DATA_SOVEREIGNTY.md)
- [Community Resilience](COMMUNITY_RESILIENCE.md)
- [Sovereign AI](SOVEREIGN_AI.md)