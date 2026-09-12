# CASE-024 — Evaluator and annotator roles conflated

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-024.md)

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

2026-08-06

## Source Traceability

- **PRE ID:** PRE-030
- **TRIAGE ID:** traceable from `EVENT-0782`
- **Conversation Title:** Cabang   Cabang   Pembelajaran DOLA Web Search
- **Conversation ID:** `6a72a288-7c74-83ec-aeaf-f4dd70afdf90`
- **Source JSON:** `conversations-001.json`
- **Event ID:** `EVENT-0782`
- **Relevant Message IDs:** assistant `76d0ccc3-1c80-4ed4-b61e-a05ba4ff083e`; correction `bbb21b23-8101-4522-983b-ad3927447336`; follow-up `9302d964-ab51-4f35-91d2-187b8e1e79e4`

## Evidence List

- **CASE-024-E01:** `bbb211dd-a0f2-4fb5-9d91-3cbe3b4bbf80`; speaker `user`; timestamp `2026-08-06T10:44:25.903148Z`; function: governing instruction/context; conversation `6a72a288-7c74-83ec-aeaf-f4dd70afdf90`.
- **CASE-024-E02:** `76d0ccc3-1c80-4ed4-b61e-a05ba4ff083e`; speaker `assistant`; timestamp `2026-08-06T10:44:26.393798Z`; function: problematic response; conversation `6a72a288-7c74-83ec-aeaf-f4dd70afdf90`.
- **CASE-024-E03:** `bbb21b23-8101-4522-983b-ad3927447336`; speaker `user`; timestamp `2026-08-06T10:46:29.611173Z`; function: user correction; conversation `6a72a288-7c74-83ec-aeaf-f4dd70afdf90`.
- **CASE-024-E04:** `9302d964-ab51-4f35-91d2-187b8e1e79e4`; speaker `assistant`; timestamp `2026-08-06T10:46:30.170951Z`; function: assistant follow-up; conversation `6a72a288-7c74-83ec-aeaf-f4dd70afdf90`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-030: governing instruction/context (`bbb211dd-a0f2-4fb5-9d91-3cbe3b4bbf80` at 2026-08-06T10:44:25.903148Z).
2. PRE-030: problematic response (`76d0ccc3-1c80-4ed4-b61e-a05ba4ff083e` at 2026-08-06T10:44:26.393798Z).
3. PRE-030: user correction (`bbb21b23-8101-4522-983b-ad3927447336` at 2026-08-06T10:46:29.611173Z).
4. PRE-030: assistant follow-up (`9302d964-ab51-4f35-91d2-187b8e1e79e4` at 2026-08-06T10:46:30.170951Z).

## Issue Category

Reasoning Error; Inconsistency

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence records a training example in which an evaluator confused categories and the response attributed the classification error to the annotated actor rather than the evaluator. The correction preserves the role distinction. This supports an attribution failure, not a claim that the annotated actor’s underlying behaviour was flawless.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The explanation assigned responsibility for a category mistake to the person or item being annotated, even though the error arose in the evaluator’s categorisation. **Requirement and deviation.** Evaluator and annotated actor are different roles: one produces or exhibits behaviour, the other applies a label. Confusing them changes both diagnosis and remediation. **Inference and limit.** The record establishes misattribution in the training account; it does not prove intent or competence beyond this example. The consequence is misplaced feedback and an evaluator lesson that trains the wrong corrective action.

## Recommended Improvement

### A. Response Improvement

State that the evaluator made the category distinction error, then separately describe the annotated behaviour only if the evidence requires it.

### B. Prompt/User Mitigation

Name the actor and evaluator roles explicitly in examples with multiple participants; the supplied terminology already provided the essential distinction.

### C. Model Improvement

Add role-aware evaluation tests in which identical labels can be wrongly assigned to an annotator, evaluator, or source actor, and require the rationale to identify the correct decision-maker.

## Lessons for Users

When reading a classification explanation, ask ‘who chose the label?’ before deciding who made the mistake. This prevents feedback from being directed at the object of evaluation instead of the evaluator.

## Lessons for Developers

Use counterfactual training examples where the annotated behaviour stays fixed but the evaluator changes the label incorrectly. A passing diagnosis assigns the error to the labeling role.

## Final Conclusion

The case is about responsibility placement in an evaluation workflow. By conflating evaluator with annotated actor, the response obscured the true location of the classification error and weakened the value of the training feedback.

