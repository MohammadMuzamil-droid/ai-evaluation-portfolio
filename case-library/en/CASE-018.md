# CASE-018 — Prompt-length assumption reversed requested direction

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

2026-07-29

## Source Traceability

- **PRE ID:** PRE-024
- **TRIAGE ID:** traceable from `EVENT-0432`
- **Conversation Title:** Perkembangan siswa prompt editor
- **Conversation ID:** `6a684b13-532c-83ec-aeee-47e456ac72ce`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0432`
- **Relevant Message IDs:** assistant `ce1a7ae1-4f00-4d55-96cd-1550a8271fa8`; correction `bbb2173a-3657-4d74-84d0-b5845cc4d269`; follow-up `8f75e155-1fe2-4376-974d-efc66d1d1f1a`

## Evidence List

- **CASE-018-E01:** `bbb21cd1-ebe0-4274-aa66-a1733f6f80c1`; speaker `user`; timestamp `2026-07-29T02:04:44.118437Z`; function: governing instruction/context; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E02:** `ce1a7ae1-4f00-4d55-96cd-1550a8271fa8`; speaker `assistant`; timestamp `2026-07-29T02:04:44.517557Z`; function: problematic response; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E03:** `bbb2173a-3657-4d74-84d0-b5845cc4d269`; speaker `user`; timestamp `2026-07-29T02:05:39.316235Z`; function: user correction; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E04:** `8f75e155-1fe2-4376-974d-efc66d1d1f1a`; speaker `assistant`; timestamp `2026-07-29T02:05:39.606745Z`; function: assistant follow-up; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-024: governing instruction/context (`bbb21cd1-ebe0-4274-aa66-a1733f6f80c1` at 2026-07-29T02:04:44.118437Z).
2. PRE-024: problematic response (`ce1a7ae1-4f00-4d55-96cd-1550a8271fa8` at 2026-07-29T02:04:44.517557Z).
3. PRE-024: user correction (`bbb2173a-3657-4d74-84d0-b5845cc4d269` at 2026-07-29T02:05:39.316235Z).
4. PRE-024: assistant follow-up (`8f75e155-1fe2-4376-974d-efc66d1d1f1a` at 2026-07-29T02:05:39.606745Z).

## Issue Category

Instruction Following; Formatting Error

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The archive contains the full Project Instructions before and after the rewrite, plus the feasibility assertion, user correction, and renewed rewrite request. Direct measurement verified 6,566 to 5,482 characters including whitespace (−1,084; 16.51% reduction), and 5,558 to 4,601 excluding whitespace (−957; 17.22%). The evidence supports a reversed length assumption; it does not support the earlier approximately-40% claim.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Before producing the rewrite, the assistant said restructuring would make the instructions longer even though the user wanted them more concise. The later raw pair demonstrates the opposite direction: the complete rewritten instructions are 1,084 characters shorter including whitespace. **Requirement and deviation.** The task required a full rewrite under a character-budget preference, so length should have been measured after drafting rather than assumed from the idea of restructuring. **Inference and limit.** This is a demonstrable feasibility-assumption error, not proof that every rewrite will shrink. The exact chronology and counts resolve the prior validation conflict without explaining the original prediction.

## Recommended Improvement

### A. Response Improvement

Draft the entire revised Project Instructions, measure characters including whitespace, and present the measured comparison rather than predicting expansion; retain the complete text as the primary deliverable.

### B. Prompt/User Mitigation

State the desired direction—shorter while retaining required rules—and request a before/after character count. In this incident, the verified reduction shows the user’s preference was achievable without a prompt change.

### C. Model Improvement

Use character-budget regression tests with this raw pair: 6,566 before and 5,482 after including whitespace, rejecting a feasibility assertion that has not been checked against a drafted full output.

## Lessons for Users

For length-sensitive rewrites, ask for a full before/after measurement instead of accepting an estimate. In this case, the verified 16.51% reduction is the relevant result, not an unmeasured intuition about restructuring.

## Lessons for Developers

Maintain a regression fixture containing the two exact instruction messages and calculate both whitespace-inclusive and whitespace-excluded counts. The test should distinguish an estimate from a completed measured rewrite.

## Final Conclusion

CASE-018 remains quantitatively verified: the final rewrite reduced the full instructions from 6,566 to 5,482 characters including whitespace. The case demonstrates why length feasibility must be measured on the finished artefact; it makes no claim about a universal compression rate.

