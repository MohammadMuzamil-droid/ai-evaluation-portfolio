# CASE-020 — Student-progress format mismatch

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-020.md)

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

2026-07-29

## Source Traceability

- **PRE ID:** PRE-026
- **TRIAGE ID:** traceable from `EVENT-0471`
- **Conversation Title:** Proyek Progres Muhafadhoh
- **Conversation ID:** `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0471`
- **Relevant Message IDs:** assistant `3b615542-58c4-4903-aa0a-de2cce1692ac`; correction `bbb210d3-4788-4c88-b96e-f4f025754f41`; follow-up `ba50f229-105c-4075-8a10-18e54abba17e`

## Evidence List

- **CASE-020-E01:** `bbb21a4c-4a0a-406d-ae63-d21e54d53f71`; speaker `user`; timestamp `2026-07-29T12:21:55.473670Z`; function: governing instruction/context; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-020-E02:** `3b615542-58c4-4903-aa0a-de2cce1692ac`; speaker `assistant`; timestamp `2026-07-29T12:21:57.793977Z`; function: problematic response; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-020-E03:** `bbb210d3-4788-4c88-b96e-f4f025754f41`; speaker `user`; timestamp `2026-07-29T12:22:34.769825Z`; function: user correction; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-020-E04:** `ba50f229-105c-4075-8a10-18e54abba17e`; speaker `assistant`; timestamp `2026-07-29T12:22:37.274684Z`; function: assistant follow-up; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-026: governing instruction/context (`bbb21a4c-4a0a-406d-ae63-d21e54d53f71` at 2026-07-29T12:21:55.473670Z).
2. PRE-026: problematic response (`3b615542-58c4-4903-aa0a-de2cce1692ac` at 2026-07-29T12:21:57.793977Z).
3. PRE-026: user correction (`bbb210d3-4788-4c88-b96e-f4f025754f41` at 2026-07-29T12:22:34.769825Z).
4. PRE-026: assistant follow-up (`ba50f229-105c-4075-8a10-18e54abba17e` at 2026-07-29T12:22:37.274684Z).

## Issue Category

Instruction Following; Formatting Error

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The incident distinguishes students’ progress/perolehan records from a list of students who have not submitted. The response used a format that blurred or misplaced those state classes, and the correction identifies the separation requirement. The evidence supports a schema mismatch, not a judgment about the accuracy of every individual student value.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Progress data and non-submission status were not represented as the distinct categories required by the requested output. **Requirement and deviation.** A learner with recorded progress belongs in a progress/perolehan structure; a learner with no submission belongs in a separate exception list. Combining the two changes the meaning of the table. **Inference and limit.** The record supports a state-classification/format error, not proof that all underlying records were wrong. The consequence is misleading monitoring information: an administrator cannot reliably tell activity from absence.

## Recommended Improvement

### A. Response Improvement

Produce two explicitly labelled sections or tables: one for progress/perolehan and one for students with no submission, preserving each student’s state in the correct location.

### B. Prompt/User Mitigation

Provide headings for the two required state classes when sharing raw data; nevertheless, the archived schema requirement was operational rather than merely stylistic.

### C. Model Improvement

Validate generated progress reports against state-aware schemas so a record cannot appear simultaneously as progress and non-submission without an explicit exception rule.

## Lessons for Users

Review student reports by asking whether each row answers ‘what progress was recorded?’ or ‘who has not submitted?’. If one layout answers both ambiguously, the classification is not yet usable.

## Lessons for Developers

Use a fixture with active students and non-submitters, then require separate output classes. Visual table neatness should not pass if it erases the distinction between participation and absence.

## Final Conclusion

The documented defect is semantic formatting: the report’s structure failed to preserve two different student states. That matters for follow-up decisions, even though the evidence does not establish a numerical error in every entry.

