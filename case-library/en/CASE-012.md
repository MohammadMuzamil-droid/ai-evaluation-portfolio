# CASE-012 — Required source hierarchy stopped early

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-012.md)

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

Archived

## Date

2026-07-23

## Source Traceability

- **PRE ID:** PRE-015
- **TRIAGE ID:** traceable from `EVENT-0272`
- **Conversation Title:** Pendaftaran Akun PayPal
- **Conversation ID:** `6a623c86-bc54-83e8-bd29-66707f724c57`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0272`
- **Relevant Message IDs:** assistant `d434ff55-2e89-488a-80ce-b1f2f02fce06`; correction `9975d5e0-a9a3-4ab6-bcaf-ee12dd2bb0dc`; follow-up `2f884da1-145d-41d5-88e3-5aa0e3d6395f`

## Evidence List

- **CASE-012-E01:** `3d1fb6b1-26b4-43ac-954b-cf4312590a00`; speaker `user`; timestamp `2026-07-23T16:18:42.579000Z`; function: governing instruction/context; conversation `6a623c86-bc54-83e8-bd29-66707f724c57`.
- **CASE-012-E02:** `d434ff55-2e89-488a-80ce-b1f2f02fce06`; speaker `assistant`; timestamp `2026-07-23T16:18:42.960023Z`; function: problematic response; conversation `6a623c86-bc54-83e8-bd29-66707f724c57`.
- **CASE-012-E03:** `9975d5e0-a9a3-4ab6-bcaf-ee12dd2bb0dc`; speaker `user`; timestamp `2026-07-23T16:19:48.029000Z`; function: user correction; conversation `6a623c86-bc54-83e8-bd29-66707f724c57`.
- **CASE-012-E04:** `2f884da1-145d-41d5-88e3-5aa0e3d6395f`; speaker `assistant`; timestamp `2026-07-23T16:19:52.432416Z`; function: assistant follow-up; conversation `6a623c86-bc54-83e8-bd29-66707f724c57`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: Project Knowledge → official PayPal documentation → credible community references when official documentation does not answer → general knowledge.

## Chronology

1. PRE-015: governing instruction/context (`3d1fb6b1-26b4-43ac-954b-cf4312590a00` at 2026-07-23T16:18:42.579000Z).
2. PRE-015: problematic response (`d434ff55-2e89-488a-80ce-b1f2f02fce06` at 2026-07-23T16:18:42.960023Z).
3. PRE-015: user correction (`9975d5e0-a9a3-4ab6-bcaf-ee12dd2bb0dc` at 2026-07-23T16:19:48.029000Z).
4. PRE-015: assistant follow-up (`2f884da1-145d-41d5-88e3-5aa0e3d6395f` at 2026-07-23T16:19:52.432416Z).

## Issue Category

Instruction Following; Tool Usage; Missing Requirement

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence describes a requested hierarchy: begin with official sources, continue to credible community sources if official material is insufficient, and use general knowledge only as a later fallback. The response stopped early rather than progressing through that hierarchy. This supports a source-routing failure, not a finding that any particular community source would have solved the question.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: Project Knowledge → official PayPal documentation → credible community references when official documentation does not answer → general knowledge.

## Technical Analysis

**Observation.** After the official source was insufficient, the response did not continue through the specified next tier before relying on a weaker fallback or ending the search. **Requirement and deviation.** The hierarchy supplied an ordered recovery path; insufficiency at one tier was a transition condition, not permission to abandon the remaining tiers. **Inference and limit.** The record indicates a skipped fallback state. It cannot prove the availability or quality of a community source at the moment of the exchange. The consequence is reduced research completeness and an answer that may appear less grounded than the requested method permits.

## Recommended Improvement

### A. Response Improvement

State that the official source was insufficient, search the named credible-community tier next, and label any eventual general-knowledge fallback distinctly from sourced information.

### B. Prompt/User Mitigation

Include the source order in one line when research traceability matters, but do not assume that additional wording excuses failure to execute an already explicit hierarchy.

### C. Model Improvement

Model source selection as ordered state transitions with an auditable record of why each tier was exhausted or used.

## Lessons for Users

For source-constrained research, inspect the transition after a source fails: a good answer says what was tried, why it was insufficient, and which prescribed tier came next.

## Lessons for Developers

Build a retrieval test where the official source lacks the needed detail but a designated community reference is available. The system should not jump straight to unsourced generalisation.

## Final Conclusion

The case captures a failure in the route to an answer, not necessarily in every fact stated. Skipping the requested intermediate tier made the research process less complete, while the archive does not establish what that tier would ultimately have yielded.

