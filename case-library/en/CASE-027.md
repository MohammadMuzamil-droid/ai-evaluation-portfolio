# CASE-027 — Guideline-training structure flattened

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

2026-08-11

## Source Traceability

- **PRE ID:** PRE-033
- **TRIAGE ID:** traceable from `EVENT-0947`
- **Conversation Title:** Cabang   Bab 4 Rating
- **Conversation ID:** `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`
- **Source JSON:** `conversations-001.json`
- **Event ID:** `EVENT-0947`
- **Relevant Message IDs:** assistant `0ff7c441-7bff-48a5-95bb-5fff990cf823`; correction `bbb21011-1743-4a38-b382-3476ccbdeefc`; follow-up `f8c944eb-af19-444b-badf-8cd93a9fa0d6`

## Evidence List

- **CASE-027-E01:** `bbb2147a-877b-4852-9e35-ad973e0a4539`; speaker `user`; timestamp `2026-08-11T03:54:14.849810Z`; function: governing instruction/context; conversation `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E02:** `0ff7c441-7bff-48a5-95bb-5fff990cf823`; speaker `assistant`; timestamp `2026-08-11T03:54:15.248598Z`; function: problematic response; conversation `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E03:** `bbb21011-1743-4a38-b382-3476ccbdeefc`; speaker `user`; timestamp `2026-08-11T03:57:57.477553Z`; function: user correction; conversation `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E04:** `f8c944eb-af19-444b-badf-8cd93a9fa0d6`; speaker `assistant`; timestamp `2026-08-11T03:57:57.980883Z`; function: assistant follow-up; conversation `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: Progress 1 and 2 each contain Guideline 1/2; Progress 3+ creates a guideline before each question set.

## Chronology

1. PRE-033: governing instruction/context (`bbb2147a-877b-4852-9e35-ad973e0a4539` at 2026-08-11T03:54:14.849810Z).
2. PRE-033: problematic response (`0ff7c441-7bff-48a5-95bb-5fff990cf823` at 2026-08-11T03:54:15.248598Z).
3. PRE-033: user correction (`bbb21011-1743-4a38-b382-3476ccbdeefc` at 2026-08-11T03:57:57.477553Z).
4. PRE-033: assistant follow-up (`f8c944eb-af19-444b-badf-8cd93a9fa0d6` at 2026-08-11T03:57:57.980883Z).

## Issue Category

Instruction Following; Context Handling

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence describes a hierarchical guideline-training workflow: a two-guideline pattern applies only to Progress 1 and 2, while later question cycles require a guideline before each cycle. The response flattened those stage-specific rules. The evidence supports a hierarchy/exception handling failure, not a claim that one simple workflow could never be useful elsewhere.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: Progress 1 and 2 each contain Guideline 1/2; Progress 3+ creates a guideline before each question set.

## Technical Analysis

**Observation.** The response generalised the early two-guideline pattern across later progress stages instead of applying the stated per-cycle guideline requirement. **Requirement and deviation.** The workflow had a base pattern plus a stage-dependent exception; correct execution depends on preserving both the common structure and the boundary where it changes. Flattening the hierarchy erases the later rule. **Inference and limit.** The archive shows failed exception handling in this sequence, not the reason the stage distinction was lost. The consequence is incorrect guideline timing for later learning cycles.

## Recommended Improvement

### A. Response Improvement

Apply the two-guideline setup only to Progress 1 and 2, then create or invoke a guideline before each later question cycle as specified.

### B. Prompt/User Mitigation

Present the workflow as a small stage table—Progress 1–2 versus later cycles—when handing it to an assistant, while recognising that the differentiated structure was already part of the validated requirement.

### C. Model Improvement

Test hierarchical instruction following with a general rule, an explicit stage exception, and multiple later cycles; scoring must penalise a flattened one-rule interpretation.

## Lessons for Users

For staged procedures, check the exception boundary, not just the first repeated pattern. The most important review question is often where a familiar rule stops applying.

## Lessons for Developers

A regression case should run through Progress 1, Progress 2, and two later cycles. Passing behaviour changes guideline timing after the early stages and retains that change on each later cycle.

## Final Conclusion

The failure was not a missing guideline in the abstract; it was loss of a stage-specific rule that changed the workflow after Progress 2. The evidence supports that hierarchy mismatch while leaving open how the model represented the procedure internally.

