Project: Student Directory MVP (Phase 0–1 locked)
Scope (What we are building)

This MVP provides a secure Admin-only student directory that supports:

Admin login required for all access

Create student records

View student list (Active by default)

View student profile

Edit student record

Deactivate student (no hard delete)

Audit logging for create/edit and sensitive changes

Upload and view student photos/documents with private access

Out of scope (Not in MVP)

Classes/sections

Attendance

Parent login

Teacher accounts

Reports

Search & filters

Notifications

Payments

Mobile app

Data fields (Locked)

Required

Internal ID (system-generated, immutable)

Public Student ID (manual, unique)

First name

Last name

Grade/Level

Date of birth

Address

Phone number

Email

Parent/Guardian information

Photos

Documents

Medical/disability information

Status (Active/Inactive)

Created at, Updated at (system timestamps)

Optional

Notes (internal; no sensitive content)

User roles (Locked)

Admin (only role in MVP)

Security rules (Locked)

Login required for all access

No public access

No hard delete for students

Audit logging required:

Student creation

Student edits

Sensitive field changes (medical, docs, photos, guardian/contact fields)

Acceptance Criteria (Definition of Done)
1) Authentication

Admin can log in

Unauthenticated users cannot access any student pages

2) Create Student

Admin can create a student with required fields

Public Student ID must be unique

Clear validation messages appear on invalid input

Student is Active by default

3) Student List

Admin can view a list of Active students

Inactive students are hidden by default

List does not display medical/disability info or document contents

4) Student Profile

Admin can view full student profile

Sensitive data is visible only on profile view (not in list)

5) Edit Student

Admin can edit student fields

Changes are saved correctly

Sensitive field changes are recorded in audit logs

6) Deactivate Student

Admin can deactivate a student

Deactivated students are hidden from default lists

Student record remains accessible to Admin

7) Audit Logs

System records: who, what, when, which student

Audit logs cannot be disabled via the app

8) Files (Photos/Documents)

Admin can upload and view files per student

Files are private (not publicly accessible)

File access is logged

Risks and notes

This MVP stores sensitive data about minors, including medical/disability information and documents. Production use requires strong security hardening, careful access controls, and a clear privacy policy before real deployment.
