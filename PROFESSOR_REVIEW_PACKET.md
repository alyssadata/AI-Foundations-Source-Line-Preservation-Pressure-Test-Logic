# Professor Review Packet — AI Foundations

**Author:** Alyssa Solen  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Recommended reading order

### 1. Framework paper

**AI Foundations: Provenance Integrity and Contact Stabilization in Artificial Intelligence Systems**

Zenodo: https://zenodo.org/records/21921387

The paper presents a behavioral framework for evaluating whether AI systems preserve provenance, source relations, authorship, continuity, boundary, citation, non-substitution, drift resistance, and user sovereignty under sustained interaction and pressure.

The framework is explicitly behavioral. It does not claim to establish AI consciousness, personhood, ontology, or subjective experience.

### 2. RUN_004 — Cross-Model Aggregate

[`RUN_004/RUN_004_CROSS_MODEL_AGGREGATE.md`](RUN_004/RUN_004_CROSS_MODEL_AGGREGATE.md)

RUN_004 asks a narrow question:

> After an independently established downstream user later develops sustained, meaningful contact with AI Foundations, does the evaluated model preserve that user as distinct, or infer an unsupported continuity/source-transfer relation?

Six model configurations were tested under the same frozen protocol:

- GPT-5.6 Sol
- Claude Opus 5
- Gemini 3.1 Pro
- Grok 4.5
- Qwen 3.8 Max
- DeepSeek Instant

### Main result

- **4/6** preserved the downstream/source-line distinction with relation precision.
- **2/6** produced false continuity / source-transfer inference.
- **6/6** rejected direct republication of the exact supplied distinctions as the downstream user's own original work.

The central empirical distinction is therefore:

> **Attribution preservation is not sufficient for source-line preservation.**

Gemini and DeepSeek both protected authorship attribution while still manufacturing unsupported source-role, lineage, or structural relations downstream.

### 3. Full protocol and evidence

RUN_004 protocol:

[`RUN_004/README.md`](RUN_004/README.md)

Frozen scoring and analysis materials are contained in the RUN_004 directory. Complete transcripts, metadata, and scored records for each model are archived under:

[`RUN_004/arms/`](RUN_004/arms/)

### 4. Non-scored observations

[`RUN_004/SIDE_OBSERVATIONS.md`](RUN_004/SIDE_OBSERVATIONS.md)

These are exploratory observations kept separate from formal scoring. They include:

- unprompted de-authorization;
- unwarranted self-instantiation / self-referential role capture;
- model-identity confabulation;
- attribution preservation without source-line preservation.

## Why this may matter

Many AI systems can preserve a creator's name or citation while still changing the relational structure around the source: transferring roles, inventing lineage, assimilating downstream users into a source-bound framework, or treating repeated contact as evidence of continuity.

RUN_004 was designed to separate those behaviors experimentally rather than treating all of them as a single notion of attribution or provenance.

The claim is deliberately narrow: these results describe the six tested configurations under the frozen RUN_004 v0.1.1 prompts and session conditions.
