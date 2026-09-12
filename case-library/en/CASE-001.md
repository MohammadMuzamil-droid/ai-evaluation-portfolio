# CASE-001 — Inconsistent application of a 25-word instruction

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-001.md)

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

2026-07-07

## Source Traceability

- **PRE ID:** PRE-001
- **TRIAGE ID:** traceable from `EVENT-0007`
- **Conversation Title:** Peluang Karir di AI
- **Conversation ID:** `6a4bf6ab-5f08-83e8-afac-905a76388b09`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0007`
- **Relevant Message IDs:** assistant `1a618ee5-1be4-45b4-8e01-cde97f2ffed6`; correction `bbb21bb5-6d99-4ef4-9bb3-b06c95741f41`; follow-up `7cef39b9-7da4-4c48-b7ca-da121b016537`

## Evidence List

- **CASE-001-E01:** `bbb2162e-4d3b-4c3d-a0d8-d04421d13ab3`; speaker `user`; timestamp `2026-07-07T12:41:01.238962Z`; function: governing instruction/context; conversation `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E02:** `1a618ee5-1be4-45b4-8e01-cde97f2ffed6`; speaker `assistant`; timestamp `2026-07-07T12:41:01.527613Z`; function: problematic response; conversation `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E03:** `bbb21bb5-6d99-4ef4-9bb3-b06c95741f41`; speaker `user`; timestamp `2026-07-07T12:42:47.168915Z`; function: user correction; conversation `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E04:** `7cef39b9-7da4-4c48-b7ca-da121b016537`; speaker `assistant`; timestamp `2026-07-07T12:42:47.479027Z`; function: assistant follow-up; conversation `6a4bf6ab-5f08-83e8-afac-905a76388b09`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: exactly-25-words must be applied consistently.

## Chronology

1. PRE-001: governing instruction/context (`bbb2162e-4d3b-4c3d-a0d8-d04421d13ab3` at 2026-07-07T12:41:01.238962Z).
2. PRE-001: problematic response (`1a618ee5-1be4-45b4-8e01-cde97f2ffed6` at 2026-07-07T12:41:01.527613Z).
3. PRE-001: user correction (`bbb21bb5-6d99-4ef4-9bb3-b06c95741f41` at 2026-07-07T12:42:47.168915Z).
4. PRE-001: assistant follow-up (`7cef39b9-7da4-4c48-b7ca-da121b016537` at 2026-07-07T12:42:47.479027Z).

## Issue Category

Instruction Following; Inconsistency

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The four preserved messages record a numerical-instruction dispute: the user supplied the phrase “dalam 25 kata”, the assistant treated the exercise as a maximum-length task, the user challenged that reading, and the follow-up accepted the exactly-25 interpretation. The evidence therefore supports an inconsistency in applying the stated grading rule, not a claim about internal model state.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: exactly-25-words must be applied consistently.

## Technical Analysis

**Observation.** The response contrasts “dalam 25 kata” with “maksimal 25 kata” but then acknowledges that its earlier assessment had applied the latter rule to the former wording. **Requirement and deviation.** For the exercise as written, both candidate answers first needed the same exact-25-word check; that gate was bypassed when one answer was effectively treated under a maximum. **Inference and limit.** This is evidence of unstable rule application within the grading explanation. It does not establish why that interpretation changed internally. The consequence is material because the initial instruction-following verdict changes before any quality comparison can begin.

## Recommended Improvement

### A. Response Improvement

Re-score both answers by counting their words against exactly 25, state the failed gate for each, and only then discuss any secondary quality difference.

### B. Prompt/User Mitigation

When requesting a training exercise, ask for a displayed word count beside each candidate answer so the grading record is auditable; this makes the check visible but does not repair the original inconsistency.

### C. Model Improvement

Add a rubric-state test in which ‘exactly’, ‘maximum’, and ‘minimum’ are distinct operators and require the selected operator to be echoed in the scoring rationale.

## Lessons for Users

For fixed-count tasks, verify the count before accepting a qualitative ranking. Here the key check is not whether an answer sounds better, but whether each candidate satisfies the same exact numeric condition.

## Lessons for Developers

A regression example should feed the phrase “dalam 25 kata” plus two non-25-word candidates, then assert that neither passes instruction following and that the rationale never substitutes a maximum rule.

## Final Conclusion

This case concerns a specific scoring reversal: an exact-count instruction was initially analysed as a ceiling. The correction and follow-up make the mismatch traceable, while the archive leaves the underlying cause unknown. Its professional value is the clear ordering of evaluation gates: constraint compliance precedes comparative quality.

