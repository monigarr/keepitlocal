# Example — A Personal Photo Library

**Scale:** Personal
**Framework applied:** Dependency Model + Infrastructure Stack + Resilience Model + Sovereignty Model, governed by the Evidence Standard
**Model instance:** this analysis; recorded using the [Infrastructure Data Model](../models/infrastructure-data-model.md) concepts

---

## 1. The question

Can I still access, export, and recover my photo library if my current cloud service disappeared tomorrow?

## 2. System boundary

**System under analysis:** One person's photo library — originals, edits, and the software used to view, edit, and sync them.

**Out of scope:** other personal data, work files, and other household members' libraries.

**Failure of the system** = the person permanently loses photos they care about, or cannot access them for an extended period.

## 3. Dependency inventory

| # | Dependency | Type | Owner / Operator | Location | Data involved | Layer | Criticality |
| --- | --- | --- | --- | --- | --- | --- | --- |
| D1 | Cloud photo sync & backup service | service + storage | Vendor | Vendor data centers (documented region) | Original photos, edits | storage / service | HIGH |
| D2 | Phone local storage | hardware + storage | Person | Person's home | Recent originals | storage | MODERATE |
| D3 | Home laptop with photo-editing software | hardware + software | Person | Person's home | Edited library | compute / applications | HIGH |
| D4 | External hard drive (local backup) | hardware + storage | Person | Person's home | Backup copy of library | storage | CRITICAL |
| D5 | Internet connection | network | ISP | Local area | Upload/download traffic | networking | HIGH |
| D6 | Power supply | energy | Utility | Local grid | none | power | CRITICAL |

## 4. Evidence classification

Per the [Evidence Standard](../methodology/EVIDENCE_STANDARD.md), each inventory claim is classified. **UNKNOWN is recorded, not guessed.**

| Claim | Evidence | Classification |
| --- | --- | --- |
| Cloud service stores full-resolution originals | Vendor documentation; account settings | REPORTED (not independently verified) |
| Phone keeps recent originals locally | Person can inspect own device | CONFIRMED |
| Editing software licenses permit local use offline | License terms | CONFIRMED (point-in-time) |
| External drive holds a full backup | Person's own records; last sync date | CONFIRMED |
| Backup is independent of the cloud service | Person's own setup | CONFIRMED |
| Backup is fully up to date | **Unknown** — last verified date not recorded | UNKNOWN |

> The single most important finding is the **UNKNOWN**: whether the backup is actually current. That is not a gap filled by assumption; it is a task.

## 5. Failure modes and resilience

Using the [Resilience Model](../models/resilience-model.md):

| Failure mode | Consequence | Existing measure | Gap |
| --- | --- | --- | --- |
| Cloud service shuts down | Remote access lost | Local phone + drive copies | Dependent on how current they are |
| Cloud account suspended/lost | Same as above | Phone + drive | Laptop & drive also hold copies |
| Phone lost or damaged | Recent photos at risk | Auto-uploaded to cloud | Cloud is a single-path for phone originals |
| Laptop fails | Editing capability lost | Photos remain on drive/cloud | Software restore needed; time-to-recovery not tested |
| External drive fails | Only backup lost | Cloud copy | Drive is single-copy; no second independent backup |
| Internet outage | No sync | Offline access to local copies | Fine for viewing; sync paused |
| Power outage | No access | Laptop battery, UPS not present | Minor for this use; not critical to data |

The key resilience tests:

- **Is any recovery path independent of the primary path?** Yes — the external drive is independent of the cloud (but it is the only backup copy → needs a second independent copy).
- **Can the person operate temporarily without the dependency?** Yes — offline access to local copies.

## 6. Sovereignty

Using the [Sovereignty Model](../models/sovereignty-model.md):

| Dimension | Finding |
| --- | --- |
| Ownership | Originals are owned; cloud copy is licensed under vendor terms (terms not re-read → UNKNOWN at review date) |
| Access | Person has access while service operates and data is current |
| Data control / export | Export capability per vendor; **not yet tested** → UNKNOWN |
| Infrastructure control | Local storage is controlled; cloud storage is not |
| Portability | Depends on export formats; not tested → UNKNOWN |

## 7. Unknowns

- How current is the external-drive backup?
- Can every full-resolution photo be exported from the cloud, in a usable format?
- What do the cloud vendor's terms currently say about data on account cancellation?
- What is the measured time to recover the library from the backup?

## 8. Decision

Concrete next actions, each directly tied to a finding:

1. **Verify the backup** — run the backup, record the date, and store the record (closes the UNKNOWN on D2/D3/D4).
2. **Add a second independent backup** — a second medium not co-located with the first (addresses the single-copy gap in D4).
3. **Test export** — attempt a full export of the library from the cloud (closes the UNKNOWN on #5 rows 1 and 3).
4. **Record recovery time** — time a full restore on a spare laptop (closes the UNKNOWN on recovery).

These follow directly from the [Resilience Model](../models/resilience-model.md) gate: prevent, degrade safely, recover, operate without, replace, export, continue.

## 9. What this example shows

The same five-model sequence — dependency inventory → evidence classification → infrastructure stack → failure/resilience → sovereignty — can be applied to one person's photo library exactly as it is applied to regional infrastructure in the [EO 14420/14421 case study](../research/EO_14420_14421/README.md).

The method did not need to change. Only the boundary and the depth of evidence changed.