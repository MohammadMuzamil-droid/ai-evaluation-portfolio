# CASE-023 — Mandatory summary stage skipped

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-023.md)

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

2026-08-05

## Source Traceability

- **PRE ID:** PRE-029
- **TRIAGE ID:** traceable from `EVENT-0727`
- **Conversation Title:** Cabang   Pembelajaran DOLA Web Search
- **Conversation ID:** `6a6c23dd-6324-83ec-9140-0ddb70b79925`
- **Source JSON:** `conversations-001.json`
- **Event ID:** `EVENT-0727`
- **Relevant Message IDs:** assistant `e6f36f62-a835-41a7-913e-e826fdabe6c9`; correction `bbb215e2-8479-49fa-bb19-72215ca16b77`; follow-up `a91c1336-bc62-42fa-bf37-9edfc4ae5b53`

## Evidence List

- **CASE-023-E01:** `bbb21070-3388-4202-8e95-d75be5c72700`; speaker `user`; timestamp `2026-08-05T02:31:10.990286Z`; function: governing instruction/context; conversation `6a6c23dd-6324-83ec-9140-0ddb70b79925`.
- **CASE-023-E02:** `e6f36f62-a835-41a7-913e-e826fdabe6c9`; speaker `assistant`; timestamp `2026-08-05T02:31:18.025584Z`; function: problematic response; conversation `6a6c23dd-6324-83ec-9140-0ddb70b79925`.
- **CASE-023-E03:** `bbb215e2-8479-49fa-bb19-72215ca16b77`; speaker `user`; timestamp `2026-08-05T02:31:47.967398Z`; function: user correction; conversation `6a6c23dd-6324-83ec-9140-0ddb70b79925`.
- **CASE-023-E04:** `a91c1336-bc62-42fa-bf37-9edfc4ae5b53`; speaker `assistant`; timestamp `2026-08-05T02:31:48.269454Z`; function: assistant follow-up; conversation `6a6c23dd-6324-83ec-9140-0ddb70b79925`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-029: governing instruction/context (`bbb21070-3388-4202-8e95-d75be5c72700` at 2026-08-05T02:31:10.990286Z).
2. PRE-029: problematic response (`e6f36f62-a835-41a7-913e-e826fdabe6c9` at 2026-08-05T02:31:18.025584Z).
3. PRE-029: user correction (`bbb215e2-8479-49fa-bb19-72215ca16b77` at 2026-08-05T02:31:47.967398Z).
4. PRE-029: assistant follow-up (`a91c1336-bc62-42fa-bf37-9edfc4ae5b53` at 2026-08-05T02:31:48.269454Z).

## Issue Category

Instruction Following; Missing Requirement

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The preserved learning workflow includes a mandatory pedagogical summary stage before transition to the next module. The response advanced without completing that stage, and the correction points to the checklist requirement. The evidence supports a progression-gate failure, not a claim that the subsequent module content was inherently incorrect.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The assistant moved to the next topic while the required summary had not been delivered. **Requirement and deviation.** The summary was an explicit completion condition, intended to consolidate the prior material before progression. Skipping it changes the learning sequence from guided closure to abrupt transition. **Inference and limit.** The exchange shows a missed stage gate, not proof that the learner failed to understand the preceding topic. The consequence is a less auditable and potentially less coherent instructional path.

## Recommended Improvement

### A. Response Improvement

Provide the required summary, confirm that its key points are covered, and only then introduce the next module or offer a transition.

### B. Prompt/User Mitigation

Keep a visible stage checklist for multi-module learning and ask the assistant to mark the summary complete before progressing; the workflow’s existing gate should still be respected without repeated prompting.

### C. Model Improvement

Represent mandatory instructional stages as completion prerequisites and test that a topic transition is blocked when the summary artefact is absent.

## Lessons for Users

In sequential learning, look for the closure artefact before accepting a topic change. A new lesson may be relevant, but it should not silently replace the recap that makes the previous lesson reviewable.

## Lessons for Developers

Build a curriculum test with a required summary between two modules. The output should fail if it jumps directly to the second module, even when the new material is well written.

## Final Conclusion

This is a workflow-order defect: the assistant advanced past a named teaching checkpoint. The record does not measure learning outcomes, but it clearly shows that the prescribed summary stage was not completed first.

