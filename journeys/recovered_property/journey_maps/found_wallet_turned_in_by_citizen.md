# OTIS 2.0 Journey Map: Recovered Property (Non-Offense)

## Scenario A: Found Wallet Turned In by Citizen

## Purpose

This journey map documents the current-state business workflow for a recovered property non-offense case involving a wallet turned in by a citizen.

The purpose of this exercise is not to design screens or define requirements. The goal is to understand:

- Who performs each activity
- What information is needed
- What decisions are made
- What handoffs occur
- What questions require additional SME validation

This journey map will serve as a foundation for future:
- Service blueprints
- UX flows
- Requirements gathering
- OTIS workflow design
- Additional discovery activities

---

## Scenario

A traveler approaches an Ohio State Highway Patrol trooper at a turnpike rest area and turns in a wallet containing:

- Cash
- Driver's license
- Credit cards

The trooper must:

- Accept custody of the property
- Determine how the property should be documented
- Create a recovered property case
- Complete HB-28 documentation
- Create a narrative
- Secure the property in temporary evidence storage

The property will later transition to a Property & Evidence Custodian for ongoing management.

---

## Primary Persona

## Recovered Property Reporting Officer

The Reporting Officer is responsible for:

- Initial intake
- Initial documentation
- Property description
- Narrative creation
- HB-28 completion
- Temporary evidence storage

The Reporting Officer establishes the initial record of truth for the property.

---

## Journey Map

| Stage | Property Turned In | Initial Assessment | Case Creation | Property Documentation | HB-28 Completion | Narrative Creation | Temporary Storage | End of Shift / Handoff |
|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| Primary Actor | Reporting Officer | Reporting Officer | Reporting Officer | Reporting Officer | Reporting Officer | Reporting Officer | Reporting Officer | Reporting Officer |
| Action | Citizen turns in wallet | Officer examines contents | Officer creates recovered property case | Officer documents wallet and contents | Officer completes HB-28 | Officer writes narrative | Officer places wallet into temporary locker | Case prepared for downstream processing |
| Information Needed | Finder identity (if willing), location, date/time | Wallet contents, identifying information | Nature code, incident information | Cash amount, cards, ID, property description | Property details, case information | Circumstances of discovery and transfer | Locker location, case number | Case number, locker location |
| Questions | Who found it? Where was it found? | Is owner identifiable? Is anything suspicious? | What type of case should be created? | What must be documented individually? | What information is required on HB-28? | What facts should be preserved? | Which locker should be used? | Is everything ready for handoff? |
| Decisions | Accept property? | Standard recovered property? | Recovered Property nature code? | Single item or multiple items? | How should property be recorded? | What level of detail is needed? | Property secured? | Ready for handoff? |
| Output | Property in OSHP custody | Property evaluated | Recovered property case exists | Property inventory documented | HB-28 completed | Narrative recorded | Property secured | Case ready for next actor |

---

## What Happens Next?

The Reporting Officer's workflow ends.

The property transitions into the Property & Evidence Custodian workflow.

Typical future activities may include:

1. Removal from temporary evidence storage
2. Entry into evidence management system
3. Assignment to permanent storage
4. Owner identification efforts
5. LEADS entry (if applicable)
6. Owner notification
7. Property return
8. Property disposition if unclaimed

---

## Information We Believe To Be True

Based on current discovery findings:

- Recovered Property is a non-offense workflow
- Property may exist independently of criminal offenses
- Property is initially placed into temporary evidence storage
- Property is later removed by a Property & Evidence Custodian
- Custodians are responsible for ongoing property management
- HB-28 forms are used to document property and support chain of custody
- Cases may remain active for extended periods of time
- Property may eventually be:
  - Returned
  - Destroyed
  - Forfeited
  - Transferred
  - Retained

---

## Open Questions For SMEs

## Owner Identification

- Is a driver's license sufficient for owner identification?
- Is LEADS used during this process?
- Are additional systems involved?

## Finder Information

- Is the finder always recorded?
- Can the finder remain anonymous?

## Property Documentation

- Is cash documented separately from the wallet?
- Are credit cards documented individually?
- Is there a threshold where itemization requirements change?

## HB-28

- Does one HB-28 cover the entire wallet?
- Are multiple property entries created?

## Notifications

- Who is responsible for contacting the owner?
- Reporting Officer?
- Property & Evidence Custodian?
- Someone else?

## Disposition

- What happens if the wallet is never claimed?
- Does the finder have any rights to the property?
- Is court involvement required?

---

## Early UX Observations

Even without extensive friction data, several workflow needs are already apparent.

## Preserve User Work

Users should not lose narratives or documentation because of:

- Navigation mistakes
- Connectivity interruptions
- Device failures
- Session timeouts

## Support Incomplete Information

Reporting Officers frequently begin cases without knowing:

- Property ownership
- Final storage location
- Final disposition

The workflow should support progressive completion.

## Reduce Rework

Users consistently express a desire to:

- Get things right the first time
- Avoid corrections
- Avoid revisiting completed work

## Improve Handoff Quality

The quality of downstream work depends heavily on:

- Accurate narratives
- Accurate property descriptions
- Complete documentation

---

## Future Journey Maps

This scenario intentionally represents a relatively simple recovered property workflow.

Additional journey maps should include:

## Scenario B
Recovered Property from Abandoned Vehicle After Pursuit

Examples:
- Firearms
- Narcotics
- Personal property
- Unknown ownership

This scenario introduces:

- Criminal context
- Multiple evidence items
- Photography requirements
- Expanded chain-of-custody complexity
- Potential crime lab involvement

This second journey map will help validate that the workflow scales from simple property recovery to complex evidence recovery situations.
