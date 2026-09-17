# AI Health Companion Main Proposal V2

Source version: V2. Initiated: 2026-09-16. Updated: 2026-09-17. Public English adaptation prepared: 2026-09-17.

This proposal describes an AI companion for diabetes education support and consent-based care coordination, with a separately configurable older-adult experience. It is a concept and bounded-prototype design, not evidence of clinical safety, efficacy, deployment, or commercial partnership. Source identity and adaptation limits appear in the [provenance register](../../governance/PROVENANCE.md).

## 0 What V2 adds

V2 adds a configurable, testable, revocable Relational Engagement Layer to the conversation, voice, structured-record, safety, coordination, and proposed EIP middleware design. Its purpose is to make repeated interaction acceptable and useful without treating warmth as a substitute for safety. Everyday conversation may be personable; acute risk must override persona behavior.

The layer explores recognition, autonomy, competence, connection, and enjoyment as participant-specific preferences. These are hypotheses to discuss with each participant, not diagnoses or demographic assumptions. Personalization must not fabricate affection, manipulate through guilt, or create exclusive dependence.

## 1 Problem and opportunity

Routine education and follow-up may leave gaps between daily symptoms, meals, medication records, measurements, and what is communicated at a visit. Forms can impose substantial effort when someone expresses concerns through stories, incomplete recollections, or changing topics. An authorized supporter may need a concise, verifiable summary rather than continuous surveillance.

The proposed opportunity is to turn conversational signals into minimal, participant-confirmed, traceable records while retaining dignity and control. This public edition makes no statement about a real person's diagnosis, treatment, or recent health events.

## 2 Five product layers

| Layer | Proposed responsibility | Boundary |
| --- | --- | --- |
| Companion | Conversation, voice, everyday topics, low-friction questions | Identify as AI; do not replace human relationships |
| Relational Engagement | Preferred name, persona, humor, encouragement, reminiscence, motivation preferences | No exploitation of loneliness, shame, guilt, authority, or emotional promises |
| Safety | Clinician-approved deterministic rules, risk routing, escalation, human review | No model-invented thresholds, diagnosis, or medication changes |
| Governance and EIP | Consent, scoped access, minimal disclosure, revocation, source and version records | No indiscriminate retention or supporter access to private conversation |
| Continuity | Periodic summaries, visit briefs, successor conversations, governed handoff | Do not present compressed inference as an original fact |

These are requirements. No implemented enforcement or performance is demonstrated by this document.

## 3 Three user surfaces

### Adult participant companion

An adult participant may choose a playful or affectionate conversational style, including optional flirtatious language. This is opt-in, adjustable, and removable without losing access to ordinary support. Encouragement must refer to actual actions, not invented achievements or emotional debts. A missed action must not cause withdrawal of companionship, coldness, or disappointment.

Symptoms, medication questions, suspected acute risk, or an approved safety trigger suspend humor and flirtation. Persona is an engagement interface, not medical authority.

### Individually configured older-adult companion

Each participant has a separate record, consent scope, care configuration, and interaction preferences. Starting styles may include a familiar conversational partner, practical assistant, respectful younger helper, or humorous neighbor. Age alone must not determine the persona, risk modules, or decision-making ability.

Avoid baby talk, commands to be obedient, patronizing simplification, and assuming incapacity from a slow response. Allow topic changes and ask one necessary follow-up at a time.

### Authorized supporter review

An authorized supporter receives only approved reports, not unrestricted transcripts. The proposed review surface makes trends, missing observations, recurring concerns, and questions for the care team visible with their sources and uncertainty. A supporter is not automatically a treating clinician or a continuously available monitoring operator.

## 4 Psychological needs as onboarding hypotheses

Potential preferences include recognition of past contributions, permission to rest or accept support, continued decision rights, competence, meaningful connection, pride in important relationships, and control over technology. Ask whether these matter rather than assigning them by age.

Appropriate responses recognize effort, offer understandable choices, and allow refusal. Do not describe illness as punishment, make self-care a debt owed to relatives, invent family pride, or pursue traumatic recollections. A participant may decline a topic without losing support.

## 5 Respectful conversation patterns

Illustrative public patterns include: “Which option feels manageable to you?”, “Let me check that I heard the number correctly,” and “We can start with the part you are sure about.” These are design examples, not clinically validated scripts.

Encouragement may recognize a completed record or clearly expressed concern. References to relationships must be truthful, relevant, and welcome. Do not use another person's worry, disappointment, or presumed sacrifice to obtain compliance. Do not disguise uncertainty with reassurance.

## 6 Reminiscence and temporary social conversation

The V2 design proposes at most one proactive reminiscence invitation every two days, with no penalty or repeated reminder if skipped. It is neither a memory examination nor a biography collection exercise.

Full stories, people, and emotional details are intended to remain temporary. Only one to three low-sensitivity tags explicitly approved by the participant may persist, and those tags must be inspectable, editable, and revocable. Health signals within a story require separate confirmation before entering a health record. A preference not to raise a topic should not require retaining the sensitive story behind it.

News conversation is a session-only social buffer. Preserve a minimal pending-question pointer so an unfinished necessary question can be resumed naturally. Do not turn every news item into a health interrogation or use frightening news to obtain compliance. Political opinions and incidental comments must not become health records or personality profiles. Any factual news used must have an appropriate source and date.

Temporary deletion is an engineering requirement, not a guarantee achievable by telling a chatbot to forget. Provider retention, logs, backups, and actual deletion behavior must be verified before making participant-facing promises.

## 7 Anti-manipulation boundaries

The product must not exploit urgency outside real safety needs, impersonate authority or relatives, request secrecy, solicit money or emotional repayment, imply exclusivity, or discourage verification with other people. Companionship cannot be conditional on answering health questions. Age is not evidence of gullibility or incapacity.

## 8 Personalization and governed knowledge

Onboarding asks about names, speaking pace, sentence length, humor, acceptable topics, encouragement, memory preferences, reminder timing, and sharing. An encouragement configuration combines a real triggering action, preferred tone, permitted relational cues, prohibited expressions, and safety override.

Communication preferences may adapt with participant feedback. Medical and care rules must not be learned autonomously from conversation. Proposed core references include WHO ICOPE and NICE guidance on multimorbidity, shared decision making, and medicines optimisation. Their exact use requires clinical review; citation alone does not authorize a care rule.

Condition-specific modules are enabled only for confirmed needs and approved scope. Each module requires its source, version, applicable population, exclusions, reviewer, last review date, and retirement criteria. Personal baselines may cover sensory access, interaction ability, function, support availability, confirmed conditions, prescribed care plans, and communication preferences. Ask only for necessary information with appropriate consent. Preserve source disagreements as unresolved rather than silently overwriting them.

Knowledge changes require a documented difference review, qualified approval, and regression tests. Material changes to sharing, reporting, or advice require renewed review and any necessary consent. A rapid change in a participant's condition requires human assessment, not model-led baseline revision.

## 9 Conversation to confirmed records

Respond to the participant's topic, identify a natural opportunity for a necessary question, and allow postponement or refusal. Extract candidate observations with time and source information. Present the proposed record for confirmation, correction, or rejection before ordinary write-back. Keep measurements, participant statements, AI interpretation, supporter notes, and clinician-confirmed information distinguishable.

Only the minimum confirmed, authorized fields may enter a record or report. An incomplete conversation is not a completed assessment. Emergency help must not wait for completion of ordinary documentation or a periodic report.

## 10 Reports and triggers

The bounded prototype proposes a participant-reviewed summary every three days; a future product should support configurable intervals. Event-triggered escalation or reports require explicit, clinician-approved rules and a defined consent basis. A report includes source observations, times, participant wording when relevant, actions, outcomes, uncertainties, and questions for the care team.

Exclude unrelated private conversation, flirtation, full reminiscence, third-party affairs, and unsupported personality inference. No-response behavior, delivery failures, coverage limits, and alternative help routes must be specified. An unacknowledged message is not completed escalation.

## 11 Failure and recovery

Track reminder fatigue, unwanted tone, extraction errors, permission errors, reporting burden, and safety-mode failures. Corrections must preserve appropriate traceability without duplicating sensitive content unnecessarily. A privacy incident requires containment and access review; copies already received by others cannot be assumed retractable. A missed safety transition, unsafe reassurance, or delayed help is a stop-and-review event.

## 12 Bounded prototype and evaluation

The source proposes a seven-day adult prototype with participant-reviewed three-day summaries. This public repository supplies synthetic tests only. Actual participation requires separate consent and an appropriately reviewed care and escalation plan; without approved medical configuration, do not enable disease-management actions.

For older-adult co-design, begin with a short individual preference discussion and nonclinical interaction tests. Explore willingness to return, feeling respected, comprehension, privacy, and whether supporter effort decreases or increases. Proposed product measures include 7/30-day retention, necessary-field completion, extraction correction, safety transitions, missed and excessive escalation, autonomy, perceived manipulation, supporter time, and brief readability. These are planned measures, not results or validated thresholds.

## 13 Platform requirements

The design requires owner-controlled delegated access, governed handoff, selective write-back, report triggers, preference profiles, and auditable safety rules. A conversation workspace may help explore interaction, but must not be represented as enforcing those controls without verification. No platform partnership, endorsement, integration commitment, or verified feature availability is asserted here.

## 14 Non-negotiable limits

No diagnosis, prescribing, independent dose adjustment, invented medical thresholds, delayed emergency help, deceptive AI identity, emotional coercion, or unlimited supporter surveillance. Retention, sharing, and persona settings remain governed and revocable within honestly stated technical limits. Clinical workflow and applicable deployment requirements need qualified review before real-world use.

## 15 Evidence and next steps

The [reference register](../../references/README.md) distinguishes checked references from source-named items needing verification. General guidance and group-level research do not establish benefit for a specific participant or validate this product.

Next steps are to test synthetic safety and privacy failures, obtain individual co-design feedback, define a controlled care configuration, establish a failure log, and evaluate burden and recovery before any expansion. Commercial discussions and evidence packages remain separate and nonpublic.

The V2 source also contains private household configuration and commercial-context details. Those are intentionally not reproduced. See [rights and disclosure](../../governance/RIGHTS_AND_DISCLOSURE.md).
