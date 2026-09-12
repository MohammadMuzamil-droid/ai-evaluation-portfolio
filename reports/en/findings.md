# Portfolio Findings

[Portfolio home](../../README.md) · [Case library](../../case-library/en/README.md) · [Methodology](../../methodology/en/evaluation-methodology.md) · [Evidence mapping](../../evidence/README.md) · [Bahasa Indonesia](../id/findings.md)

## What This Portfolio Shows

The 27 cases document quality issues in real-world ChatGPT Go use. The strongest pattern is instruction following, but the cases also show context, reasoning, format, tool-use, and workflow problems. Severity describes the approved context of each case, not a general product rating.

## Non-Exclusive Issue Categories

| Issue category | Cases |
|---|---:|
| Instruction Following | 19 |
| Formatting Error | 11 |
| Context Handling | 8 |
| Missing Requirement | 6 |
| Tool Usage | 6 |
| Inconsistency | 5 |
| Reasoning Error | 5 |
| Wrong Assumption | 2 |
| Contradiction | 1 |
| Hallucination | 1 |

Categories overlap, so the total category count is greater than 27. These counts describe this portfolio only. They are not prevalence estimates for ChatGPT Go and are not comparisons with other plans, models, configurations, or versions.

## Evaluation Patterns

### Requirement interpretation

Several cases show why an evaluator must identify the active requirement before judging output quality. Examples include the exact-word-count distinction in [CASE-001](../../case-library/en/CASE-001.md), the operational JSON question in [CASE-007](../../case-library/en/CASE-007.md), and the summary stage in [CASE-023](../../case-library/en/CASE-023.md).

### Context and workflow continuity

Multi-step work can fail even when each response appears reasonable in isolation. [CASE-008](../../case-library/en/CASE-008.md) tests a repeated command contract. [CASE-014](../../case-library/en/CASE-014.md) follows approved content through retrieval and export. [CASE-016](../../case-library/en/CASE-016.md) checks whether uncertainty is resolved before execution.

### Fidelity and measurable claims

Presentation quality does not replace source fidelity. [CASE-021](../../case-library/en/CASE-021.md) separates preservation from summarisation. [CASE-018](../../case-library/en/CASE-018.md) shows why a feasibility claim should be tested with reproducible measurements.

### Role and responsibility

[CASE-024](../../case-library/en/CASE-024.md) shows that an evaluator must identify who made a classification decision before assigning error or corrective action.

## Limits

The portfolio does not test every ChatGPT Go feature or interaction. It does not establish internal causes, general failure rates, or performance differences between products. Findings remain bounded to the evidence, human validation, approved severity, and uncertainty recorded in each case.
