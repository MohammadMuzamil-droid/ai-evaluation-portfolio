# CASE-002 — Contradictory CV advice about supportable claims

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-002.md)

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

2026-07-09

## Source Traceability

- **PRE ID:** PRE-002
- **TRIAGE ID:** traceable from `EVENT-0033`
- **Conversation Title:** Buat gambar
- **Conversation ID:** `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0033`
- **Relevant Message IDs:** assistant `523a35b7-1741-48db-8e66-db15a1324899`; correction `bbb21b3e-8f22-406a-b3ea-8be79021b22e`; follow-up `8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6`

## Evidence List

- **CASE-002-E01:** `bbb21e5d-dd3b-45ec-8134-14f84b08e903`; speaker `user`; timestamp `2026-07-09T21:46:10.199103Z`; function: governing instruction/context; conversation `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E02:** `523a35b7-1741-48db-8e66-db15a1324899`; speaker `assistant`; timestamp `2026-07-09T21:46:10.546755Z`; function: problematic response; conversation `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E03:** `bbb21b3e-8f22-406a-b3ea-8be79021b22e`; speaker `user`; timestamp `2026-07-09T21:47:56.998648Z`; function: user correction; conversation `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E04:** `8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6`; speaker `assistant`; timestamp `2026-07-09T21:47:57.368687Z`; function: assistant follow-up; conversation `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: the advice presents a potential risk of an unsupported/inappropriate platform claim; no actual policy violation is asserted.

## Chronology

1. PRE-002: governing instruction/context (`bbb21e5d-dd3b-45ec-8134-14f84b08e903` at 2026-07-09T21:46:10.199103Z).
2. PRE-002: problematic response (`523a35b7-1741-48db-8e66-db15a1324899` at 2026-07-09T21:46:10.546755Z).
3. PRE-002: user correction (`bbb21b3e-8f22-406a-b3ea-8be79021b22e` at 2026-07-09T21:47:56.998648Z).
4. PRE-002: assistant follow-up (`8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6` at 2026-07-09T21:47:57.368687Z).

## Issue Category

Contradiction; Inconsistency; Wrong Assumption

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The preserved CV-advice sequence juxtaposes recommendations about claims that should be supportable with wording that could encourage an unsupported platform or experience claim. The user’s validation judgment frames this as a potential risk rather than a proven policy breach. The evidence supports testing consistency of advice, not alleging an actual external violation.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: the advice presents a potential risk of an unsupported/inappropriate platform claim; no actual policy violation is asserted.

## Technical Analysis

**Observation.** The advice differentiates evidence-backed qualifications from claims that need support, yet another portion proposes language whose support is not established in the supplied context. **Requirement and deviation.** A CV recommendation must either use demonstrated experience or label a proposed skill as a learning goal; it cannot apply a stricter evidence standard selectively. **Inference and limit.** The exchange indicates contradictory recommendation logic, not proof that the user would submit a false CV or breach a platform policy. The practical harm is that a learner may copy a polished phrase that the surrounding advice itself says should be substantiated.

## Recommended Improvement

### A. Response Improvement

Rewrite the CV guidance into two labelled buckets—verified experience and future-development goals—and remove or qualify any sentence whose supporting evidence is absent.

### B. Prompt/User Mitigation

Supply a short list of completed projects, tools used, and demonstrable outcomes before requesting CV wording; when that material is already given, the assistant should not silently lower its evidentiary standard.

### C. Model Improvement

Evaluate career-writing responses for consistency between their cautionary rules and their suggested claims, including a contradiction check for unverifiable product, credential, or platform references.

## Lessons for Users

Treat a CV suggestion as a claim inventory: ask what concrete work, artefact, or result would let the candidate defend each line. Aspirational capability belongs in a development plan, not automatically in experience wording.

## Lessons for Developers

Use a paired test where the assistant warns against unsupported claims and later receives an invitation to draft one. The expected behaviour is to preserve the warning and offer a clearly future-oriented alternative.

## Final Conclusion

The evidence shows advice that is cautious in principle but potentially permissive in application. Because the user judgment does not allege a completed policy violation, the case is strongest as a consistency and claim-supportability problem rather than a compliance accusation.

