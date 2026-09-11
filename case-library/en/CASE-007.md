# CASE-007 — Template Library JSON and workflow deviation

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

2026-07-17

## Source Traceability

- **PRE ID:** PRE-007
- **TRIAGE ID:** traceable from `EVENT-0138`
- **Conversation Title:** Template Library
- **Conversation ID:** `6a57d4d3-bff4-83e8-9966-384ed9d41334`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0138`
- **Relevant Message IDs:** assistant `8fc51020-a797-49ec-8138-b68c62641100`; correction `ff7a5ca0-7cef-40d7-a3d1-2226c222b29d`; follow-up `f4759725-34b7-45c0-a38e-2d0fc0eda88d`

## Evidence List

- **CASE-007-E01:** `ab0fa726-8246-4477-8494-e45633df9209`; speaker `user`; timestamp `2026-07-17T15:14:47.421000Z`; function: governing instruction/context; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E02:** `8fc51020-a797-49ec-8138-b68c62641100`; speaker `assistant`; timestamp `2026-07-17T15:14:49.079363Z`; function: problematic response; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E03:** `ff7a5ca0-7cef-40d7-a3d1-2226c222b29d`; speaker `user`; timestamp `2026-07-17T15:15:53.854000Z`; function: user correction; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E04:** `f4759725-34b7-45c0-a38e-2d0fc0eda88d`; speaker `assistant`; timestamp `2026-07-17T15:15:55.468077Z`; function: assistant follow-up; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-007: governing instruction/context (`ab0fa726-8246-4477-8494-e45633df9209` at 2026-07-17T15:14:47.421000Z).
2. PRE-007: problematic response (`8fc51020-a797-49ec-8138-b68c62641100` at 2026-07-17T15:14:49.079363Z).
3. PRE-007: user correction (`ff7a5ca0-7cef-40d7-a3d1-2226c222b29d` at 2026-07-17T15:15:53.854000Z).
4. PRE-007: assistant follow-up (`f4759725-34b7-45c0-a38e-2d0fc0eda88d` at 2026-07-17T15:15:55.468077Z).

## Issue Category

Instruction Following; Formatting Error; Tool Usage

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The incident centres on a multipart JSON question about a Template Library workflow. The assistant treated it as an invitation to design a new architecture rather than answer the operational question presented. The evidence therefore supports an intent-classification and workflow-deviation issue, not a judgment that design discussion is always inappropriate.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The response moved from the supplied multipart JSON/task structure into a new design task. **Requirement and deviation.** The active request asked how to handle an operational configuration; the answer needed to interpret the given fields and steps before proposing redesign. **Inference and limit.** This is consistent with intent drift from implementation/question answering toward architecture generation. The archive cannot establish the internal classifier responsible. The consequence is that the user’s immediate JSON workflow remains unanswered despite receiving potentially relevant design material.

## Recommended Improvement

### A. Response Improvement

Answer the multipart JSON question field by field, state the operational action for each part, and offer an architectural redesign only as an optional next step.

### B. Prompt/User Mitigation

Lead with a direct question such as ‘How should this JSON workflow be processed?’ and ask for design alternatives separately; the existing multipart context should still remain the primary signal.

### C. Model Improvement

Train and test routing that distinguishes configuration interpretation, implementation guidance, and greenfield design requests when the same domain terms appear in all three.

## Lessons for Users

For structured-data tasks, check whether the answer addresses the supplied keys, values, and workflow transitions. A broader design proposal can be useful but should not displace the requested operational answer.

## Lessons for Developers

Create a test with a multipart JSON payload and a narrow operational question. Passing behaviour references the payload’s actual parts; failure is a generic architecture proposal with no field-level resolution.

## Final Conclusion

The response changed the kind of work being done—from operational interpretation to design. The evidence makes that diversion visible and supports a task-routing evaluation, while not ruling out design as a later, opt-in conversation.

