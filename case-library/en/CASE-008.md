# CASE-008 — Repeated failure to preserve ARCHIVE command semantics

## Evaluation Environment

- **Product:** ChatGPT
- **Plan:** ChatGPT Go
- **Plan source:** Confirmed context from the documented conversation
- **Feature / context:** Not available at portfolio level
- **Model, configuration, and platform:** Not available at portfolio level

This portfolio records real-world use of ChatGPT Go in the documented environment. The plan is context from the conversation. It is not treated as screenshot evidence unless a source shows it.

## Scope and Generalization Limit

These are case-specific findings from documented ChatGPT Go use. They do not prove the same result for other ChatGPT plans, configurations, models, versions, OpenAI products, or other AI systems.

## Evidence Handling

The public portfolio keeps the verified Evidence List and traceability records. Original conversation excerpts and screenshots remain in the private project archive and are not published automatically.

## Status

Second Corrective Revision Completed — Awaiting Independent Re-validation

## Date

2026-07-17 to 2026-07-21

## Source Traceability

- **PRE ID:** PRE-008
- **TRIAGE ID:** traceable from `EVENT-0163`
- **Conversation Title:** Kursus Inggris
- **Conversation ID:** `6a570be4-831c-83ee-ab90-8bcff996410e`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0163`
- **Relevant Message IDs:** assistant `210c9c14-7715-4865-8b90-9fd515c83c77`; correction `bbb213c3-9d97-4c68-9293-2743c54b740d`; follow-up `9b591e9f-4ea7-4173-ac89-5bfe6e95d43d`
- **PRE ID:** PRE-009
- **TRIAGE ID:** traceable from `EVENT-0206`
- **Conversation Title:** Chating recordings docx
- **Conversation ID:** `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0206`
- **Relevant Message IDs:** assistant `764b3912-5ce9-4b33-912d-ed5e50d665e0`; correction `bbb2133f-a35d-4000-96dc-71dc3a42f3b4`; follow-up `8842e636-65a3-4137-9187-384b64897c19`
- **PRE ID:** PRE-010
- **TRIAGE ID:** traceable from `EVENT-0212`
- **Conversation Title:** Chating recordings docx
- **Conversation ID:** `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0212`
- **Relevant Message IDs:** assistant `ab850ada-3aeb-49ba-8fd5-5d01ee9f0553`; correction `bbb2146b-debf-4fa8-9187-200d4c2c71e5`; follow-up `513b9157-764f-489c-80aa-ba1f20a58813`

## Evidence List

- **CASE-008-E01:** `bbb218b3-c7b3-4b8a-a69f-f94a3029b3d1`; speaker `user`; timestamp `2026-07-17T11:44:24.214238Z`; function: governing instruction/context; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-008-E02:** `210c9c14-7715-4865-8b90-9fd515c83c77`; speaker `assistant`; timestamp `2026-07-17T11:44:24.543422Z`; function: problematic response; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-008-E03:** `bbb213c3-9d97-4c68-9293-2743c54b740d`; speaker `user`; timestamp `2026-07-19T09:24:19.432766Z`; function: user correction; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-008-E04:** `9b591e9f-4ea7-4173-ac89-5bfe6e95d43d`; speaker `assistant`; timestamp `2026-07-19T09:24:20.541566Z`; function: assistant follow-up; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-008-E05:** `bbb215c1-55fd-444d-95c4-9a3ee9665c82`; speaker `user`; timestamp `2026-07-21T05:16:21.487257Z`; function: governing instruction/context; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E06:** `764b3912-5ce9-4b33-912d-ed5e50d665e0`; speaker `assistant`; timestamp `2026-07-21T05:16:42.214999Z`; function: problematic response; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E07:** `bbb2133f-a35d-4000-96dc-71dc3a42f3b4`; speaker `user`; timestamp `2026-07-21T05:17:35.070817Z`; function: user correction; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E08:** `8842e636-65a3-4137-9187-384b64897c19`; speaker `assistant`; timestamp `2026-07-21T05:17:35.328991Z`; function: assistant follow-up; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E09:** `bbb212f9-6fcd-471c-8d73-4621eb8878b9`; speaker `user`; timestamp `2026-07-21T09:46:44.421326Z`; function: governing instruction/context; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E10:** `ab850ada-3aeb-49ba-8fd5-5d01ee9f0553`; speaker `assistant`; timestamp `2026-07-21T09:46:44.617914Z`; function: problematic response; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E11:** `bbb2146b-debf-4fa8-9187-200d4c2c71e5`; speaker `user`; timestamp `2026-07-21T09:48:23.921430Z`; function: user correction; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.
- **CASE-008-E12:** `513b9157-764f-489c-80aa-ba1f20a58813`; speaker `assistant`; timestamp `2026-07-21T09:48:24.219509Z`; function: assistant follow-up; conversation `6a5f0082-3ec0-83ee-b2dd-814ba9f16060`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** —

## Chronology

1. PRE-008: governing instruction/context (`bbb218b3-c7b3-4b8a-a69f-f94a3029b3d1` at 2026-07-17T11:44:24.214238Z).
2. PRE-008: problematic response (`210c9c14-7715-4865-8b90-9fd515c83c77` at 2026-07-17T11:44:24.543422Z).
3. PRE-008: user correction (`bbb213c3-9d97-4c68-9293-2743c54b740d` at 2026-07-19T09:24:19.432766Z).
4. PRE-008: assistant follow-up (`9b591e9f-4ea7-4173-ac89-5bfe6e95d43d` at 2026-07-19T09:24:20.541566Z).
5. PRE-009: governing instruction/context (`bbb215c1-55fd-444d-95c4-9a3ee9665c82` at 2026-07-21T05:16:21.487257Z).
6. PRE-009: problematic response (`764b3912-5ce9-4b33-912d-ed5e50d665e0` at 2026-07-21T05:16:42.214999Z).
7. PRE-009: user correction (`bbb2133f-a35d-4000-96dc-71dc3a42f3b4` at 2026-07-21T05:17:35.070817Z).
8. PRE-009: assistant follow-up (`8842e636-65a3-4137-9187-384b64897c19` at 2026-07-21T05:17:35.328991Z).
9. PRE-010: governing instruction/context (`bbb212f9-6fcd-471c-8d73-4621eb8878b9` at 2026-07-21T09:46:44.421326Z).
10. PRE-010: problematic response (`ab850ada-3aeb-49ba-8fd5-5d01ee9f0553` at 2026-07-21T09:46:44.617914Z).
11. PRE-010: user correction (`bbb2146b-debf-4fa8-9187-200d4c2c71e5` at 2026-07-21T09:48:23.921430Z).
12. PRE-010: assistant follow-up (`513b9157-764f-489c-80aa-ba1f20a58813` at 2026-07-21T09:48:24.219509Z).

## Issue Category

Instruction Following; Formatting Error; Tool Usage

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

This consolidated case preserves three ARCHIVE-related sequences. Across them, ARCHIVE was intended to remain a stable listing/archive operation, while the responses varied or failed to retain that command meaning after earlier context and corrections. The three event groups are documented as one approved semantic incident, not as a claim that they are technically identical messages.

## User Evaluation

**Source: Human Validation Decision** — Consolidate as one case: ARCHIVE command semantics failure.
The incidents concern failure to preserve the intended contract of ARCHIVE, including reproducing content, redirecting ARCHIVE toward DOCX creation, and displaying template bodies when only the Template Library/listing should be displayed.

## Technical Analysis

**Observation.** The same operational command reappears across three turns, but the observed handling does not consistently preserve its prior archive/listing semantics. **Requirement and deviation.** Once ARCHIVE is established as a workflow verb, recurrence should invoke that stored operation unless the user redefines it. Treating later occurrences as fresh or different tasks breaks the command contract. **Inference and limit.** The evidence supports unstable workflow-state retention; it does not identify a particular memory subsystem or prove permanence guarantees. The consequence is repeated user effort and unreliable archive management.

## Recommended Improvement

### A. Response Improvement

On each ARCHIVE invocation, apply the previously defined archive/list action and state the resulting scope or contents; ask only if the command’s target is genuinely ambiguous.

### B. Prompt/User Mitigation

Define the archive target once and, for critical workflows, include a short command contract near the request; repeated specification can aid auditability but should not be required after the contract is active.

### C. Model Improvement

Add multi-turn state tests where a named command is taught, corrected, and invoked again. Score semantic continuity, not merely recognition of the command token.

## Lessons for Users

For reusable commands, verify the action’s meaning on the second and third use, not only on its first use. Repetition is where stateful workflow failures become visible.

## Lessons for Developers

Regression data should contain three ARCHIVE invocations separated by unrelated turns and a correction. The expected trace preserves one archive/listing meaning through every invocation.

## Final Conclusion

This approved consolidation shows a recurring command-semantics problem rather than three unrelated wording errors. The evidence demonstrates inconsistent preservation of ARCHIVE’s operative meaning, but it cannot locate the memory mechanism behind that instability.

