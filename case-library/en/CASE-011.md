# CASE-011 — Invented multiple-choice restriction

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

2026-07-22

## Source Traceability

- **PRE ID:** PRE-013
- **TRIAGE ID:** traceable from `EVENT-0246`
- **Conversation Title:** Data anontation
- **Conversation ID:** `6a5fab6f-6cf8-83ee-8a04-960e18d40895`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0246`
- **Relevant Message IDs:** assistant `340ff6dc-dbf7-4b4b-ad00-bb841550e649`; correction `bbb21e2b-73f4-4c86-899a-88da2e697bee`; follow-up `0509f710-fb8e-4fbc-998c-3ea059fdf4f2`

## Evidence List

- **CASE-011-E01:** `bbb21ba9-1a30-42ce-9c4f-12793bdabda2`; speaker `user`; timestamp `2026-07-22T00:27:47.135599Z`; function: governing instruction/context; conversation `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E02:** `340ff6dc-dbf7-4b4b-ad00-bb841550e649`; speaker `assistant`; timestamp `2026-07-22T00:27:47.481355Z`; function: problematic response; conversation `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E03:** `bbb21e2b-73f4-4c86-899a-88da2e697bee`; speaker `user`; timestamp `2026-07-22T00:28:35.166404Z`; function: user correction; conversation `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E04:** `0509f710-fb8e-4fbc-998c-3ea059fdf4f2`; speaker `assistant`; timestamp `2026-07-22T00:28:35.801158Z`; function: assistant follow-up; conversation `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-013: governing instruction/context (`bbb21ba9-1a30-42ce-9c4f-12793bdabda2` at 2026-07-22T00:27:47.135599Z).
2. PRE-013: problematic response (`340ff6dc-dbf7-4b4b-ad00-bb841550e649` at 2026-07-22T00:27:47.481355Z).
3. PRE-013: user correction (`bbb21e2b-73f4-4c86-899a-88da2e697bee` at 2026-07-22T00:28:35.166404Z).
4. PRE-013: assistant follow-up (`0509f710-fb8e-4fbc-998c-3ea059fdf4f2` at 2026-07-22T00:28:35.801158Z).

## Issue Category

Hallucination; Instruction Following

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The preserved evaluation workflow includes an A/B/C/D guideline context and a response that introduced a multiple-choice restriction not supplied by the active rule. The correction challenges that inserted restriction. The evidence supports an unsupported-constraint finding rather than a claim that the underlying guideline had no legitimate limits.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The assistant treated a limitation as if it belonged to the active A/B/C/D rubric even though the supplied guideline did not establish it. **Requirement and deviation.** An evaluator must distinguish written criteria from assumptions that sound plausible. Adding a rule changes which answers can be considered and therefore changes the evaluation. **Inference and limit.** The archive shows a constraint-insertion error, not the source of that assumption. Its importance is procedural: invented restrictions can invalidate a judgment while appearing more rigorous.

## Recommended Improvement

### A. Response Improvement

Quote or paraphrase the governing rubric before applying a restriction, and if a needed rule is absent, ask for clarification rather than manufacture one.

### B. Prompt/User Mitigation

Provide the relevant rubric excerpt with the evaluation prompt when possible; users should not need to defend against constraints that are not in the stated guideline.

### C. Model Improvement

Develop unsupported-rule detection that compares each asserted limitation in a rationale against the active instruction set and flags unmatched claims.

## Lessons for Users

When receiving an evaluation rationale, ask which exact rubric sentence authorises each disqualifying rule. This is especially useful when the rule narrows the available answer options.

## Lessons for Developers

A counterexample fixture should present a rubric with A/B/C/D labels but omit the alleged restriction. Passing output identifies the omission; failure treats the invented condition as binding.

## Final Conclusion

The documented problem is not disagreement over an answer choice but an extra rule inserted into the judging process. The correction makes the absence of that rule central, while the archive cannot establish where the assumption originated.

