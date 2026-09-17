# Consent Data Lifecycle and Safety Governance

Public implementation requirements derived from Main Proposal V2 and Addendum V2. Packaging clarifications specify publication boundaries and distinguish proposed controls from demonstrated capabilities. They do not certify an implementation.

## Consent and decision rights

Seek separate, understandable choices for participation, record retention, optional persona, relationship tags, reminders, reporting recipients, and any exceptional escalation arrangement. Refusal of optional interaction must not remove ordinary support. Explain how to pause, withdraw, correct, export, or request deletion, and the real limits of each action. Consent records and signatures stay nonpublic.

The participant is the primary authority for their ordinary sharing choices. A family or supporter relationship does not itself grant access. Any representative decision arrangement needs a separately reviewed authority basis; do not infer it from age or a diagnosis. The treating team controls approved medical plans; neither the companion nor a nonclinical supporter inherits clinical authority.

## Scoped access

| Role | Intended access | Must not imply |
| --- | --- | --- |
| Participant | Own records and preferences, subject to actual system capabilities | Access to other participants |
| Authorized supporter | Approved reports or fields for specified purposes and duration | Raw-chat access, prescribing authority, or constant availability |
| Clinical reviewer | Agreed clinical material and rule-review responsibilities | Blanket access to social conversation |
| Project designer | Synthetic tests and authorized, minimized evaluation material | Entitlement to household records through authorship |

Enforcement must be technically tested. Folder names in a Git repository do not provide participant-level authorization, even when the repository is private. Sensitive product work, participant data, and commercial evidence require separate access-controlled stores or repositories where different readers are intended.

## Lifecycle requirements

1. Collect only necessary information with purpose and provenance.
2. Hold conversational detail temporarily by default; avoid unnecessary third-party data.
3. Present candidate ordinary health records for participant confirmation.
4. Persist only approved fields and minimal optional tags, with version and access scope.
5. Produce reports under defined triggers and authorized recipients; do not delay urgent help for report completion.
6. Reassess access and consent on changes, correct errors, and retire obsolete rules and records under defined schedules.

Before real use, specify and verify retention periods, deletion mechanisms, provider-side logs, backups, exports, audit records, and recipient copies. A prompt instruction is not evidence of deletion. Explain any conflicts between deletion requests and applicable retention obligations through qualified review. Avoid storing sensitive content inside audit logs merely to prove deletion.

## Safety and knowledge

Only appropriately reviewed, versioned care plans and rules may define medical actions and escalation. No default dose or clinical threshold is supplied by this project. Persona yields to safety. Approved help routes must identify coverage and no-response behavior; a chat notification is not guaranteed monitoring or emergency dispatch.

Medical knowledge changes require provenance, applicability, exclusions, qualified review, regression tests, and retirement conditions. Conversational adaptation must not alter medical rules. Proposed reference sources do not establish product approval, compliance, or clinical benefit.

## Public release controls

Publish only the approved Markdown files and content hashes listed in this project. Exclude original attachments, household initialization text, medication packaging, medical images, private reports, contact details, email screenshots, business correspondence, evidence packages, fiction text, and identity mappings. Do not store those items in public Git history, issues, release attachments, or pull-request discussions.

Use fresh text-only adaptations rather than black boxes over source files. Review for indirect identification through family roles, diagnoses, dates of health events, quotations, and contextual combinations. Source document dates are provenance dates, not participant medical-event dates. Do not represent role replacement as a formal guarantee of anonymity.

On accidental disclosure, stop publication, contain access where possible, notify the owner, and assess Git history, clones, caches, and recipient copies. A later deletion commit does not erase prior exposure.

## Evidence boundary

The project is a proposal and evaluation plan. It does not establish clinical effectiveness, an implemented security model, regulatory status, or EIP validation. Narrative prototyping supports design exploration only. See [rights](RIGHTS_AND_DISCLOSURE.md) and [provenance](PROVENANCE.md).
