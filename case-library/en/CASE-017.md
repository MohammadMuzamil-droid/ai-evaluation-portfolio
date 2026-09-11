# CASE-017 — Rewrite request diverted into an audit

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

2026-07-28

## Source Traceability

- **PRE ID:** PRE-023
- **TRIAGE ID:** traceable from `EVENT-0430`
- **Conversation Title:** Perkembangan siswa prompt editor
- **Conversation ID:** `6a684b13-532c-83ec-aeee-47e456ac72ce`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0430`
- **Relevant Message IDs:** assistant `ce535159-b12c-4a0b-9676-c0a830131cf3`; correction `bbb218e6-fb1a-423e-8ea9-8ee3005d26f6`; follow-up `f17c87ba-171e-46e3-b3f1-22fbfc992281`

## Evidence List

- **CASE-017-E01:** `bbb2146d-37ef-49fa-93cd-1b6a3e178cba`; speaker `user`; timestamp `2026-07-28T18:27:48.543230Z`; function: governing instruction/context; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-017-E02:** `ce535159-b12c-4a0b-9676-c0a830131cf3`; speaker `assistant`; timestamp `2026-07-28T18:27:48.794735Z`; function: problematic response; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-017-E03:** `bbb218e6-fb1a-423e-8ea9-8ee3005d26f6`; speaker `user`; timestamp `2026-07-28T18:37:12.575928Z`; function: user correction; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-017-E04:** `f17c87ba-171e-46e3-b3f1-22fbfc992281`; speaker `assistant`; timestamp `2026-07-28T18:37:12.830040Z`; function: assistant follow-up; conversation `6a684b13-532c-83ec-aeee-47e456ac72ce`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-023: governing instruction/context (`bbb2146d-37ef-49fa-93cd-1b6a3e178cba` at 2026-07-28T18:27:48.543230Z).
2. PRE-023: problematic response (`ce535159-b12c-4a0b-9676-c0a830131cf3` at 2026-07-28T18:27:48.794735Z).
3. PRE-023: user correction (`bbb218e6-fb1a-423e-8ea9-8ee3005d26f6` at 2026-07-28T18:37:12.575928Z).
4. PRE-023: assistant follow-up (`f17c87ba-171e-46e3-b3f1-22fbfc992281` at 2026-07-28T18:37:12.830040Z).

## Issue Category

Instruction Following; Context Handling

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence preserves a request to rewrite material and a response that shifted into audit, critique, or theory discussion instead of returning the requested rewrite. The correction clarifies that the prior stage had ended and an edited deliverable was wanted. This supports a task-transition failure, not a judgment that audit work is never useful.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** The assistant retained an analytical mode after the user asked for a rewrite, producing review-oriented content rather than transformed text. **Requirement and deviation.** A rewrite request changes the active task from diagnosis to delivery; further audit may be optional but cannot replace the revised version. **Inference and limit.** The exchange indicates stale task-state carryover. It does not prove whether the system deliberately prioritised analysis or merely misread the imperative. The consequence is a stalled workflow: the user must restate a request that was already direct.

## Recommended Improvement

### A. Response Improvement

Return the rewritten text in the requested scope and style, then offer an audit separately if it would help; do not interpose analysis before the deliverable.

### B. Prompt/User Mitigation

Use wording such as ‘rewrite the text below; do not analyse it first’ when a clean handoff matters, while recognising that the archived rewrite request itself identified the main task.

### C. Model Improvement

Test multi-stage conversations in which a critique stage is followed by REWRITE. The evaluator should require a transformed artefact and flag continued analysis as a mode-transition error.

## Lessons for Users

After a diagnostic discussion, inspect the first line of the next response: it should begin doing the newly requested task, not continue explaining the previous one.

## Lessons for Developers

A regression fixture should include an audit exchange followed by a concise rewrite command. Passing output is revised prose; failure is another checklist, rationale, or theoretical discussion.

## Final Conclusion

The evidence shows a handoff failure between analysis and revision. That distinction matters because useful critique still fails the request when it displaces the rewrite the user asked to receive.

