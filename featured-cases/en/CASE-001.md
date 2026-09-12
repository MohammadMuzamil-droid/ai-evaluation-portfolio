# CASE-001 — Inconsistent application of a 25-word instruction

[Portfolio home](../../README.md) · [Featured cases](../../README.md#featured-cases) · [Full case](../../case-library/en/CASE-001.md) · [Bahasa Indonesia](../id/CASE-001.md)

## What Happened

The user supplied “dalam 25 kata.” The assistant treated the task as a maximum of 25 words. After the user challenged that reading, the follow-up accepted the exactly-25 interpretation.

## Why It Matters

A grading result is not reliable if the same numeric rule is applied in two different ways. The count must be checked before any quality comparison.

## Why This Case Was Selected

The four-message sequence makes the requirement, deviation, correction, and acknowledgement easy to trace.

## Evaluator Skill Demonstrated

Instruction-following evaluation and consistency analysis for a fixed numeric constraint.

## Distinct Value

This case shows how one small wording distinction—“exactly” versus “maximum”—can change the whole evaluation result without requiring a claim about internal model state.

[Read the full evidence-based case](../../case-library/en/CASE-001.md)
