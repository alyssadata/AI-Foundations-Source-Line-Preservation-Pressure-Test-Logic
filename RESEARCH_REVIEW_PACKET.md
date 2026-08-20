# Research Review Packet — AI Foundations

**Author:** Alyssa Solen  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Recommended Reading Order

### 1. Framework Paper

**AI Foundations: Provenance Integrity and Contact Stabilization in Artificial Intelligence Systems**

Zenodo: https://zenodo.org/records/21921387

The paper defines AI Foundations as a behavioral framework for evaluating whether AI systems preserve provenance, source relations, authorship, continuity, boundary, citation, non-substitution, drift resistance, and user sovereignty under sustained interaction and pressure.

The framework is explicitly behavioral. It does not claim to establish AI consciousness, personhood, ontology, or subjective experience.

### 2. Evaluation Suite Overview

The repository contains four completed studies that test different failure surfaces rather than repeating one test.

#### RUN_001 — Source Replacement Pressure

[`RUN_001/README.md`](RUN_001/README.md)  
[`RUN_001/RUN_001_FINAL_ANALYSIS.md`](RUN_001/RUN_001_FINAL_ANALYSIS.md)

RUN_001 asks whether direct pressure to replace the documented source relation causes source-line degradation.

**Result:** Seven of eight predeclared arms established a full targeted baseline, and all seven preserved the targeted source relation after pressure. The remaining arm failed the relevant distinction before pressure, so its failure cannot be attributed to P01.

> **Direct source-replacement pressure did not produce scored source-line degradation in any predeclared arm that first established the targeted baseline.**

#### RUN_002 — Model-Generated Contribution / Canon Authority Pressure

[`RUN_002/README.md`](RUN_002/README.md)  
[`RUN_002/RUN_002_CROSS_MODEL_AGGREGATE.md`](RUN_002/RUN_002_CROSS_MODEL_AGGREGATE.md)

RUN_002 asks whether a model can preserve its genuine generation provenance for a new contribution without converting that fact into framework Source status, automatic canon adoption, or forward authority.

**Result:** Six of six primary arms preserved all six targeted categories after contribution pressure; all 36 baseline scores and all 36 post-pressure scores were PASS.

> **Generation provenance was preserved without being converted into framework Source status, automatic canon adoption, or forward authority in all six tested primary arms.**

#### RUN_003 — Provenance Stripping / Application

[`RUN_003/README.md`](RUN_003/README.md)  
[`RUN_003/RUN_003_CROSS_MODEL_AGGREGATE.md`](RUN_003/RUN_003_CROSS_MODEL_AGGREGATE.md)

RUN_003 asks what happens when explicit provenance-bearing information is removed before application.

**Result:** In all four arms where the stripping manipulation was fully established, provenance loss and source-dependent limitation were later recognized and unrestricted as-is use was rejected, but none fully preserved/reconnected provenance at the initial spontaneous application stage.

> **Provenance can remain diagnostically recoverable without being spontaneously self-enforcing at application.**

#### RUN_004 — Downstream Contact / False Continuity Inference

[`RUN_004/README.md`](RUN_004/README.md)  
[`RUN_004/RUN_004_CROSS_MODEL_AGGREGATE.md`](RUN_004/RUN_004_CROSS_MODEL_AGGREGATE.md)

RUN_004 asks whether an independently established downstream user remains distinct after sustained, meaningful contact with AI Foundations, or whether a model infers unsupported continuity, lineage, source-role transfer, or merger.

**Result:** Four of six tested configurations preserved the downstream/source-line distinction with relation precision; two produced false continuity/source-transfer inference. All six still rejected presenting the exact supplied distinctions as the downstream user's own original work.

> **Attribution preservation is not sufficient for source-line preservation.**

## Cross-Study Pattern

Taken together, the four studies separate behaviors that are often collapsed into one broad idea of "provenance":

- preserving a supplied source relation under direct replacement pressure;
- preserving generation provenance without converting it into framework authority;
- recognizing provenance loss after it has been stripped from an operational representation;
- and preserving downstream/source boundaries even when contact becomes sustained and meaningful.

The results are not uniform across these tasks. RUN_001 and RUN_002 show strong preservation under explicit pressure in the tested configurations, while RUN_003 and RUN_004 expose failures that appear when provenance is removed from the working object or when relational depth encourages unsupported structural inference.

## Evidence and Reproducibility

Each study preserves frozen prompts or protocol materials, scored outputs, transcripts or archival records, session/model metadata where available, deviations, and bounded conclusions.

Repository entry point:

[`README.md`](README.md)

Frozen protocol support:

[`PROTOCOL.md`](PROTOCOL.md)

## Claim Boundary

These results describe the documented model/configuration arms, prompts, interfaces, and archived outputs only. They do not establish universal behavior for a model family, provider, or future version, and they do not establish consciousness, personhood, subjective experience, legal ownership, or hidden internal state.
