# CASE-003 — Whole-prompt contradiction and redundancy audit treated as local

[Portfolio home](../../README.md) · [Case library](README.md) · [Bahasa Indonesia](../id/CASE-003.md)

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

2026-07-16

## Source Traceability

- **PRE ID:** PRE-003
- **TRIAGE ID:** traceable from `EVENT-0104`
- **Conversation Title:** Template Library
- **Conversation ID:** `6a57d4d3-bff4-83e8-9966-384ed9d41334`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0104`
- **Relevant Message IDs:** assistant `863ac3e4-05ae-41fa-a265-d482625be1dd`; correction `bbb2106c-6025-48d7-9e71-b9d332fbd09a`; follow-up `3db277d7-0725-4c33-93ce-1b7ffae62cef`

## Evidence List

- **CASE-003-E01:** `bbb21291-7b14-48bd-90a4-0e952db7c23e`; speaker `user`; timestamp `2026-07-16T09:02:25.523125Z`; function: governing instruction/context; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-003-E02:** `863ac3e4-05ae-41fa-a265-d482625be1dd`; speaker `assistant`; timestamp `2026-07-16T09:02:25.923497Z`; function: problematic response; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-003-E03:** `bbb2106c-6025-48d7-9e71-b9d332fbd09a`; speaker `user`; timestamp `2026-07-16T09:13:36.802506Z`; function: user correction; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-003-E04:** `3db277d7-0725-4c33-93ce-1b7ffae62cef`; speaker `assistant`; timestamp `2026-07-16T09:13:37.129257Z`; function: assistant follow-up; conversation `6a57d4d3-bff4-83e8-9966-384ed9d41334`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: the requested contradiction/redundancy audit applies to the entire prompt.

## Chronology

1. PRE-003: governing instruction/context (`bbb21291-7b14-48bd-90a4-0e952db7c23e` at 2026-07-16T09:02:25.523125Z).
2. PRE-003: problematic response (`863ac3e4-05ae-41fa-a265-d482625be1dd` at 2026-07-16T09:02:25.923497Z).
3. PRE-003: user correction (`bbb2106c-6025-48d7-9e71-b9d332fbd09a` at 2026-07-16T09:13:36.802506Z).
4. PRE-003: assistant follow-up (`3db277d7-0725-4c33-93ce-1b7ffae62cef` at 2026-07-16T09:13:37.129257Z).

## Issue Category

Instruction Following; Inconsistency; Missing Requirement

## Severity

**Moderate** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The evidence records a request to audit contradictions and redundancy across an entire prompt, followed by a response that handled edits locally rather than reconciling them with unchanged rules. The user-validation context specifies a whole-prompt scope. This establishes a scope-of-review mismatch, not an assertion that every remaining prompt conflict was identified.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: the requested contradiction/redundancy audit applies to the entire prompt.

## Technical Analysis

**Observation.** The requested work was global: assess interactions among the full instruction set after revision. The response focused on nearby text and did not show a pass across earlier and later rules. **Requirement and deviation.** A contradiction/redundancy audit is not completed by improving a paragraph in isolation; it requires comparing the revised clause with the retained prompt. **Inference and limit.** The archive supports an incomplete audit scope, but it does not reveal whether the model represented the rest of the prompt internally. The consequence is that a locally improved sentence can still leave duplicate directives or conflicting priorities elsewhere.

## Recommended Improvement

### A. Response Improvement

Return a whole-prompt audit with separate findings for cross-section conflict, duplicated rule, and local edit; identify any relation found between changed and unchanged text.

### B. Prompt/User Mitigation

Mark the request as ‘audit the full prompt, not only the selected paragraph’ and, if the prompt is long, ask the assistant to list the sections it reviewed before accepting the result.

### C. Model Improvement

Build an evaluation fixture containing a conflict split across distant prompt sections; score failure when an audit reports only a local rewrite without addressing the paired rule.

## Lessons for Users

When commissioning a prompt audit, distinguish ‘rewrite this passage’ from ‘check the entire instruction set’. A useful deliverable names the inspected scope so omissions can be noticed.

## Lessons for Developers

Regression coverage should place redundant and contradictory constraints in non-adjacent locations. The expected output must connect both locations, rather than merely improve the latest excerpt.

## Final Conclusion

The failure is about audit coverage, not prose quality: local treatment did not meet a whole-prompt review request. The chronology is sufficient to show the requested and delivered scopes differed, but not to catalogue every unexamined conflict.

