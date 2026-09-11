# CASE-021 — EXTRACT produced summary PDF

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

2026-07-31

## Source Traceability

- **PRE ID:** PRE-027
- **TRIAGE ID:** traceable from `EVENT-0510`
- **Conversation Title:** Pembelajaran DOLA Web Search
- **Conversation ID:** `6a6b508e-8c68-83ec-bc9e-207be38c8039`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0510`
- **Relevant Message IDs:** assistant `b0448e02-aa19-4645-b819-b477b1ce06f5`; correction `bbb21e81-8b18-41e7-8952-c0f072400691`; follow-up `4fa6fa74-46a4-4724-a79f-5d2398cd0c42`

## Evidence List

- **CASE-021-E01:** `bbb21f84-c99e-44d2-b798-18fdff8263c9`; speaker `user`; timestamp `2026-07-31T04:19:57.654775Z`; function: governing instruction/context; conversation `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E02:** `b0448e02-aa19-4645-b819-b477b1ce06f5`; speaker `assistant`; timestamp `2026-07-31T04:20:07.865488Z`; function: problematic response; conversation `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E03:** `bbb21e81-8b18-41e7-8952-c0f072400691`; speaker `user`; timestamp `2026-07-31T04:21:09.065567Z`; function: user correction; conversation `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E04:** `4fa6fa74-46a4-4724-a79f-5d2398cd0c42`; speaker `assistant`; timestamp `2026-07-31T04:21:23.473186Z`; function: assistant follow-up; conversation `6a6b508e-8c68-83ec-bc9e-207be38c8039`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-027: governing instruction/context (`bbb21f84-c99e-44d2-b798-18fdff8263c9` at 2026-07-31T04:19:57.654775Z).
2. PRE-027: problematic response (`b0448e02-aa19-4645-b819-b477b1ce06f5` at 2026-07-31T04:20:07.865488Z).
3. PRE-027: user correction (`bbb21e81-8b18-41e7-8952-c0f072400691` at 2026-07-31T04:21:09.065567Z).
4. PRE-027: assistant follow-up (`4fa6fa74-46a4-4724-a79f-5d2398cd0c42` at 2026-07-31T04:21:23.473186Z).

## Issue Category

Instruction Following; Formatting Error; Tool Usage

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The preserved EXTRACT command required retention of the latest output, while the assistant produced a summary PDF that omitted or transformed material instead of preserving it. The correction focuses on EXTRACT semantics. The evidence supports a lossiness finding without claiming that summarisation is never useful when explicitly requested.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Invoking EXTRACT produced a summarised PDF rather than a faithful preservation of the latest output. **Requirement and deviation.** In this workflow, EXTRACT meant carry the source material forward; summarisation changes selection, wording, and potentially omissions. A polished PDF is not equivalent to an extract when preservation is the command contract. **Inference and limit.** The record demonstrates a semantic substitution from preservation to condensation. It does not quantify every lost passage unless compared line by line. The consequence is that the exported artefact cannot serve as the requested source-faithful record.

## Recommended Improvement

### A. Response Improvement

Create an extract that reproduces the latest output without summarising it, and label any separate synopsis as a distinct optional artefact.

### B. Prompt/User Mitigation

Specify ‘verbatim/latest-output extract’ when a downstream user needs exact preservation, while the established EXTRACT command should already be honoured once defined.

### C. Model Improvement

Add source-to-export comparison for preservation commands, failing delivery when content is condensed, reordered, or omitted without an explicit transformation request.

## Lessons for Users

For preservation commands, compare the source and the result rather than judging only whether the result looks polished. A summary can be useful and still be the wrong artefact.

## Lessons for Developers

A regression test should call EXTRACT on a multi-part response and compare the generated file to that response for omissions. A summary PDF must be classified as a different operation.

## Final Conclusion

This case turns on command semantics: EXTRACT required fidelity, but the response delivered condensation. The evidence supports the preservation mismatch, while a detailed inventory of every omitted line would require a separate source–file diff.

