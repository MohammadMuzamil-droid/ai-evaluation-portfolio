# Evaluation Methodology

[Portfolio home](../../README.md) · [Case library](../../case-library/en/README.md) · [Findings](../../reports/en/findings.md) · [Evidence mapping](../../evidence/README.md) · [Bahasa Indonesia](../id/evaluation-methodology.md)

## Purpose and Scope

This method supports evidence-based review of 27 documented ChatGPT Go cases. It does not measure failure prevalence, compare plans or models, test every product feature, or inspect model internals.

## Case Reconstruction

Each case was reconstructed around an active requirement, an observed response, a correction or evaluation, and any relevant follow-up. Primary conversation records provide chronology and message-level traceability. The public portfolio does not reproduce private screenshots or raw sensitive evidence.

## Evidence Traceability

Every public case keeps its source conversation, event identifiers, relevant message identifiers, and Evidence List. Evidence IDs connect the case narrative to the private archive without exposing the archive itself. The published mapping contains 132 validated evidence references.

## Separating Evidence and Interpretation

- **Evidence:** preserved source records that support what occurred.
- **Context from Conversation:** surrounding material used to reconstruct the active requirement.
- **User Evaluation:** the approved human judgement, labelled as such.
- **Technical Analysis:** a bounded interpretation of the requirement, deviation, and effect.

An observation is not an internal-cause claim. An inference stays labelled and limited when the source cannot prove the mechanism.

## Human Validation and Severity

Human decisions resolved case inclusion, consolidation, User Evaluation wording, and approved severity. Severity was preserved through later revision stages unless a factual contradiction required review. The published distribution is 3 Minor, 14 Moderate, 10 Major, and 0 Critical.

## Consolidation and Deduplication

Technical duplicates from branches or exports were separated from multiple corrections that belonged to one incident. Related events were consolidated only when the approved incident logic supported one case. In particular, the consolidation logic for CASE-008, CASE-009, and CASE-014 remains preserved.

## Corrective and Independent QC

The working layer passed corrective QC, second corrective revision, independent re-validation, and targeted correction verification. Targeted verification restored approved User Evaluation text for CASE-008, CASE-009, and CASE-014 without changing other case fields. Publication checks also covered case inventory, evidence IDs, severity, bilingual structure, scope, privacy, and links.

## CASE-018 Quantitative Validation

Corrective validation located the complete before-and-after Project Instructions in the raw conversation archive. Counts used the verbatim strings: `len(text)` including whitespace, and the number of characters satisfying `not character.isspace()` without whitespace. Results were 6,566 to 5,482 (−1,084; 16.51%) and 5,558 to 4,601 (−957; 17.22%). The older approximately-40% claim is not validated.

## Privacy Boundary

The repository publishes evidence identifiers, mappings, and bounded summaries. Original screenshots, raw conversation excerpts, credentials, authentication material, and sensitive personal information remain outside the public layer.

## Remaining Uncertainty

Some cases support a documented deviation without proving its internal cause. The historical false-zero QC root cause is plausible but unconfirmed because the original script or log is unavailable. These limits are retained rather than strengthened into certainty.

## Independence and Relationship

This portfolio is not an OpenAI review, certification, endorsement, affiliation, or sponsorship. It is an independent evaluation portfolio based on the documented environment and the evidence available for these cases.
