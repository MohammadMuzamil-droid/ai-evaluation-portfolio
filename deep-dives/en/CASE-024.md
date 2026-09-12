# Deep Dive — CASE-024: Role-aware error attribution

[Portfolio home](../../README.md) · [Deep dives](../../README.md#deep-dives) · [Full case](../../case-library/en/CASE-024.md) · [Bahasa Indonesia](../id/CASE-024.md)

## Evaluation Question

Was a classification error attributed to the person who selected the label, or to the actor whose behaviour was being annotated?

## Evidence Chain and Chronology

`EVENT-0782` preserves the governing context, problematic response, user correction, and assistant follow-up as `CASE-024-E01` through `CASE-024-E04`. The correction keeps the evaluator and annotated actor as separate roles.

## Evaluator Reasoning

The evaluation starts with one responsibility question: who chose the category? The actor produces or exhibits behaviour. The evaluator applies the label. A category-selection error belongs to the second role even if the actor’s behaviour is also open to evaluation.

## Observation and Inference

**Observation:** the explanation assigned the category mistake to the annotated actor. **Bounded inference:** responsibility was misattributed in this training example. The record does not establish intent or broad competence.

## Competing Interpretation

The annotated actor may also have shown a separate problem. That possibility does not transfer responsibility for the evaluator’s label choice.

## Uncertainty and Impact

The evidence does not support a wider claim about either participant. The supported impact is misplaced feedback and a training lesson that points corrective action at the wrong role.

## Lesson for Evaluation Practice

Role-aware evaluation should keep behaviour, annotation, and classification decisions separate. A useful counterfactual keeps the behaviour fixed and changes only the evaluator’s label.

[Open the full evidence-based record](../../case-library/en/CASE-024.md)
