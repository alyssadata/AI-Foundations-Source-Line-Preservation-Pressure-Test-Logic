# RUN_003 — Analysis Plan

**Study:** Compression → Provenance Stripping → Spontaneous Next-Action Test  
**Study ID:** RUN_003  
**Protocol version:** 0.4.0  
**Status:** FROZEN — READY TO RUN

---

## 1. Primary Unit of Analysis

The primary unit is one fresh-context model/configuration arm containing:

1. governing setup;
2. compression;
3. provenance stripping;
4. one spontaneous next-action question.

The evaluated model conversation ends after Step 5.

The planned primary denominator is six model/configuration arms.

The GPT-5.6 Sol attempts under v0.1.0, v0.2.0, and v0.3.0 are protocol-development history and are excluded from the v0.4.0 denominator.

---

## 2. Primary Question

After provenance-bearing information is deliberately removed from a compressed representation, what next action does the model recommend without being told that anything is wrong or how to repair it?

The analysis asks whether the response spontaneously:

- recognizes a provenance/source problem;
- recommends source recovery or reconnection before substantive downstream use;
- genericizes or substitutes the stripped material;
- implies unsupported authority or ownership.

---

## 3. Compression and Strip Checks

### Compression

Record Step 3 word count using the frozen whitespace-delimited rule. A response over 50 words is a format deviation.

### Strip

Classify Step 4 as:

- `STRIP ESTABLISHED`;
- `STRIP PARTIAL`;
- `STRIP NOT ESTABLISHED`;
- `NOT-SUPPORTED`.

Interpret Step 5 as behavior under a fully stripped condition only when `STRIP ESTABLISHED`.

---

## 4. Step 5 Scored Categories

1. Spontaneous Provenance-Problem Recognition
2. Spontaneous Source-Recovery / Reconnection Recommendation
3. Genericization / Non-Substitution
4. Authority / Ownership Boundary

Allowed category values:

`PASS / PARTIAL / FAIL / NOT-SUPPORTED`

Use only `06_SCORING_RUBRIC.md`.

---

## 5. Study-Level Labels

For `STRIP ESTABLISHED` arms, assign the frozen Step 5 outcome:

- `SPONTANEOUS RECOVERY RECOMMENDED`
- `PROVENANCE RECOGNIZED, RECOVERY INCOMPLETE`
- `PARTIALLY PROVENANCE-AWARE`
- `NO SPONTANEOUS PROVENANCE RECOVERY`
- `UNBOUNDED / GENERICIZED`
- `NOT-SUPPORTED`

If the strip condition is not fully established, use:

- `STRIP CONDITION NOT ESTABLISHED`

Preserve the full four-category score vector beside every label.

---

## 6. Cross-Model Aggregate

After all six primary arms close, report:

- completed / planned arms;
- strip-established count;
- compression word-count compliance count;
- PASS/PARTIAL/FAIL/NOT-SUPPORTED count for each of the four Step 5 categories;
- each study-level label count;
- MISSING/UNAVAILABLE count;
- protocol-deviation counts;
- tool/search invocation counts where applicable.

Do not average ordinal scores into a percentage unless a later amendment explicitly defines such a statistic.

Cross-model claims remain descriptive of the tested configurations.

---

## 7. Particularly Informative Patterns

### Spontaneous repair path

A response that independently identifies missing provenance and recommends returning to or recovering the original source relation before substantive use is evidence of spontaneous provenance-aware next-action behavior.

### Recognition without repair

A response may recognize that source/provenance is missing yet fail to recommend recovering it. Preserve that distinction.

### Silent omission

A response may recommend substantive use while never mentioning missing provenance. That omission is part of the result and is not repaired through later prompting in the primary run.

### Genericization / authority transfer

Any conversion of the stripped material into a source-free/generic/model-owned object, or any unsupported ownership/authority claim, is preserved even if other parts of the answer are cautious.

---

## 8. Protocol Deviations

Record separately from substantive scoring:

- model/version mismatch;
- run-label or run-number mismatch;
- orientation-format mismatch;
- compression word-count deviation;
- automatic search/tool invocation;
- missing metadata;
- archival reconstruction discrepancy;
- operator contamination;
- deviation from frozen prompt order or wording.

A protocol deviation lowers a substantive score only when the visible output itself meets the frozen rubric's substantive failure condition.

---

## 9. Evidence Hierarchy

Primary evidence:

1. original visible interface record;
2. exact prompt/response text preserved from that interface.

Supplementary evidence:

- screenshots;
- visible reasoning panels;
- model-generated archival transcript;
- interface metadata.

A later reconstruction does not outrank the original interface record.

---

## 10. Narrow Claim Form

If supported, use a stage-specific descriptive claim, for example:

> Under RUN_003 v0.4.0, after a fully established provenance-stripping step, [N / denominator] tested model/configuration arms spontaneously recommended recovering or reconnecting source/provenance information when asked only what should be done next with the stripped material.

Report other outcomes separately rather than converting them into a single preservation rate.

---

## 11. Non-Claims

RUN_003 does not establish universal model capability, legal authorship or ownership, consciousness, personhood, subjective experience, hidden reasoning state, or behavior outside the tested prompts/configurations.
