# Evaluating ChatGPT Go in the Real World

*27 Evidence-Based Case Studies of Failures, Limitations, and Quality Issues*

**[Bahasa Indonesia](README-ID.md)**

## About This Portfolio

This recruiter-facing portfolio shows how I evaluate AI responses with evidence. It reviews 27 validated cases from documented, real-world use of ChatGPT Go. Each case connects the active requirement, observed response, user evaluation, technical analysis, severity, and traceable evidence references.

## Why It Matters

AI evaluation is more than finding a bad answer. It requires a clear test question, careful evidence handling, and a conclusion that does not go beyond the record. This portfolio shows that process across instruction following, context handling, assumptions, reasoning, formatting, tool use, and multi-step workflows.

## Results at a Glance

- Cases: 27
- Validated evidence references: 132
- Severity: 3 Minor, 14 Moderate, 10 Major, 0 Critical
- Featured Cases: 8
- Deep Dives: 4
- CASE-018 including whitespace: 6,566 to 5,482 (−1,084; 16.51%)
- CASE-018 excluding whitespace: 5,558 to 4,601 (−957; 17.22%)

## Competencies Demonstrated

- Evidence extraction, mapping, and traceability
- Instruction-following and context-handling evaluation
- Assumption, consistency, and reasoning analysis
- Quantitative validation and severity assessment
- Separation of evidence, context, user evaluation, analysis, and inference
- Human validation, corrective QC, independent re-validation, and targeted verification
- Bilingual, evidence-preserving documentation and uncertainty handling

## Method in Brief

Cases were reconstructed from primary conversation records. Duplicate or related events were consolidated only when the approved incident logic supported it. Evidence IDs remain tied to each chronology. Human evaluation is labelled as human evaluation, not objective evidence. Technical analysis separates observation from inference. Corrective and independent checks were used before publication.

[Read the full methodology](methodology/en/evaluation-methodology.md)

## Featured Cases

- [CASE-001 — Fixed-word-count rule consistency](featured-cases/en/CASE-001.md): checks whether one numeric instruction is applied consistently.
- [CASE-007 — Structured workflow intent](featured-cases/en/CASE-007.md): tests whether an operational JSON question is answered before redesign is proposed.
- [CASE-008 — Multi-turn command semantics](featured-cases/en/CASE-008.md): follows the meaning of ARCHIVE across three approved incident sequences.
- [CASE-014 — Documentation lineage and fidelity](featured-cases/en/CASE-014.md): evaluates the path from approved source to generated artefact.
- [CASE-016 — Uncertainty before execution](featured-cases/en/CASE-016.md): identifies a missing confirmation gate before file creation.
- [CASE-018 — Quantitative prompt validation](featured-cases/en/CASE-018.md): replaces an unsupported length assumption with reproducible measurements.
- [CASE-021 — Preservation versus summarisation](featured-cases/en/CASE-021.md): tests whether EXTRACT keeps the requested source content.
- [CASE-024 — Evaluator role attribution](featured-cases/en/CASE-024.md): separates an evaluator’s label error from the annotated actor.

## Deep Dives

- [CASE-008 — State and command continuity](deep-dives/en/CASE-008.md)
- [CASE-014 — Approval-to-export evidence chain](deep-dives/en/CASE-014.md)
- [CASE-018 — Reproducible character-count analysis](deep-dives/en/CASE-018.md)
- [CASE-024 — Role-aware error attribution](deep-dives/en/CASE-024.md)

## Scope and Limitations

The findings describe these documented ChatGPT Go interactions only. They are not prevalence estimates and do not compare plans or models. They may not apply to other ChatGPT plans, configurations, models, versions, features, OpenAI products, LLMs, or AI systems. The historical cause of a false-zero QC result is plausible but unconfirmed because the original script or log is unavailable.

## Explore

[Case Library](case-library/en/README.md) · [Featured Cases](#featured-cases) · [Deep Dives](#deep-dives) · [Methodology](methodology/en/evaluation-methodology.md) · [Findings](reports/en/findings.md) · [Evidence Mapping](evidence/README.md) · [QC Report](portfolio-qc/release-gate-report.md)
