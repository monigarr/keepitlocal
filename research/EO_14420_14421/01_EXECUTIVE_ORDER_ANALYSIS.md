# Executive Order 14420 / 14421 — Technical Analysis

> **Framework references:** [Case-study index](00_CASE_STUDY_INDEX.md) · [Infrastructure Stack](../../models/infrastructure-stack.md) · [Evidence Standard](../../methodology/EVIDENCE_STANDARD.md). Classifications below follow the Evidence Standard.

> **Document-number note:** The White House page supplied for this project identifies the action as **Executive Order 14420**. Public references may also identify the same August 26, 2026 action as **Executive Order 14421**. Until the discrepancy is resolved in the official publication record, this repository uses `EO_14420_14421` as the folder name and avoids relying on the number alone.

## 1. What the order does

The August 26, 2026 presidential action declares a national emergency concerning foreign-produced equipment used in the United States bulk-power system.

The stated concern is that foreign actors may exploit vulnerabilities in electrical equipment and associated digital systems, including through malicious remote access or supply-chain disruption.

The order explicitly connects the issue to the growth of:

- advanced manufacturing
- data centers
- artificial intelligence
- defense production

The policy premise is that increasing electricity dependence makes successful attacks or supply disruptions more consequential.

## 2. What falls within the technical scope

The order defines the bulk-power system around interconnected transmission and generation needed for reliability, including transmission lines rated at **69 kV or higher**.

The listed bulk-power equipment includes, among other things:

- substation transformers
- utility-scale and grid-connected inverters
- battery energy storage systems
- UPS systems supporting critical infrastructure
- large and small generators
- voltage regulators
- protective relaying
- metering
- high-voltage circuit breakers
- turbines
- industrial control systems
- remote terminal units
- PLCs
- intelligent electronic devices
- distributed control systems
- safety instrumented systems

The order also directs agencies to consider associated:

- software
- firmware
- remote-access capabilities
- lifecycle maintenance
- update mechanisms
- other supply-chain dependencies

## 3. What the order does NOT establish

The order does not establish that:

- every foreign-made component is prohibited;
- every data center is a national-security threat;
- every large electricity load falls within the bulk-power-system definition;
- the Massena project is prohibited;
- Akwesasne receives new regulatory authority over the Massena project;
- an equipment vendor is a security threat merely because it is foreign;
- the order automatically governs Canadian infrastructure.

The prohibitions are conditional. They depend on determinations made through the implementation process concerning covered foreign entities and unacceptable or undue risks.

## 4. Implementation matters

The Secretary of Energy is directed to develop implementing rules and procedures. The order also provides authority to identify equipment and vendors, impose conditions, and potentially require isolation, monitoring, disconnection, replacement, or removal of equipment presenting unacceptable risks.

The implementation timeline therefore matters.

The repository should be updated when:

- covered foreign entities are identified;
- equipment/vendor lists are published;
- implementing regulations appear;
- licensing procedures appear;
- federal procurement rules change;
- relevant DOE/FERC/NERC actions clarify scope.

## 5. Why this matters to Keep It Local

The important architectural insight is:

**AI infrastructure is not only compute.**

A more complete stack is:

`POWER → TRANSMISSION → SUBSTATION → TRANSFORMER → CONTROL SYSTEMS → UPS/BATTERY → NETWORK → COMPUTE → STORAGE → SOFTWARE → DATA`

The Executive Order is primarily concerned with the lower infrastructure layers, but those layers directly enable modern AI infrastructure.

This makes critical-infrastructure literacy an important component of responsible AI infrastructure planning.

## 6. Research principle

Use the Executive Order as a **question generator and policy context**, not as proof of a specific local allegation.

For each proposed project, determine what is actually known about:

- electrical interconnection
- voltage levels
- substations
- transformers
- backup generation
- batteries/UPS
- control systems
- remote access
- maintenance
- software/firmware
- vendors
- country of manufacture
- ownership/control
- replacement availability
- incident response
- continuity of service

## Primary source

White House presidential action, August 26, 2026:

https://www.whitehouse.gov/presidential-actions/2026/08/declaring-a-national-emergency-to-secure-the-united-states-bulk-power-system/
