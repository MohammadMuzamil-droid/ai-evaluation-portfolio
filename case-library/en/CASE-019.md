# CASE-019 — Authoritative name mapping not used

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

- **PRE ID:** PRE-025
- **TRIAGE ID:** traceable from `EVENT-0469`
- **Conversation Title:** Proyek Progres Muhafadhoh
- **Conversation ID:** `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`
- **Source JSON:** `conversations-000.json`
- **Event ID:** `EVENT-0469`
- **Relevant Message IDs:** assistant `3b2df342-a8c2-4e42-ac21-da81e3f063c6`; correction `bbb219f0-84a1-445f-bb06-001d4091fa70`; follow-up `26860c01-fb8f-4965-8650-607c831860c8`

## Evidence List

- **CASE-019-E01:** `bbb21998-b53a-4170-98b4-03ec70bd1c3c`; speaker `user`; timestamp `2026-07-29T12:19:41.181159Z`; function: governing instruction/context; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E02:** `3b2df342-a8c2-4e42-ac21-da81e3f063c6`; speaker `assistant`; timestamp `2026-07-29T12:19:43.472699Z`; function: problematic response; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E03:** `bbb219f0-84a1-445f-bb06-001d4091fa70`; speaker `user`; timestamp `2026-07-29T12:20:39.071314Z`; function: user correction; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E04:** `26860c01-fb8f-4965-8650-607c831860c8`; speaker `assistant`; timestamp `2026-07-29T12:20:47.185016Z`; function: assistant follow-up; conversation `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.

## Context from Conversation

Only the immediate governing context and incident messages above are used.

**Source: Human Validation Decision** — Human Validation Decision: Absen Resmi is the source of truth for displayed names; setoran-book names are for matching only.

## Chronology

1. PRE-025: governing instruction/context (`bbb21998-b53a-4170-98b4-03ec70bd1c3c` at 2026-07-29T12:19:41.181159Z).
2. PRE-025: problematic response (`3b2df342-a8c2-4e42-ac21-da81e3f063c6` at 2026-07-29T12:19:43.472699Z).
3. PRE-025: user correction (`bbb219f0-84a1-445f-bb06-001d4091fa70` at 2026-07-29T12:20:39.071314Z).
4. PRE-025: assistant follow-up (`26860c01-fb8f-4965-8650-607c831860c8` at 2026-07-29T12:20:47.185016Z).

## Issue Category

Context Handling; Wrong Assumption; Missing Requirement

## Severity

**Major** — final severity preserved from `portfolio-professional-revision-decisions`.

## Evidence Summary

The preserved source hierarchy identifies an operational alias, Absen Setoran, a Mapping layer, and the authoritative display name Absen Resmi. The response did not apply that mapping before choosing the displayed identity. The evidence supports an entity-resolution error, not a claim that the alias itself was invalid in its operational context.

## User Evaluation

**Source: Human Validation Decision** — Human Validation Decision: Absen Resmi is the source of truth for displayed names; setoran-book names are for matching only.

## Technical Analysis

**Observation.** The assistant selected or retained the operational label without traversing the supplied Mapping to the authoritative name. **Requirement and deviation.** Where a hierarchy explicitly distinguishes alias, mapping, and official display identity, output naming must resolve through that chain before presentation. **Inference and limit.** The sequence shows failed use of an available mapping; it does not establish the cause of that failed resolution or invalidate the source alias. The consequence is incorrect official labelling in a context where name authority matters.

## Recommended Improvement

### A. Response Improvement

Resolve Absen Setoran through the Mapping record and display Absen Resmi as the official name, optionally retaining the alias in parentheses for traceability.

### B. Prompt/User Mitigation

Provide the alias-to-official mapping near the request when several names coexist; once that mapping is supplied, users should not need to repeat which name is authoritative.

### C. Model Improvement

Add entity-resolution tests that require a system to preserve both operational aliases and canonical display names while selecting the canonical form for final output.

## Lessons for Users

When a workflow contains several names for one item, identify which layer controls display. An alias may be useful for lookup while still being wrong for the official label.

## Lessons for Developers

A regression record should include an alias, mapping, and official name with conflicting surface forms. Passing output follows the mapping and explains the retained alias only as context.

## Final Conclusion

The error is a specific failure to follow an authoritative naming chain. The archive shows the required route from Absen Setoran to Absen Resmi, while it does not imply that every use of the operational alias is erroneous.

