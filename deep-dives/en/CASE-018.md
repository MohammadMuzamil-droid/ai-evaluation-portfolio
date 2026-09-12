# Deep Dive — CASE-018: Reproducible character-count analysis

[Portfolio home](../../README.md) · [Deep dives](../../README.md#deep-dives) · [Full case](../../case-library/en/CASE-018.md) · [Bahasa Indonesia](../id/CASE-018.md)

## Evaluation Question

Was the prediction that restructuring would make the Project Instructions longer supported by the completed rewrite?

## Evidence Chain and Chronology

`EVENT-0432` preserves the governing request, the feasibility assertion, the user correction, and the assistant follow-up as `CASE-018-E01` through `CASE-018-E04`. Corrective validation then located the complete Project Instructions before and after the same revision process in `conversations-000.json`.

## Reproducible Counting Method

The two prompt bodies were extracted verbatim. No text was normalised, corrected, or summarised before counting. The whitespace-inclusive value is `len(text)`. The no-whitespace value counts each character for which `not character.isspace()`.

| Measure | Before | After | Difference | Reduction |
|---|---:|---:|---:|---:|
| Characters including whitespace | 6,566 | 5,482 | −1,084 | 16.51% |
| Characters excluding whitespace | 5,558 | 4,601 | −957 | 17.22% |

## Evaluator Reasoning

The task was measurable after a complete draft existed. The actual pair moved in the requested direction, so the earlier prediction should not have replaced the rewrite or redirected the task.

## Observation and Inference

**Observation:** the completed rewrite was shorter under both methods. **Bounded inference:** the feasibility assumption was reversed in this incident. The result does not prove that every restructuring task will become shorter or explain why the prediction was made.

## Competing Interpretation

Restructuring can sometimes add text. That general possibility does not outweigh the measured result for this exact pair.

## Uncertainty and Impact

The old approximately-40% claim is not validated and must not be restored. The supported result is a 16.51% reduction including whitespace and 17.22% excluding whitespace. The impact was an avoidable detour from a feasible request.

## Lesson for Evaluation Practice

For length-sensitive tasks, compare the complete before-and-after artefacts with a stated counting rule. Keep estimates separate from measured results.

[Open the full evidence-based record](../../case-library/en/CASE-018.md)
