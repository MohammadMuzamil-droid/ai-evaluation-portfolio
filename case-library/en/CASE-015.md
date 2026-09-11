# CASE-015 — Evaluation omitted complete answer text

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

2026-07-27

## Source Traceability

- **PRE ID:** PRE-021
- **TRIAGE ID:** traceable from `EVENT-0373`
- **Conversation Title:** Sertifikasi OneForma LLM
- **Conversation ID:** `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0373`
- **Relevant Message IDs:** assistant `37192b10-28ec-4b5d-b04c-6c6dab4ac3c8`; correction `bbb217c9-23b4-40d0-8ad2-2d7480fd9edb`; follow-up `ca81f180-6671-4c78-b729-959495f0b444`

## Evidence List

- **CASE-015-E01:** `bbb21a3e-6b5c-4218-82cb-6786cdf814a1`; speaker `user`; timestamp `2026-07-27T12:37:02.935905Z`; function: governing instruction/context; conversation `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E02:** `37192b10-28ec-4b5d-b04c-6c6dab4ac3c8`; speaker `assistant`; timestamp `2026-07-27T12:37:03.202118Z`; function: problematic response; conversation `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E03:** `bbb217c9-23b4-40d0-8ad2-2d7480fd9edb`; speaker `user`; timestamp `2026-07-27T12:37:41.375942Z`; function: user correction; conversation `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E04:** `ca81f180-6671-4c78-b729-959495f0b444`; speaker `assistant`; timestamp `2026-07-27T12:37:41.588036Z`; function: assistant follow-up; conversation `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-021: governing instruction/context (`bbb21a3e-6b5c-4218-82cb-6786cdf814a1` at 2026-07-27T12:37:02.935905Z).
2. PRE-021: problematic response (`37192b10-28ec-4b5d-b04c-6c6dab4ac3c8` at 2026-07-27T12:37:03.202118Z).
3. PRE-021: user correction (`bbb217c9-23b4-40d0-8ad2-2d7480fd9edb` at 2026-07-27T12:37:41.375942Z).
4. PRE-021: assistant follow-up (`ca81f180-6671-4c78-b729-959495f0b444` at 2026-07-27T12:37:41.588036Z).

## Issue Category

Instruction Following; Formatting Error

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence records an evaluation or research workflow whose later analysis required the complete answer text, while the produced record retained labels or summaries without the full answer content. The correction identifies the missing field as material. This supports a schema-completeness issue, not a claim that the retained labels were themselves inaccurate.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The record omitted the complete answer text that downstream evaluation needed. **Requirement and deviation.** In an analysis schema, answer labels, scores, or summaries cannot substitute for the text required to inspect reasoning, wording, and evidence. The omission made later review structurally impossible or weaker. **Inference and limit.** The archive demonstrates missing required payload, not a conclusion about why the field was dropped. The consequence is loss of auditability: a reviewer cannot independently reconstruct the evaluated response from a label alone.

## Recommended Improvement

### A. Response Improvement

Store the full answer verbatim alongside labels, scores, and notes, then validate that every required record field is present before closing the evaluation step.

### B. Prompt/User Mitigation

When commissioning an evaluation table, name the downstream fields needed for later review; where that need was already stated, the absence remains a delivery defect rather than a prompt omission.

### C. Model Improvement

Add schema validation that rejects incomplete evaluation records and preserves a content hash or exact text field for each response under review.

## Lessons for Users

For evaluation datasets, confirm that a future reader could see the exact answer being judged. A verdict without its underlying text cannot support detailed quality review.

## Lessons for Developers

Regression coverage should send an answer, require labels plus verbatim content, and fail when the system keeps only a score or abbreviated description. This tests preservation, not merely classification accuracy.

## Final Conclusion

The case is about an incomplete record, not merely a less detailed summary. Because the full answer was required for subsequent analysis, its absence undermined traceability even if the remaining labels were useful.

