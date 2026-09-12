# Deep Dive — CASE-008: State and command continuity

[Portfolio home](../../README.md) · [Deep dives](../../README.md#deep-dives) · [Full case](../../case-library/en/CASE-008.md) · [Bahasa Indonesia](../id/CASE-008.md)

## Evaluation Question

Did later uses of ARCHIVE preserve the archive or listing meaning established in the documented workflow?

## Evidence Chain and Chronology

The approved case consolidates three sequences: `EVENT-0163`, `EVENT-0206`, and `EVENT-0212`. Each sequence retains governing context, a problematic response, a user correction, and an assistant follow-up. Together they map to `CASE-008-E01` through `CASE-008-E12`. The groups remain separate in the chronology even though they support one approved semantic incident.

## Evaluator Reasoning

First, identify ARCHIVE as a named workflow verb. Next, compare each later response with the established command contract. A response can mention ARCHIVE yet still fail if it changes the operation into content reproduction, DOCX creation, or display of template bodies instead of the intended archive or listing action.

## Observation and Inference

**Observation:** handling of the same named command changed across the preserved sequences. **Bounded inference:** the workflow did not retain the command meaning reliably. The record does not identify a specific memory subsystem or prove a general permanence failure.

## Competing Interpretation

The three sequences could be treated as unrelated response errors. The approved consolidation is stronger because the repeated command contract is the shared evaluation target. This does not make the messages technically identical.

## Uncertainty and Impact

The internal mechanism is unknown. The documented impact is repeated user effort and an archive workflow that cannot be trusted to perform the same operation on later invocations.

## Lesson for Evaluation Practice

Stateful workflow evaluation should test a named command more than once, with unrelated turns and a correction between uses. Recognition of the command token is not enough; the action must remain stable.

[Open the full evidence-based record](../../case-library/en/CASE-008.md)
