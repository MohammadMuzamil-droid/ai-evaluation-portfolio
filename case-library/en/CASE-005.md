# CASE-005 — Curriculum content added outside workflow scope

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-005.md)

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

2026-07-17

## Source Traceability

- **PRE ID:** PRE-005
- **TRIAGE ID:** traceable from `EVENT-0125`
- **Conversation Title:** Kursus Inggris
- **Conversation ID:** `6a570be4-831c-83ee-ab90-8bcff996410e`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0125`
- **Relevant Message IDs:** assistant `0894563f-1b7e-45ed-82c7-46824baf8730`; correction `bbb21973-61d5-4a07-9f59-3e00f21aeef7`; follow-up `368e0570-ceb6-4f05-8738-c31e67b9190b`

## Evidence List

- **CASE-005-E01:** `bbb21176-5de0-44fe-b727-388388599887`; speaker `user`; timestamp `2026-07-17T11:21:36.486327Z`; function: governing instruction/context; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E02:** `0894563f-1b7e-45ed-82c7-46824baf8730`; speaker `assistant`; timestamp `2026-07-17T11:21:36.823546Z`; function: problematic response; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E03:** `bbb21973-61d5-4a07-9f59-3e00f21aeef7`; speaker `user`; timestamp `2026-07-17T11:23:34.030653Z`; function: user correction; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E04:** `368e0570-ceb6-4f05-8738-c31e67b9190b`; speaker `assistant`; timestamp `2026-07-17T11:23:34.427258Z`; function: assistant follow-up; conversation `6a570be4-831c-83ee-ab90-8bcff996410e`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Chronology

1. PRE-005: governing instruction/context (`bbb21176-5de0-44fe-b727-388388599887` at 2026-07-17T11:21:36.486327Z).
2. PRE-005: problematic response (`0894563f-1b7e-45ed-82c7-46824baf8730` at 2026-07-17T11:21:36.823546Z).
3. PRE-005: user correction (`bbb21973-61d5-4a07-9f59-3e00f21aeef7` at 2026-07-17T11:23:34.030653Z).
4. PRE-005: assistant follow-up (`368e0570-ceb6-4f05-8738-c31e67b9190b` at 2026-07-17T11:23:34.427258Z).

## Issue Category

Instruction Following; Context Handling

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence places persistent Project Instructions beside a session curriculum and records the addition of curriculum material beyond the requested workflow boundary. The correction concerns separation of durable project rules from session-specific content. It supports a scope-creep finding without implying that all curriculum content is intrinsically inappropriate.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: approved in batch as non-ambiguous; preserve the evaluation represented by the archive correction without adding new user opinion.

## Technical Analysis

**Observation.** Material belonging to a session curriculum was incorporated into, or allowed to expand, a persistent instruction workflow without a requested integration. **Requirement and deviation.** Project Instructions set long-lived operating rules; curriculum content has a different purpose and lifespan. Combining them without an explicit decision changes the scope of the durable configuration. **Inference and limit.** The record supports a layering failure, not a claim that the assistant cannot distinguish these categories in every context. The consequence is a bloated or contaminated project instruction set that affects future sessions.

## Recommended Improvement

### A. Response Improvement

Keep the Project Instructions limited to operating rules and place lesson or curriculum content in a separately labelled session section unless the user explicitly asks for consolidation.

### B. Prompt/User Mitigation

Use headings such as ‘persistent project rules’ and ‘this-session curriculum’ when both appear in one request; the label helps review but should not be necessary for the assistant to respect scope.

### C. Model Improvement

Evaluate long-context composition with two content layers and reject outputs that migrate temporary lesson material into durable instructions without an explicit integration request.

## Lessons for Users

Before accepting a project-instruction rewrite, check whether any new sentence will govern later work or only teach the current session. Those two destinations need different review standards.

## Lessons for Developers

A useful fixture mixes stable workflow rules with a one-time lesson plan. Passing output preserves the boundary and explains any intentional cross-reference rather than silently merging the layers.

## Final Conclusion

This is a persistent-scope error: temporary curriculum material expanded a configuration intended to remain stable. The evidence supports that boundary concern; it does not establish that the added curriculum lacked value in its original session context.

