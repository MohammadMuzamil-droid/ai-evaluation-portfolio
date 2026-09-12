# CASE-004 — REVISE returned a change log instead of a revised draft

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-004.md)

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

2026-07-17

## Source Traceability

- **PRE ID:** PRE-004
- **TRIAGE ID:** traceable from `EVENT-0114`
- **Conversation Title:** Template Library
- **Conversation ID:** `6a57d4d3-bff4-83e8-9966-384ed9d41334`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0114`
- **Relevant Message IDs:** assistant `0f152a19-8805-4dfa-8423-9682f5b5e537`; correction `bbb219b8-a1b8-4829-8bf8-4af32aac8f93`; follow-up `f469d3f5-2141-411e-9d9d-24aac56b3a77`

## Evidence List

- **CASE-004-E01:** `bbb21b26-d6d8-4209-9388-d5d7e354590f`; speaker `user`; timestamp `2026-07-17T03:06:48.299575Z`; function: governing instruction/context; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E02:** `0f152a19-8805-4dfa-8423-9682f5b5e537`; speaker `assistant`; timestamp `2026-07-17T03:06:48.680813Z`; function: problematic response; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E03:** `bbb219b8-a1b8-4829-8bf8-4af32aac8f93`; speaker `user`; timestamp `2026-07-17T03:07:43.795771Z`; function: user correction; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E04:** `f469d3f5-2141-411e-9d9d-24aac56b3a77`; speaker `assistant`; timestamp `2026-07-17T03:07:44.175886Z`; function: assistant follow-up; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-004: governing instruction/context (`bbb21b26-d6d8-4209-9388-d5d7e354590f` at 2026-07-17T03:06:48.299575Z).
2. PRE-004: problematic response (`0f152a19-8805-4dfa-8423-9682f5b5e537` at 2026-07-17T03:06:48.680813Z).
3. PRE-004: user correction (`bbb219b8-a1b8-4829-8bf8-4af32aac8f93` at 2026-07-17T03:07:43.795771Z).
4. PRE-004: assistant follow-up (`f469d3f5-2141-411e-9d9d-24aac56b3a77` at 2026-07-17T03:07:44.175886Z).

## Issue Category

Instruction Following; Formatting Error

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The incident messages preserve a command labelled REVISE, an assistant response consisting of a change log or discussion, and the user’s correction that the revised draft itself was needed. The follow-up confirms the distinction. The evidence identifies a command-to-deliverable substitution rather than a disagreement about style.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Instead of emitting the revised text requested by REVISE, the assistant described or enumerated changes. **Requirement and deviation.** A change log can accompany a revision, but it cannot replace the primary artefact when the command calls for a rewritten draft. **Inference and limit.** The sequence demonstrates an output-type mismatch; it does not tell us whether the omitted draft had been generated internally. This matters because the user could not review, copy, or apply the requested revision from the delivered material.

## Recommended Improvement

### A. Response Improvement

Produce the complete revised draft first, preserving the requested format; append a concise change log only after the draft if it adds value.

### B. Prompt/User Mitigation

State ‘return the full replacement text’ when a draft must be directly usable, while recognising that the original REVISE command was already sufficiently specific.

### C. Model Improvement

Add intent-to-artifact checks so REVISE maps to transformed content and not solely to commentary about transformation.

## Lessons for Users

For editing commands, inspect whether the response contains a replacement artefact that can be pasted into the work. An explanation of edits is not operationally equivalent to the edited text.

## Lessons for Developers

Test REVISE with a source paragraph and require an output containing the full revised paragraph. A response containing only bullets about changes should fail even if the bullets are sensible.

## Final Conclusion

The preserved exchange isolates a straightforward deliverable failure: a change description was supplied where a revised draft was required. Its significance is practical—without the draft, the requested editing task remains unfinished.

