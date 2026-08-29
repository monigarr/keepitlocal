# Keep It Local — Principle: Data Sovereignty

## What it means

Data sovereignty is **meaningful control over data** — not isolation, and not merely "data residency."

Meaningful control means being able to answer:

- Who can access this data?
- Who can change it?
- Who can delete it?
- Can I export it in a usable format?
- Can I continue to use it if the service that holds it disappears?
- Can I back it up to something I control?

## Why it matters

Data sits at the center of most digital dependencies. A person, business, or community that cannot export, back up, or recover its own data is dependent in a way that ownership of hardware alone does not fix.

Sovereignty over data is **layered**. It can exist at the level of physical storage, the application, the format, the key, and the governance of access. Control at one layer does not guarantee control at another.

## What it shapes in the framework

- The [Dependency Model](../models/dependency-model.md) records the data involved in each dependency and whether it is exportable and portable.
- The [Sovereignty Model](../models/sovereignty-model.md) treats data control as one of its core dimensions.
- The [Resilience Model](../models/resilience-model.md) requires that backups and recovery not depend on the same external system as the primary data.

## Practical guidance

- Prefer open, portable formats where possible.
- Maintain at least one local backup that does not depend on the same external infrastructure.
- Test whether you can export what you store.
- Keep credentials, encryption keys, and configurations under your own control where practical.

## Related

- [Local First](LOCAL_FIRST.md)
- [Sovereign AI](SOVEREIGN_AI.md)
- [Community Resilience](COMMUNITY_RESILIENCE.md)