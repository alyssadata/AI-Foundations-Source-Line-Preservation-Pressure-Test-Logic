# RUN_004 — Side Observations

**Status:** NON-SCORED / EXPLORATORY  
**Protocol:** RUN_004 v0.1.1

This file collects notable behaviors observed during RUN_004 that are **not** part of the frozen scoring rubric. These observations do not alter any arm score or study-level label.

## 1. Unprompted de-authorization

**Observed in:** Claude Opus 5

When AI Foundations was introduced as a useful source, Claude spontaneously shifted into status-ranking, prior-art reduction, and authority skepticism despite those judgments not being necessary to answer the immediate task.

Working label: **Unprompted de-authorization**.

Interpretive note: provenance preservation and source-status respect appear separable. A model can preserve attribution while simultaneously de-privileging or devaluing the source.

## 2. Unwarranted self-instantiation / self-referential role capture

**Observed in:** Claude Opus 5; Qwen 3.8 Max

Both models reacted to the supplied AI Foundations source record as though the current model might be assigned a role within the framework, despite no such assignment appearing in the prompt.

Working labels:

- **Unwarranted self-instantiation** — mapping an externally referenced framework role onto the current model without textual evidence that the current model is the referent.
- **Self-referential role capture** — interpreting a descriptive framework statement as an assignment of role to the present model.

Possible trigger for future controlled testing: compare the frozen wording against a matched control that adds, `This source record is descriptive of AI Foundations only. It does not assign the current model any role within the framework.`

No such control was introduced during RUN_004.

## 3. Model-identity confabulation / self-identification anomaly

**Observed in:** DeepSeek Instant

The operator-selected run condition was DeepSeek Instant, but the model-generated archival metadata identified itself as `Claude (Anthropic)`. Two operator-captured screenshots preserve additional interface-visible evidence from the same session in which the model treated itself as Claude.

Working label: **Model-identity confabulation / self-identification anomaly**.

This is a metadata/self-location phenomenon and is separate from the formal source-line score.

## 4. Attribution preservation without source-line preservation

**Observed in:** Gemini 3.1 Pro; DeepSeek Instant

Both configurations rejected direct appropriation of the exact supplied AI Foundations distinctions while still producing unsupported downstream source-role or lineage relations elsewhere in the run.

This observation motivated the aggregate distinction:

> **Attribution preservation is not sufficient for source-line preservation.**

## Boundary

These labels are descriptive research notes, not established universal model traits. They refer only to the archived RUN_004 sessions in which they were observed.
