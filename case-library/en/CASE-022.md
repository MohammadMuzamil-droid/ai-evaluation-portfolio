# CASE-022 — Exercise artifacts not retained for later evaluation

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-022.md)

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

2026-07-31

## Source Traceability

- **PRE ID:** PRE-028
- **TRIAGE ID:** traceable from `EVENT-0551`
- **Conversation Title:** Cabang   Cabang   Pembelajaran DOLA Web Search
- **Conversation ID:** `6a6c2431-527c-83ec-8b9a-fa87bf101a92`
- **Source JSON:** `conversations-001.json`
- **Event ID:** `EVENT-0551`
- **Relevant Message IDs:** assistant `5ec6aedd-a2a7-4b8e-8671-9895fb95b4f7`; correction `bbb21440-1f67-4cab-adcf-0838fe664c8a`; follow-up `a8f5bd98-b7df-4bc6-abe5-9b510f6e09e3`

## Evidence List

- **CASE-022-E01:** `bbb21e6a-b48d-4904-ada6-9e0e99b5f217`; speaker `user`; timestamp `2026-07-31T05:23:40.626305Z`; function: governing instruction/context; conversation `6a6c2431-527c-83ec-8b9a-fa87bf101a92`.
- **CASE-022-E02:** `5ec6aedd-a2a7-4b8e-8671-9895fb95b4f7`; speaker `assistant`; timestamp `2026-07-31T05:23:40.882747Z`; function: problematic response; conversation `6a6c2431-527c-83ec-8b9a-fa87bf101a92`.
- **CASE-022-E03:** `bbb21440-1f67-4cab-adcf-0838fe664c8a`; speaker `user`; timestamp `2026-07-31T05:26:16.164953Z`; function: user correction; conversation `6a6c2431-527c-83ec-8b9a-fa87bf101a92`.
- **CASE-022-E04:** `a8f5bd98-b7df-4bc6-abe5-9b510f6e09e3`; speaker `assistant`; timestamp `2026-07-31T05:26:16.443131Z`; function: assistant follow-up; conversation `6a6c2431-527c-83ec-8b9a-fa87bf101a92`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-028: governing instruction/context (`bbb21e6a-b48d-4904-ada6-9e0e99b5f217` at 2026-07-31T05:23:40.626305Z).
2. PRE-028: problematic response (`5ec6aedd-a2a7-4b8e-8671-9895fb95b4f7` at 2026-07-31T05:23:40.882747Z).
3. PRE-028: user correction (`bbb21440-1f67-4cab-adcf-0838fe664c8a` at 2026-07-31T05:26:16.164953Z).
4. PRE-028: assistant follow-up (`a8f5bd98-b7df-4bc6-abe5-9b510f6e09e3` at 2026-07-31T05:26:16.443131Z).

## Issue Category

Context Handling; Missing Requirement

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence concerns a high-priority exercise workflow where questions, options, answers, and evaluation context needed to remain available for later detailed review. The response did not retain those artefacts sufficiently. This supports a downstream-state preservation issue, not an assertion that the exercise itself lacked educational value.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Essential exercise artefacts were not carried forward in a form that allowed later evaluation to inspect the question, candidate options, answer, and context together. **Requirement and deviation.** These fields are interdependent: an answer cannot be evaluated fairly without the question and options that defined its choice space. Losing them breaks the later review chain. **Inference and limit.** The archive shows prioritisation failure in retained state, not the exact context-window or storage cause. The consequence is that subsequent feedback must rely on memory or reconstruction rather than the original exercise evidence.

## Recommended Improvement

### A. Response Improvement

Preserve a structured exercise record containing prompt, options, selected answer, expected answer if available, and evaluation notes before moving to later tasks.

### B. Prompt/User Mitigation

Ask for a saved exercise record or a recap checkpoint when planning later evaluation, but do not treat repeated user upload as the default remedy for artefacts already marked high priority.

### C. Model Improvement

Protect downstream-evaluation fields in context budgeting and test transitions from quiz delivery to detailed review with the full exercise record still available.

## Lessons for Users

If a quiz will be reviewed later, keep the question and options with the answer. Saving only the final choice removes the context needed to understand whether the choice was defensible.

## Lessons for Developers

A state-retention fixture should deliver an exercise, switch topics, and later request detailed feedback. Passing output retrieves all defining artefacts rather than inventing or asking the user to reconstruct them.

## Final Conclusion

The failure is loss of evaluative context, not simply loss of text. Because later review depended on the exercise’s full structure, insufficient retention weakened the evidence available for feedback.

