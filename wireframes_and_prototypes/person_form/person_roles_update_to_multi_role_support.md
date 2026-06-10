Person Roles Update — Multi‑Role Support

Purpose

The current OTIS implementation often forces users to choose a single role for each person involved in a case (e.g. victim, suspect, witness, reportee). This is insufficient for complex incidents, such as mental disability cases or traffic‑related violence, where the same individual may simultaneously be a victim and a suspect. This document proposes a multi‑role model for the Person page in OTIS 2.0.

Challenges with Current Roles

- Misleading Labels: In Mental Disability incidents, individuals are not legally victims or suspects, yet OTIS 1 labels them as Reportee on the victim screen.
- Multiple Roles: A person may be both a victim and a suspect in a single incident (e.g. traffic‑related violence). The current design does not accommodate this.
- Limited Roles: Only a fixed set of roles exists, and adding special roles requires development.

Proposed Multi‑Role Drop‑Down

1. Single Person Screen: Replace separate screens for victims, suspects, witnesses, etc. with a single Person page.
2. Role Selection: Provide a multi‑select drop‑down listing all available roles (e.g. Suspect, Arrestee, Victim, Reportee, Witness, Guardian, Agency Contact, Other). Users can select one or more roles for a person.
3. Flexible Role Management: Admins should be able to add new roles without code changes (e.g. Transported, K‑9 Handler).
4. Role Context: Each selected role should display an optional tooltip or definition to guide users on when to select it.
5. Multiple Nature Codes: When an incident has multiple nature codes, allow roles to be associated with specific nature codes if necessary (e.g. person is a victim in one code but a witness in another).
6. Reporting & Search: Update reporting to filter persons by any of their roles. Searches should find a person if they match any role criteria.

Benefits

- Accuracy: Users can correctly describe an individual’s involvement without forcing them into an incorrect category.
- Flexibility: Supports evolving workflows and new case types without redesigning screens.
- Reduced Confusion: Eliminates the need to decide which page to add a person to. Instead, users add the person once and assign roles.

Implementation Considerations

- Data Model: Modify the person-role relationship to store multiple roles per person. Use a join table with person ID, role ID, and optionally nature code ID.
- User Interface: Provide intuitive multi‑select controls with checkboxes. Display selected roles prominently.
- Migration: Develop a migration strategy to map existing single-role entries to the new multi‑role structure.
