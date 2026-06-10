Computer Crimes — Tracking Property in Assist Other Agency Cases

Purpose

This document describes how Computer Crimes involving digital evidence should be recorded in OTIS 2.0. Currently, these incidents are treated as Assist Other Agency (AoA) cases to track property. This guidance recommends either creating a specific nature code or improving AoA workflows to handle digital evidence.

Current Practice

- Investigators create an Assist Other Agency (AoA) case whenever they seize computers, hard drives, mobile devices, or other digital property on behalf of another agency (e.g. FBI, local sheriff). The purpose is to track who took possession of the digital evidence and to whom it was released later.
- The case records basic information about the property, the agency requesting assistance, and the chain of custody.
- There is no dedicated Computer Crimes nature code; digital evidence is managed using the generic AoA nature code.

Recommendations for OTIS 2.0

1. Nature Code: Introduce a new non‑offense nature code (e.g. Computer Crimes Support) to differentiate digital evidence tracking from other AoA cases. This will improve searchability and reporting.
2. Property Fields: Enhance the property tab to capture digital evidence details such as device type, serial numbers, encryption status, forensic imaging status, and location of forensic images.
3. Chain of Custody: Ensure chain‑of‑custody tracking includes who seized the device, who conducted forensic imaging, and who has current possession. Provide a simple interface to document transfers between agencies.
4. Release & Destruction: Support recording when devices are returned to the owner, retained by another agency for prosecution, or destroyed (e.g. due to containing illicit material).
5. Person & Agency Association: The case should allow adding both persons (e.g. suspect, officer) and agencies (e.g. FBI, local PD) to the incident. Use the person role drop‑down to classify individuals appropriately and record agency contact information.

Workflow

1. Incident Creation: Create a non‑offense case with the new Computer Crimes Support nature code or select Assist Other Agency if the nature code does not yet exist. Record additional nature codes as needed.
2. Property Entry: Add each device with detailed description, serial numbers, and imaging status. Attach forensic imaging reports if available.
3. Agency & Person Entry: Add the requesting agency and any involved persons. Assign roles (e.g. Suspect, Owner, Agency Contact).
4. Narrative: Document the circumstances of the seizure, steps taken to secure digital evidence, and interactions with the requesting agency.
5. Transfers & Disposition: Record each transfer of the device. Update the case when the device is returned or destroyed. Provide final disposition notes.

Notes

- Differentiating computer crimes from other AoA cases will clarify reporting and help track trends in digital evidence handling.
- Align property tracking fields with best practices for digital forensics to support future auditing and legal proceedings.
