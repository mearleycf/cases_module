# OTIS 2.0 — Discovery Synthesis and Persona Foundation Notes

## Purpose of This Document

This document synthesizes discovery findings, workflow observations,
user-role discussions, operational realities, and early persona research
related to the redesign of OTIS 2.0 for the Ohio State Highway Patrol
(OSHP).

This is not intended to be:

- a finalized persona document,
- a finalized requirements document,
- or a finalized workflow specification.

Instead, this is a consolidated operational understanding of:

- who interacts with OTIS,
- how they interact with it,
- what environmental and procedural constraints exist,
- and what patterns are emerging from discovery.

The goal is to preserve and organize the collective understanding gathered
during discovery before narrowing into specific personas, journeys,
workflows, and design solutions.

---

## System Context

### What OTIS Is

OTIS is the Ohio State Highway Patrol’s long-term incident tracking and
records management system.

It is used to document, manage, update, and maintain:

- incidents,
- criminal offense cases,
- non-offense cases,
- citations,
- crashes,
- narratives,
- attachments,
- evidence/property records,
- and long-term case lifecycle activity.

OTIS differs from Motorola PremierOne (P1) in that:

| System | Primary Purpose |
|---|---|
| P1 / PremierOne | Real-time dispatch, call coordination, transient comms |
| OTIS | Long-term docs, records, evidence tracking, lifecycle |

P1 primarily supports the operational response window during and immediately
after a call.

OTIS supports the long-tail lifecycle of incidents and cases, including:

- evidence management,
- narratives,
- case updates,
- records retention,
- public records handling,
- chain of custody,
- and final disposition.

---

## Core Conceptual Model

### Incidents

An OTIS incident is the foundational organizational entity.

An incident may contain:

- persons,
- vehicles,
- locations,
- narratives,
- attachments,
- evidence/property,
- citations,
- crashes,
- and cases.

A single incident may contain:

- multiple citations,
- a crash plus citations,
- a crash plus a case,
- or multiple related forms/modules simultaneously.

---

### Cases

Cases are divided into:

- Criminal Offense Cases
- Non-Offense Cases

Criminal offense cases contain:

- offenses,
- offenders,
- victims,
- and NIBRS-related reporting structures.

Non-offense cases are broader and often operational or administrative in nature.

Examples include:

- recovered property,
- lost property,
- injured person,
- ill person,
- mental disability incidents,
- abandoned vehicles,
- found firearms,
- ODOT-discovered property,
- airport incidents,
- and miscellaneous operational documentation.

---

## Nature Codes

Nature codes are used to classify cases and support:

- analytics,
- categorization,
- operational reporting,
- and workflow identification.

Examples include:

- Recovered Property (795)
- Lost Property Report (797)
- Injured Person (840)
- Ill Person (841)
- Mental Disability-Related Incidents (905)
- Vehicle Seizure (918)
- Assistance to Other Agencies (921)

Nature codes may:

- overlap operationally,
- evolve during a case lifecycle,
- or change as additional information becomes available.

Examples:

- A recovered firearm may later become identified as stolen.
- A non-offense case may later become an offense case.
- A recovered property case may eventually become linked to a criminal investigation.

Current workflows indicate:

- up to four nature codes may be attached to a case,
- but some existing OTIS 1 constraints do not fully reflect operational reality.

---

## Key Operational Insight

OTIS is not simply a report-writing application.

OTIS is a long-term evidentiary and procedural continuity system.

The system supports:

- documentation,
- chain of custody,
- public records compliance,
- legal defensibility,
- operational analytics,
- and multi-actor collaboration over extended timeframes.

Cases may remain active:

- for months,
- or even years.

Cases may evolve repeatedly over time as:

- evidence changes location,
- owners are identified,
- court decisions occur,
- property is destroyed,
- or new investigative information becomes available.

---

## User Role Ecosystem

### Sworn Personnel

Primary operational creators and maintainers of cases.

Responsibilities include:

- creating cases,
- entering offense/non-offense data,
- issuing citations,
- attaching photos/documents,
- writing narratives,
- documenting evidence/property,
- initiating chain-of-custody records,
- identifying forfeiture/use-of-force situations,
- and approving cases.

Operational characteristics:

- frequently mobile,
- highly interrupted,
- working under time pressure,
- balancing officer safety with documentation requirements.

---

### Evidence / Property Sergeants

Responsible for:

- evidence intake,
- evidence storage management,
- updating final storage locations,
- evidence transfers,
- maintaining chain of custody,
- and coordination with external evidence systems.

Evidence workflows often involve:

- temporary lockers,
- permanent storage,
- external crime lab transfers,
- and long-term evidence tracking.

---

### Office of Investigative Services (OIS)

Responsibilities include:

- management of secure/gov cases,
- oversight of sensitive investigations,
- and additional access/security classification handling.

---

### Central Records

Responsibilities include:

- records maintenance,
- document append operations,
- public records handling,
- victim redaction,
- sealing/expungement,
- and records compliance.

Central Records functions are highly governance-oriented.

---

### Crime Lab

Responsibilities include:

- physical evidence intake,
- property custody,
- toxicology/biological processing,
- barcode/property control workflows,
- and chain-of-custody maintenance.

Uses HP-28 property control forms and evidence tracking procedures.

---

### Statistical Analysts

Responsibilities include:

- repository access,
- analytics,
- reporting,
- case corrections,
- e-trace and NIBIN report management,
- and operational data integrity.

---

### Intelligence Analysts

Responsibilities include:

- reviewing case information,
- intelligence gathering,
- and investigative support.

---

### Photo Lab

Responsible for:

- case photo management,
- and evidence-related image handling.

---

## Recovered Property Workflow

### Operational Overview

Recovered property workflows are one of the most operationally complex
non-offense workflows identified during discovery.

Example scenarios include:

- recovered firearms,
- found wallets,
- stolen vehicles,
- narcotics left at abandoned scenes,
- ODOT-found property,
- or unidentified cash/property.

Recovered property workflows may involve:

- multiple agencies,
- long retention periods,
- chain-of-custody documentation,
- court involvement,
- eventual owner recovery,
- or destruction/disposition.

---

### Typical Workflow Lifecycle

#### 1. Initial Discovery

A trooper:

- responds to an incident,
- discovers property,
- photographs/document evidence,
- and creates initial records.

Examples:

- abandoned suspect vehicle,
- found firearm,
- recovered stolen property,
- narcotics,
- wallets,
- identification cards,
- or cash.

---

#### 2. Initial Documentation

Trooper actions include:

- creating OTIS case,
- assigning nature codes,
- entering narratives,
- documenting evidence/property,
- generating HP-28 property forms,
- and attaching photos/documents.

Property may be:

- unknown ownership,
- linked to offenses,
- or entirely non-offense related.

---

#### 3. Temporary Evidence Storage

Property is often:

- temporarily secured at the post,
- placed in temporary lockers,
- and later processed by evidence personnel.

Troopers may not know final evidence destination while in the field.

---

#### 4. Evidence Sergeant Processing

Evidence/property sergeants may:

- move evidence to permanent storage,
- enter data into separate evidence applications,
- update property location information,
- manage storage logistics,
- or coordinate transfers to crime labs.

---

#### 5. LEADS / Identification

Recovered property may be entered into LEADS.

Examples:

- firearms,
- driver licenses,
- wallets,
- stolen vehicles,
- social security cards.

This enables:

- inter-agency visibility,
- owner identification,
- and property recovery coordination.

---

#### 6. Long-Term Disposition

Recovered property may eventually:

- be returned to owners,
- transferred,
- destroyed,
- forfeited,
- or released via court order.

Cases may remain active:

- for months,
- or years.

Examples:

- unclaimed cash,
- recovered firearms,
- found property without ownership information.

---

## Narrative Workflows

Narratives are a critical operational component of OTIS workflows.

Characteristics:

- high volume,
- long-form,
- chronological/journal-style usage,
- and highly relied upon operationally.

Narratives may include:

- scene descriptions,
- investigative notes,
- evidence handling,
- procedural updates,
- and chronological activity tracking.

Operational observations:

- users strongly prefer preserving chronological narrative history,
- users expect audit trails,
- users often use external tools like Microsoft Word or speech-to-text software,
- narratives may be edited over time,
- and narratives are treated similarly to evolving journal entries.

---

## Environmental and Operational Constraints

### Physical Environment

Users may operate:

- in patrol vehicles,
- at crash scenes,
- in severe weather,
- on highways,
- or in physically constrained environments.

Operational limitations include:

- limited workspace,
- mobile hardware,
- poor ergonomics,
- roadside safety concerns,
- and intermittent connectivity.

---

### Cognitive Environment

Users frequently operate under:

- high stress,
- interruptions,
- fatigue,
- split attention,
- and time pressure.

Examples:

- crash scenes,
- roadside exposure,
- combative subjects,
- officer safety concerns,
- evidence handling,
- or emotionally difficult incidents.

---

### Procedural Constraints

OTIS workflows must support:

- CJIS requirements,
- chain-of-custody integrity,
- legal defensibility,
- auditability,
- victim rights,
- and public records compliance.

Errors are not merely inconvenient.

Errors may:

- affect investigations,
- affect legal proceedings,
- create evidentiary problems,
- impact compliance,
- or affect employee performance reviews.

---

## Key Discovery Themes

### 1. Cases Evolve Over Time

OTIS workflows are not linear.

Information changes:

- evidence moves,
- ownership changes,
- cases evolve,
- and classifications may shift over time.

The system must support:

- progressive enrichment,
- incomplete states,
- deferred decisions,
- and evolving operational truth.

---

### 2. Multiple Actors Share Ownership

Cases are touched by:

- troopers,
- supervisors,
- records personnel,
- evidence custodians,
- analysts,
- labs,
- and courts.

OTIS is fundamentally collaborative and lifecycle-oriented.

---

### 3. Long-Term Traceability Is Critical

Operational history matters.

Users require:

- audit trails,
- narrative continuity,
- evidence tracking,
- and historical accountability.

---

### 4. Operational Reality Frequently Defies Rigid Data Models

Discovery revealed multiple examples where:

- workflows do not cleanly fit existing system assumptions,
- operational flexibility is required,
- and users work around system limitations to reflect real-world complexity.

Examples include:

- recovered property associated with offenses,
- evolving case classification,
- and uncertain evidence destinations during initial intake.

---

## Trooper Persona Foundations

### Early Persona Candidate

#### Patrol Trooper / Initial Reporting Officer

Core characteristics:

- initiates cases in uncertain environments,
- gathers incomplete information,
- documents rapidly evolving situations,
- balances safety with procedural accuracy,
- relies heavily on narratives,
- and works across multiple interconnected systems.

Primary goals:

- clear scenes safely,
- document incidents accurately,
- preserve evidence integrity,
- complete reports efficiently,
- and avoid downstream corrections/problems.

Behavioral tendencies:

- highly task-focused,
- prefers predictable workflows,
- values speed and reliability,
- relies on muscle memory,
- and multitasks constantly.

Operational frustrations:

- interruptions,
- uncertainty,
- fragmented workflows,
- procedural burden,
- and administrative complexity.

Emotional concerns:

- fear of mistakes,
- career consequences from system/process failures,
- and frustration when tools create operational risk.

---

## Emerging UX Implications

### OTIS Must Support

#### Progressive Workflow Completion

Users often do not know everything at case creation time.

---

#### Long-Term Case Evolution

Cases may remain active for years.

---

#### Multi-Actor Collaboration

Multiple operational roles interact with the same records.

---

#### Narrative-Centric Workflows

Narratives are operationally critical.

---

#### Operational Flexibility

Real-world incidents do not always fit rigid workflow assumptions.

---

#### Evidentiary Integrity

Chain-of-custody and auditability are foundational.

---

#### High-Stress Environments

Users operate under interruption, fatigue, and time pressure.

---

#### Trustworthy System Behavior

Operational users must trust that:

- data is preserved,
- actions are traceable,
- and workflows behave predictably.

---

## Important Discovery Reminder

Some discovery findings represent:

- OTIS 1 implementation failures,
- legacy architecture limitations,
- or already-resolved redesign problems.

Those findings should not automatically become:

- permanent persona traits,
- or future-state requirements.

However, they still reveal:

- operational priorities,
- emotional pain points,
- environmental realities,
- and workflow truths.

These should continue informing:

- persona development,
- journey mapping,
- workflow modeling,
- and UX prioritization.

---

## Current Strategic Observation

The redesign challenge appears less about:
> "creating forms"

and more about:
> supporting procedural continuity, evidentiary integrity, and evolving
> operational workflows across long-lived multi-actor cases.
