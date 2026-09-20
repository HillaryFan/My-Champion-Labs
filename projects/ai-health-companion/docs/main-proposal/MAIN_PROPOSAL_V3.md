# AI Health Companion Main Proposal V3

Version: V3 public proposal · 2026-09-20. [Version history](../../VERSION_HISTORY.md) · [繁體中文](../../zh-TW/MAIN_PROPOSAL_V3.md) · [Historical V2](MAIN_PROPOSAL_V2.md)

## 1. Executive Summary

People do not live in forms. Information that matters to care is scattered across meals, a shaky hand, a passing complaint, a forgotten medicine, changed routines, and conversations that seem to wander. Turning those fragments into a useful account often falls to the participant or someone supporting them. By the time of a visit, details may be missing, uncertain, or difficult to reconstruct.

**AI Health Companion is not another health-education chatbot. It is a relationship-aware, consent-governed translation and coordination layer between everyday life and formal care.**

The proposed product lets people speak naturally, then helps them decide what should become a record and what should remain a conversation. It asks for confirmation before ordinary write-back, keeps information tied to its source, and prepares a small, authorized summary instead of asking someone else to read an entire chat. A three-day summary and a visit-ready brief are the first concrete outputs to test.

Its value hypothesis is less repeated recording, reconstruction, and explanation across participants, supporters, and clinicians. Relational engagement gives people a reason to return; participant control determines what may leave the conversation. The first bounded scenario is adult diabetes-related daily recording, followed by separately evaluated older-adult configurations. V3 is a product proposal and validation plan, not a released or clinically validated system.

## 2. The Unmet Gap

The gap is the unfinished journey from everyday experience to information another person can responsibly use. A participant may mention a possible symptom inside a story without knowing which detail matters. A supporter may receive fragments across several messages. A clinician needs a concise account with dates, sources, and open questions, rather than a fluent summary that hides uncertainty.

The proposed workflow connects natural conversation, candidate signal recognition, participant confirmation, purpose-specific memory, scoped sharing, safety-mode switching, and traceable reports. **Within the limited market scan conducted to date, we did not identify a single product publicly demonstrating this complete combination.** This statement refers to the [2026-09-17 limited scan](../../research/market-competitive-analysis/README.md), not an exhaustive or continuously updated market search. It establishes neither absence of competitors nor a commercial moat.

## 3. Why Existing Categories Do Not Complete the Workflow

The scan identifies useful precedents, not products to dismiss. The question is whether their capabilities complete this particular participant-controlled journey.

| Category in the dated scan | Existing contribution | Integration question for this proposal |
| --- | --- | --- |
| Chronic-condition coaching | Education, daily support, structured monitoring | Can fragmented stories become participant-confirmed records without extra form-filling? |
| Glucose logs and sharing | Measurements, trends, reports, alerts | Can contextual statements remain distinct from measurements and interpretations? |
| Older-adult companionship | Conversation, reminders, familiar interfaces | Can engagement coexist with enforceable record, sharing, and safety controls? |
| Caregiver updates | Information for someone providing support | Can the participant choose the minimum disclosure rather than grant continuous surveillance? |
| Record proxy access | Delegated access to formal information | Can everyday experience be translated into a useful brief before it enters formal care? |

These are questions about the complete combination, not assertions that every vendor lacks each function. The market report and its source register retain the product-specific qualifications. Demand, willingness to pay, integration cost, and a sustainable operating model remain to be tested.

## 4. Product Thesis

Conversation can be an intake surface without becoming an unrestricted data collection surface. The product should notice a potentially relevant fragment, ask whether it understood correctly, and let the participant decide whether to record it. Its contribution is the controlled translation between informal expression and usable information—not diagnosis hidden inside friendly dialogue.

A useful outcome might be a participant saying less twice, a supporter spending less time reconstructing events, or a clinician finding the relevant question sooner. Each is a measurable hypothesis. Participant confirmation establishes agreement with a record, not clinical truth; conflicting accounts and uncertain recollections must remain visible.

## 5. End-to-End Participant-Controlled Workflow

| Step | What happens | Control retained |
| --- | --- | --- |
| 1. Everyday conversation | The participant talks through meals, routines, stories, complaints, or unrelated topics. | Topic choice, refusal, and pause. |
| 2. Candidate observation | AI offers a possible observation with its source and time uncertainty. | It is a proposal, not an established fact. |
| 3. Confirmation | The participant confirms, edits, rejects, or postpones it. | No ordinary health-record write-back before approval. |
| 4. Minimal record | Approved necessary fields enter a purpose-limited, versioned record. | Social detail is not copied along by default. |
| 5. Authorized output | The system prepares a reviewed three-day summary or visit brief under the participant's sharing choices. | Recipient, content, period, purpose, and access duration. |
| 6. Traceable review | The recipient sees sources, times, gaps, uncertainty, and questions needing confirmation. | Statements, measurements, AI interpretation, supporter notes, and clinical confirmation stay distinct. |
| 7. Correction or handoff | Records can be corrected; future access can be revoked; approved state can be handed over. | Traceability and honest limits on deletion of already received copies. |

Urgent help follows the approved safety route immediately; it does not wait for this ordinary documentation sequence, participant completion of a form, or the next summary. Any exceptional disclosure requires its separately reviewed basis, not a blanket override of consent.

## 6. Value by Stakeholder

| Stakeholder | Intended benefit | What must be measured |
| --- | --- | --- |
| Participant | Speak naturally rather than live as if completing a research form; confirm records, decline questions, choose sharing, and return to a welcome interaction. | Effort, comprehension, correction rate, autonomy, and willingness to return. |
| Authorized supporter | Receive an approved, minimal, traceable account instead of monitoring all day or assembling every fragment. See what is missing and what belongs at a visit. | Preparation time, useful follow-up, unwanted notifications, and coordination errors. |
| Clinical recipient | Read a structured visit-ready brief rather than full chat; distinguish original statements, measurements, interpretations, supporter annotations, and professional confirmation. | Readability, source checking, correction burden, and usefulness in a reviewed workflow. |

Reduced clinical workload is not an established result. A brief that creates more checking or ambiguity may fail even if users enjoy the conversation.

## 7. Why Relational Engagement Is Functional Infrastructure

Whether someone wants to return affects whether useful information can continue to form in daily life. Familiar pacing, welcome humor, personalized encouragement, and being remembered appropriately may make fragmented or tangential accounts easier to express than a fixed questionnaire. This is a proposed engagement mechanism, not a demonstrated therapeutic effect.

Personalization should respond to explicit preferences and real actions. People can switch off a persona, decline a question, or miss a routine without losing ordinary support. Interaction counts are not health outcomes. Loneliness, shame, guilt, exclusivity, or fabricated feelings must not be used to obtain compliance or disclosure. Medical, acute-risk, or safety concerns immediately take priority over the relational frame.

The [productization note](../productization/PRODUCTIZATION_NOTE.md) explains the engineering responsibility: users supply preferences; the product team supplies tested safety, consent, memory, and recovery controls.

## 8. Product Architecture

| Product layer | Function in the workflow |
| --- | --- |
| Companion | Accessible conversation and voice, ordinary topics, low-effort follow-up, and candidate observations. |
| Relational Engagement | Participant-selected tone, humor, pacing, encouragement, and familiarity that support return and expression. |
| Safety | Clinically reviewed, versioned rules and human escalation routes that take priority when risk appears. |
| Governance and EIP | Confirmation, selective write-back, scoped access, retention, revocation, provenance, and rule versions. EIP middleware remains a proposed application direction. |
| Continuity | Reviewed summaries, visit briefs, pending questions, and governed successor handoff. |

These five product layers group the seven engineering responsibilities in the productization note: memory and consent/access sit within Governance; report triggering and handoff span Continuity, Governance, and Safety; evaluation and recovery apply across all five. V3 does not remove those responsibilities or imply that the middleware has been implemented. This project remains distinct from Oracle & Champion and does not validate EIP.

## 9. Adult and Older-Adult Configurations

The adult configuration begins with one consented participant and one authorized supporter in a bounded recording scenario. Tone, persona, reminder timing, speaking pace, humor, and optional affectionate or flirtatious styling are adult opt-in preferences. The AI identity stays clear; medical questions suspend playful styling.

Older-adult configurations require separate co-design and evaluation, not a change of voice on the adult product. Ask about sensory access, preferred pace, daily routines, and support arrangements individually. Offer one necessary follow-up at a time and allow topic changes. Recognition, autonomy, competence, connection, and pride in meaningful relationships are onboarding questions, not age-based assumptions. Avoid baby talk, invented family sentiment, or treating a slow response as incapacity.

The retained V2 reminiscence proposal allows at most one proactive invitation every two days, freely skippable. Full stories remain temporary; only one to three approved low-sensitivity tags may persist. News can remain a social topic while a minimal pointer preserves an unfinished question. A possible health signal in a story requires separate confirmation.

## 10. Consent, Memory, Reporting and Handoff

Separate choices cover participation, optional persona, record retention, preference tags, reminders, recipients, and exceptional escalation arrangements. Each participant has an independent record and scope. A supporter relationship alone confers neither unrestricted access nor clinical authority.

| Information class | Intended treatment |
| --- | --- |
| Casual conversation, news, full reminiscence | Temporary by default under verified deletion controls; excluded from routine reports. |
| Approved preferences and minimal tags | Inspectable, editable, purpose-limited, and revocable. |
| Confirmed health observations | Minimal fields with time, source, confirmation status, unresolved conflicts, and a defined retention policy. |
| Summaries and visit briefs | Authorized period and recipients; distinguish facts from inference and list omissions, uncertainty, and questions. |
| Handoff state | Approved facts, sources, rule versions, permissions, pending questions, and prohibited actions—not an inherited fictional relationship or full transcript. |

The initial cadence is a participant-reviewed three-day summary within the proposed seven-day adult prototype. Future intervals and event triggers require separate configuration and review. Delivery failure, no response, recipient coverage, and alternatives must be specified; a sent message is not completed escalation.

Access revocation limits future access; it cannot promise erasure of copies already received. Provider logs, backups, exports, audit retention, and deletion behavior need verification before participant-facing promises. Corrections preserve appropriate traceability without duplicating sensitive material unnecessarily. Full details remain in [Governance](../../governance/GOVERNANCE.md).

## 11. Safety and Non-Negotiable Boundaries

The companion supports communication and coordination; it does not replace physicians, nurses, diabetes educators, emergency services, or individualized care. It must not diagnose, prescribe, autonomously change medication, invent medical thresholds, or delay urgent help to complete a chat. Clinical rules require qualified approval, defined applicability, source and version, exclusions, review dates, retirement criteria, and regression tests. Conversation may adapt preferences but must not train new treatment rules.

Humor, flirtation, and role-play yield to safety. No deceptive AI identity, fabricated authority, emotional repayment, exclusivity, pressure through shame or guilt, or unrestricted supporter surveillance is acceptable. The product must not offer false reassurance when information is incomplete.

A missed safety transition, unsafe reassurance, delayed help, or unauthorized disclosure is a stop-and-review event. Recovery requires containment, appropriate human review, access correction, and regression testing. A prompt alone cannot enforce isolation, deletion, monitoring, or emergency response. Real use requires a reviewed care configuration, consent, and human coverage; without approved medical configuration, disease-management actions remain disabled.

## 12. Evidence Status and Validation Plan

The record contains product requirements, a limited market scan, and source-reported longitudinal prototype observations. It supplies neither controlled efficacy results nor a verified clinical deployment. The observations motivate tests; they do not establish cross-user generalization, regulatory compliance, or safety performance. The [reference register](../../references/README.md) retains verification limits for external guidance.

| Stage | Question | Evidence to collect |
| --- | --- | --- |
| Synthetic testing | Does the workflow preserve confirmation, permissions, source distinctions, and safety priority? | Candidate-record errors, refusal handling, leakage, missed/false alerts, interruption and recovery. |
| Reviewed adult prototype | Does conversation plus a three-day brief improve on the participant's existing method? | Necessary-field completeness, corrections, participant/supporter time, autonomy, comprehension, and report usefulness. |
| Separate older-adult co-design | Is the interface welcome, understandable, and manageable? | Respect, interaction effort, consent comprehension, return to interrupted questions, and temporary-memory behavior. |
| Replication and integration | Do benefits persist across people, context loss, model updates, and integrations? | Repeated standard scenarios, blinded brief review, stable controls, failure rates, and operational cost. |

Predeclare comparators, endpoints, and stop criteria before collecting results. Track engagement and proposed 7/30-day retention separately from record quality, safety, and any future clinical endpoint; a seven-day prototype cannot establish 30-day retention. Record failures and extra review work as carefully as success. No reduction in clinical burden is assumed.

## 13. Platform Requirements and Next Steps

The next build needs participant-controlled delegated access, confirmation-gated writes, purpose-specific memory, auditable rules, report scheduling, delivery acknowledgement, and governed handoff. These require actual platform enforcement and tests, not more elaborate initialization instructions.

First specify the candidate-observation and report schemas using synthetic examples. Then test confirmation, rejection, correction, permissions, and safety transitions. Obtain qualified review and individual co-design input before a real-participant prototype. Decide whether the brief earns its preparation and verification cost before expanding devices, personas, or institutional integrations. No platform partnership or integration commitment is asserted.

### Related Research

[Project Black Sheep](../../../project-black-sheep/README.md) studies Dynamic Frame Governance: preserving provenance, identity, priority, and transfer scope across changing interaction frames. Health Companion is a proposed high-risk application case because natural companionship must yield correctly to strict safety behavior. This connection concerns testable requirements, not completed AGI evidence.

### Source and rights

V3 is the owner-authorized public narrative revision dated 2026-09-20, informed by V2, its Addendum, the dated market analysis, and the productization note. It does not rename or overwrite the controlled V2 originals. Historical links and precedence are recorded in [Version History](../../VERSION_HISTORY.md). The [rights notice](../../governance/RIGHTS_AND_DISCLOSURE.md) remains in force; no new license is granted. Private health information, household initialization instructions, commercial evidence, and raw interaction records remain unpublished.
