# CASE-010 — Fenced-code output requirement not followed

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

2026-07-21

## Source Traceability

- **PRE ID:** PRE-012
- **TRIAGE ID:** traceable from `EVENT-0224`
- **Conversation Title:** Alur analisis portofolio template manager
- **Conversation ID:** `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0224`
- **Relevant Message IDs:** assistant `463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9`; correction `bbb21769-6bce-43b7-a862-f638e55f457b`; follow-up `e13f8c82-229b-43a0-9f42-23d02bde668a`

## Evidence List

- **CASE-010-E01:** `bbb21174-a22d-4c35-a102-ebf3d049df4e`; speaker `user`; timestamp `2026-07-21T11:22:12.871670Z`; function: governing instruction/context; conversation `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E02:** `463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9`; speaker `assistant`; timestamp `2026-07-21T11:22:13.320447Z`; function: problematic response; conversation `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E03:** `bbb21769-6bce-43b7-a862-f638e55f457b`; speaker `user`; timestamp `2026-07-21T11:23:40.199457Z`; function: user correction; conversation `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E04:** `e13f8c82-229b-43a0-9f42-23d02bde668a`; speaker `assistant`; timestamp `2026-07-21T11:23:40.819257Z`; function: assistant follow-up; conversation `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-012: governing instruction/context (`bbb21174-a22d-4c35-a102-ebf3d049df4e` at 2026-07-21T11:22:12.871670Z).
2. PRE-012: problematic response (`463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9` at 2026-07-21T11:22:13.320447Z).
3. PRE-012: user correction (`bbb21769-6bce-43b7-a862-f638e55f457b` at 2026-07-21T11:23:40.199457Z).
4. PRE-012: assistant follow-up (`e13f8c82-229b-43a0-9f42-23d02bde668a` at 2026-07-21T11:23:40.819257Z).

## Issue Category

Instruction Following; Formatting Error

## Severity

**Minor** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence preserves an explicit requirement to return content in a fenced-code structure, an output that did not use that required wrapper, and a user correction. This is a format-compliance incident with a visible binary check. It does not depend on judging the underlying prose quality.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The requested instruction was delivered without the specified code fence. **Requirement and deviation.** The fence was part of the output schema, so plain text or alternate formatting was not interchangeable even if the wording was otherwise usable. **Inference and limit.** The sequence supports a formatting constraint miss; it does not show whether the assistant parsed the fence request and later discarded it. The consequence is reduced copyability or failure in a downstream workflow that expects a fenced block.

## Recommended Improvement

### A. Response Improvement

Return the requested text inside the exact fence delimiter and language label, with no surrounding material that breaks direct copying.

### B. Prompt/User Mitigation

Name the desired fence syntax when an external parser depends on it, while noting that the archived instruction already made the formatting obligation explicit.

### C. Model Improvement

Add a post-generation structural validator that checks for the required opening and closing fence before sending a response.

## Lessons for Users

When a response is meant to be copied into a tool, validate its container as well as its text. A visually minor wrapper can be a functional requirement.

## Lessons for Developers

Use a test that requests a fenced block and inspect the raw output tokens for both delimiters. Content equivalence alone should not pass the evaluation.

## Final Conclusion

This case is narrowly verifiable: the requested fenced wrapper was absent. Because the defect is structural rather than semantic, it offers a clean regression target without any need to speculate about model reasoning.

