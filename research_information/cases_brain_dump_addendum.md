Cases Brain Dump — Addendum for Non‑Offense Workflows

This addendum supplements the original cases_brain_dump.md with new discovery findings related to non‑offense nature codes. It highlights additional requirements and points to more detailed workflow documents.

Support for Multiple Nature Codes

- An incident may have up to four nature codes. OTIS must allow persons, property, vehicles, and narratives to be associated with specific nature codes. This enables clear separation when multiple activities occur within a single incident.

Mental Disability Incidents (905)

- A person is always involved, but the role may not be “victim,” “suspect,” or “witness.”
- The HP‑1190 Mental Disability Form is required. OTIS 2.0 should support completing this form within the system and include fields for transport information (transported by, transported to).
- See Mental Disability Incidents — Non‑Offense Workflow for details.

Lost Property Report (797)

- Handles property lost by OSP personnel or the public when no crime is suspected.
- May not involve a person, but the system should allow adding one (e.g. officer who lost property).
- Certain items (e.g. badge, firearm) require LEADS entry. See Lost Property Report — Non‑Offense Workflow.

Aircraft Investigations / Violations (870)

- Involve FAA investigation numbers, extensive documentation, and may not always result in an OTIS case.
- OTIS should allow attaching Aircraft Crash Report forms and uploading photos. See Aircraft Investigations — Non‑Offense Workflow.

Computer Crimes / Assist Other Agency (919, 921)

- Digital evidence is currently tracked as an “Assist Other Agency” case. A dedicated Computer Crimes Support nature code is recommended.
- See Computer Crimes — Tracking Property in Assist Other Agency Cases and Assist Other Agency — Standard Workflow.

Cash / Currency Seizure (919)

- Cases involve equitable sharing among participating task forces and require detailed property and agency tracking.
- See Cash / Currency Seizure — Non‑Offense Workflow.

Pupil Transportation Violation (914)

- Covers various violations during school bus operations or inspections.
- Requires fields for driver, school district, violation type, and corrective actions. See Pupil Transportation Violation — Non‑Offense Workflow.

Property Across Non‑Offense Workflows

- Property management should be available on all non‑offense cases, not just recovered property. See Property Management Across Non‑Offense Workflows.

Person Roles

- Introduce a multi‑role drop‑down for persons so that individuals can be both victims and suspects, or assume other roles such as reportee or witness. See Person Roles Update — Multi‑Role Support.

Miscellaneous Codes

- Several rarely used codes (Lost/Stolen Division Evidence, Bait Vehicle Deployment, Institutional K‑9 Sweeps, Motor Vehicle Fire, etc.) are documented in Miscellaneous Non‑Offense Codes — Additional Notes. These codes may be candidates for deprecation or redesign.

⸻

These additions should be cross‑referenced in the main cases_brain_dump.md to ensure a holistic understanding of non‑offense cases in OTIS 2.0.
