Mental Disability Incidents — Non‑Offense Workflow

Purpose

This document captures requirements and recommendations for handling Mental Disability Incidents in OTIS 2.0. These incidents are non‑offense cases that involve persons exhibiting mental health concerns. Troopers must document these interactions, ensure the individual receives appropriate care, and maintain compliance with legal requirements.

Key Considerations

- Multiple Nature Codes: An incident may have up to four nature codes. OTIS should support linking persons, property, vehicles, and narratives to each nature code independently so that data remains logically separated.
- Person Roles: Individuals involved are not legally considered victims and may not fit standard categories such as suspect or witness. OTIS 2.0 should allow a person to have one or more roles selected from a drop‑down (e.g. suspect, arrestee, victim, reportee, witness, other). This avoids mislabeling and allows a person to be both a victim and a suspect if necessary.
- Required Form (HP‑1190): The HP‑1190 Mental Disability Form must be completed whenever this nature code is selected. In OTIS 1 the form downloads as a blank PDF. For OTIS 2.0, allow the form to be completed directly within the system and then printed or exported. A link to a blank form should remain available for agencies that still rely on paper.
- Transport Information: Incidents often involve moving the individual to a hospital or other facility. OTIS should include fields for Transported By and Transported To to record who transported the person and their destination.
- Hospitalization and Patient Documents: Involuntary hospitalization requires various legal documents and forms to be provided to the patient or guardian. OTIS should support uploading scanned documents or generating them as part of the workflow. Troopers need the ability to check off which documents were provided and when.
- Person Page Simplification: Rather than placing the person on a separate “Victim” page and calling them a reportee, OTIS 2.0 should use a single Person page where roles are assigned via drop‑down. This aligns with proposed multi‑role support and avoids misuse of the Victim screen.

Recommended Workflow

1. Incident Creation: Trooper creates an incident with nature code Mental Disability (905) and optionally up to three additional nature codes.
2. Person Entry: Add the individual on the Person page and assign appropriate roles (e.g. Reportee). Record contact details and any known medical information.
3. HP‑1190 Form: Launch the HP‑1190 form within OTIS. Populate required fields and save a PDF version in attachments. Print if needed.
4. Transport Fields: Enter Transported By and Transported To information if the person is taken to a facility.
5. Narrative: Describe circumstances, actions taken, and any legal documents provided (e.g. Rights forms, involuntary commitment paperwork).
6. Property: If any property is taken into custody (e.g. personal belongings), record it on the property tab.
7. Submit Case: Save the case for review. Ensure all required documents are attached and forms completed.

Future Considerations

- Evaluate integration with mental health service providers or hospital systems to reduce duplicate data entry.
- Track outcomes (e.g. voluntary vs. involuntary hospitalization) to inform policy and training.
