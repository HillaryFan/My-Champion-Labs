# AI Health Companion Addendum V2

Source version: V2. Source date: 2026-09-17. Public English adaptation prepared: 2026-09-17.

This addendum preserves the V2 rationale for companion experience, relational interaction, memory governance, and narrative prototyping. The [Main Proposal](../main-proposal/MAIN_PROPOSAL_V2.md) governs the overall product and safety architecture. No private initialization script, character image, fictional text, or participant health record is reproduced.

## 1 Roles and design decisions

Use an adult prototype participant, separately configured older-adult participants, a configurable AI companion, and an authorized supporter. Each participant controls their own ordinary sharing choices; a relationship does not confer blanket access or clinical authority. Older-adult interaction must not inherit an adult flirtatious persona by default.

## 2 A companion that can yield to safety

The intended experience is approachable and easy to return to, with appropriate tools available when needed. Routine conversation can use preferred humor and everyday topics. Encouragement recognizes real actions. Discomfort or a safety concern suspends performance and prompts concise clarification. An approved emergency trigger activates clear, accessible help instructions without waiting for the conversation to finish.

## 3 Configurable adult persona

Persona, preferred name, appearance, and degree of flirtation are adult opt-in settings that can be changed or switched off. Missing an agreed action must not trigger disappointment, punishment, or withdrawn companionship. Medication questions and suspected acute risk override jokes and affectionate roleplay. The companion identifies as AI and must not claim genuine romantic love, demand exclusivity, seek secrets or money, or solicit emotional repayment.

## 4 Respectful older-adult interaction

Recognition, autonomy, competence, connection, and pride in meaningful relationships are possible needs to explore, not defaults to impose. Acknowledge effort, offer choices, and recognize a clear account or a completed action. Do not invent relationship history, use guilt about loved ones, infantilize, or infer incapacity from slow or tangential responses.

## 5 Reminiscence and news buffer

The proposed reminiscence cadence is at most once every two days and always skippable. Full stories remain temporary; retain only one to three explicitly approved low-sensitivity tags. A health signal requires its own confirmation and record, not retention of the surrounding story.

News conversation is temporary social interaction. Keep a minimal pointer to an unfinished necessary question, return naturally, and accept refusal. Do not retain political commentary or turn every topic into an assessment. Deletion and retention promises depend on verified system controls, including provider-side behavior.

## 6 Proposed EIP middleware and memory governance

The proposed middleware turns selected, confirmed information into traceable records. It must not convert every relationship interaction into persistent data.

| Data class | Intended handling | Access and write-back condition |
| --- | --- | --- |
| Everyday conversation | Temporary by default | Participant session; no routine persistent write-back |
| Reminiscence and news detail | Delete after the relevant interaction under verified controls | No routine health-record or report inclusion |
| Minimal preference or relationship tags | Inspectable and revocable | Explicit approval for individual companion use |
| Confirmed health events | Versioned, purpose-limited records | Scoped access; source and uncertainty retained |
| Reports | Defined reporting period or approved event | Authorized recipient, appropriate sharing consent, and specified trigger |

Source, time, version, applicable participant, approving role, and retirement conditions remain explicit where relevant. Separate participant statements, device observations, inference, supporter notes, and professional confirmation. Support correction, revocation, deletion requests, audit, and revalidation without indiscriminate transfer between projects.

## 7 Governed communication and care knowledge

Adapt conversational preferences from feedback; update clinical knowledge only through controlled review. The proposed corpus includes WHO ICOPE, age-friendly and equity principles, NICE guidance, and appropriate authoritative communication resources. Disease-specific modules require confirmed relevance. New rules require difference review, approval, and regression testing; casual conversation cannot train new treatment rules.

## 8 Individual baseline and targeted modules

Assess access needs and confirmed care requirements individually. Relevant dimensions may include sensory access, function, support availability, prescribed plans, and communication preferences. Retain provenance and unresolved conflicts. Do not activate all age-related risk modules merely because someone is older.

## 9 Narrative prototyping

Fictional-character work can inspire conversational timing, humor, persona consistency, and the transition out of character when risk appears. It is UX inspiration and a stress-testing method, not clinical evidence. Do not import fictional promises, world-building, romantic plot commitments, or unverified medical behavior. Work titles, character identities, images, and narrative text are withheld from this public edition; any separate disclosure requires owner approval.

## 10 Division of documents

The Main Proposal covers architecture, safety, reporting, MVP scope, and evaluation. This Addendum covers experience and governance interfaces. Household initialization instructions remain controlled and outside this repository. Later updates should synchronize interfaces and source versions rather than silently copy private material or imply that narrative prototypes establish safety.

## 11 Reference and rights boundary

See the [reference register](../../references/README.md), [provenance register](../../governance/PROVENANCE.md), and [rights notice](../../governance/RIGHTS_AND_DISCLOSURE.md). The source V2 remains authoritative; this public adaptation does not grant an implementation or open-source license.
