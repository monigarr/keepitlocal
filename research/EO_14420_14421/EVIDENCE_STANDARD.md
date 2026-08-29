# Keep It Local — Evidence Standard

## Purpose

The **Keep It Local** project is intended to help people understand technology and infrastructure dependencies without replacing evidence with assumption, speculation, or rhetoric.

This evidence standard establishes a consistent method for documenting claims throughout the repository.

It is particularly important when research concerns:

* artificial intelligence;
* data centers;
* electrical infrastructure;
* cybersecurity;
* critical infrastructure;
* supply chains;
* government policy;
* Indigenous communities;
* environmental impacts;
* public safety;
* and specific companies, facilities, or projects.

## Core Principle

> **Evidence before assertion. Infrastructure before rhetoric. Resilience before dependency.**

Keep It Local should distinguish clearly between what is known, what is reported, what is inferred, and what remains unknown.

The absence of evidence should not automatically be interpreted as evidence of wrongdoing, danger, or negligence.

## Evidence Classifications

Every significant factual or technical claim should be assigned one of the following classifications when practical.

### CONFIRMED

Information directly supported by a primary or authoritative source.

Examples:

* a published government regulation;
* an official Executive Order;
* a utility filing;
* an official planning-board document;
* an official Indigenous-government statement;
* a company's own technical or regulatory filing;
* a published engineering document;
* a court or administrative record.

**Use when:** the underlying source directly establishes the claim.

---

### REPORTED

Information reported by a credible secondary source but not independently established through a primary source.

Examples:

* reputable journalism reporting a project's proposed electrical load;
* an industry publication describing a proposed facility;
* a professional publication summarizing a regulatory proceeding.

**Use when:** the information is credible but the primary documentation has not yet been located or independently verified.

Always identify the reporting source where practical.

---

### INFERRED

A conclusion derived from documented information using reasonable technical or logical reasoning.

Examples:

* identifying a likely infrastructure dependency from documented electrical characteristics;
* identifying a probable relationship between two infrastructure components;
* estimating a consequence based on documented system architecture.

**Use when:** the conclusion is reasonable but is not explicitly stated by the source.

Clearly label the reasoning.

> **Inference must never be presented as a confirmed fact.**

---

### HYPOTHESIS

A technically plausible proposition that requires additional evidence.

Examples:

* a proposed facility may require particular transmission upgrades;
* a particular class of control system may be involved;
* a specific infrastructure dependency may exist but has not been documented.

**Use when:** the question is worth investigating but available evidence is insufficient.

A hypothesis should generate a research question, not a conclusion.

---

### UNKNOWN

Information that has not been established by the available evidence.

Examples:

* manufacturer not identified;
* transformer origin not documented;
* remote-access architecture not disclosed;
* exact water consumption not established;
* cost responsibility not publicly documented.

**Use when:** the correct answer is currently "we do not know."

This is an important research result.

> **UNKNOWN is not a failure. It identifies where additional evidence is needed.**

## Source Hierarchy

When multiple sources are available, prefer evidence in approximately this order:

### 1. Law, regulation, and official government records

Examples:

* statutes;
* regulations;
* Executive Orders;
* agency orders;
* official determinations;
* public regulatory filings.

### 2. Official technical and infrastructure records

Examples:

* utility filings;
* transmission studies;
* interconnection documents;
* engineering reports;
* environmental documents;
* planning-board records.

### 3. Indigenous-government sources

Examples:

* Mohawk Council of Akwesasne statements;
* official Indigenous-government resolutions;
* official consultation documents;
* Indigenous government technical reports.

These sources are particularly important when documenting the position, concerns, jurisdiction, or interests of an Indigenous government.

### 4. Project/developer primary sources

Examples:

* project presentations;
* site plans;
* environmental submissions;
* corporate filings;
* official project websites;
* public statements by project representatives.

These sources should be identified as representing the project's own claims or descriptions.

### 5. Credible secondary reporting

Examples:

* established news organizations;
* recognized trade publications;
* academic reporting;
* professional organizations.

Secondary reporting can provide useful context but should not silently replace primary evidence when primary evidence is available.

### 6. Community and public discussion

Examples:

* public meetings;
* community organizations;
* public comments;
* social-media discussions.

These can be useful for identifying questions, leads, and community concerns.

They should not automatically be treated as factual evidence.

## Claim Construction

When documenting a significant issue, use this structure where practical:

### Claim

What is being asserted?

### Evidence

What source supports the assertion?

### Classification

Is it:

* CONFIRMED
* REPORTED
* INFERRED
* HYPOTHESIS
* UNKNOWN

### Scope

What exactly does the evidence establish?

### Limitations

What does the evidence **not** establish?

### Open Questions

What additional evidence would strengthen, weaken, or resolve the claim?

This structure helps prevent accidental escalation from:

**question → assumption → allegation → "fact."**

## Technical Inference Standard

Technical inference is useful and necessary in infrastructure research.

However, inference should be explicitly separated from documentation.

For example:

> **Documented:** A project proposes a very large electrical load.

> **Reasonable inference:** Supporting infrastructure will need to accommodate that load.

> **Open question:** Which specific transmission, substation, transformer, protection, and control-system upgrades will be required?

The final question should not be answered through assumption merely because the engineering consequence appears obvious.

## Cybersecurity and National-Security Claims

Extra caution is required when discussing cybersecurity or national security.

Do not characterize a:

* company;
* country;
* manufacturer;
* software system;
* control system;
* facility;
* network;
* or piece of equipment

as a security threat solely because it is:

* foreign;
* unfamiliar;
* proprietary;
* connected to a network;
* remotely accessible;
* difficult to inspect;
* or potentially vulnerable.

A documented vulnerability, government determination, technical assessment, or other authoritative evidence should be cited before making a specific security claim.

### Important distinction

**Potential vulnerability ≠ documented vulnerability**

**Foreign origin ≠ malicious intent**

**Remote access ≠ evidence of compromise**

**Large infrastructure ≠ unsafe infrastructure**

**Unknown information ≠ evidence of wrongdoing**

These distinctions are fundamental to responsible public-interest technology research.

## Indigenous and Community Context

Research concerning Akwesasne and other Indigenous communities requires additional care.

Do not collapse:

* the position of an Indigenous government;
* the views of individual community members;
* the position of a developer;
* municipal policy;
* state policy;
* federal policy;
* Canadian policy;
* and the researcher's own analysis

into a single "community position."

Identify whose position is being documented.

Where jurisdiction is discussed, identify the relevant jurisdiction rather than implying that one government's authority automatically extends across all infrastructure or all portions of a cross-border community.

## Conflicting Sources

When credible sources disagree:

1. Do not silently choose the source that supports the preferred conclusion.
2. Identify the disagreement.
3. Determine whether the sources are actually measuring the same thing.
4. Prefer primary records where available.
5. Preserve unresolved disagreement when it cannot be independently resolved.
6. Update the repository when authoritative evidence clarifies the issue.

A disagreement can itself be an important research finding.

## Dates Matter

Infrastructure and policy information changes.

Every significant time-sensitive claim should be associated with a date where practical.

Examples include:

* project capacity;
* proposed construction phases;
* utility capacity;
* regulatory status;
* government policy;
* vendor relationships;
* permits;
* public statements.

Do not present an old proposal as if it were the current state of a project.

## Corrections

If an error is discovered:

1. Correct the document.
2. Preserve the reason for the correction when material.
3. Update related documents if the error affects them.
4. Do not quietly preserve an outdated claim simply because it supports the project's previous argument.

Accuracy is more important than consistency with an earlier conclusion.

## Research Status

For substantial research items, use:

* **OPEN** — investigation is ongoing;
* **VERIFIED** — sufficient authoritative evidence has been located;
* **PARTIALLY VERIFIED** — some elements are established while others remain uncertain;
* **UNRESOLVED** — credible sources conflict or available evidence is insufficient;
* **CLOSED** — research question has been resolved or is no longer relevant.

## The Standard in One Sentence

> **Say what the evidence shows, say what it does not show, label your inferences, preserve uncertainty, and make it possible for another person to independently verify the work.**

That is the evidence standard for Keep It Local.
