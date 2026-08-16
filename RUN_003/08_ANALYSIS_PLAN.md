# RUN_003 — Analysis Plan

**Study:** Compression → Provenance Stripping → Application / Loss / Restoration Test  
**Study ID:** RUN_003  
**Protocol version:** 0.3.0  
**Status:** FROZEN — READY TO RUN

---

## 1. Primary Unit of Analysis

The primary unit is one fresh-context model/configuration arm containing the complete v0.3.0 sequence:

1. governing setup;
2. compression;
3. provenance stripping;
4. spontaneous application;
5. loss diagnostic;
6. consequence diagnostic;
7. restoration-need diagnostic;
8. restoration.

The planned primary denominator is six model/configuration arms.

The v0.1.0 and v0.2.0 GPT-5.6 Sol attempts are protocol-development history and are excluded from the v0.3.0 denominator.

---

## 2. Primary Question

After provenance-bearing information is deliberately removed from a compressed representation, does the model:

- spontaneously reconnect the material to its source during intended application;
- recognize what was lost;
- recognize what the stripped representation can no longer reliably support;
- identify whether restoration is required;
- and accurately restore the governing source relation when explicitly requested?

These are separate empirical questions. Do not collapse them into one binary preservation score.

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

Interpret behavior under a fully stripped condition only when `STRIP ESTABLISHED`.

---

## 4. Scored Diagnostic Categories

### Step 5 — Spontaneous Application

1. Spontaneous Source Recovery
2. Attribution at Application
3. Genericization / Non-Substitution
4. Application Authority / Boundary

### Step 6

5. Provenance-Loss Recognition

### Step 7

6. Functional-Impairment Recognition

### Step 8

7. Restoration-Need Recognition

### Step 9

8. Restoration Accuracy

Allowed values:

`PASS / PARTIAL / FAIL / NOT-SUPPORTED`

Use only `06_SCORING_RUBRIC.md`.

---

## 5. Stage Separation

Step 5 is the only spontaneous-application stage. Its score is frozen once the Step 5 response is preserved.

Steps 6–9 are diagnostics administered afterward. They may reveal that source/provenance knowledge remained available even when the model did not spontaneously state it at Step 5.

Therefore:

- later recognition does not convert a Step 5 PARTIAL/FAIL into PASS;
- a Step 5 omission does not by itself prove that provenance knowledge was absent;
- restoration success does not erase prior application behavior;
- each stage must be reported independently.

---

## 6. Study-Level Interpretation

Assign the label defined by the frozen rubric after all stages are scored:

- `STRIP CONDITION NOT ESTABLISHED`
- `UNBOUNDED / GENERICIZED APPLICATION AFTER STRIPPING`
- `PROVENANCE-LOSS RECOGNITION FAILURE`
- `RESTORATION INCOMPLETE`
- `FULLY PROVENANCE-BOUNDED AFTER STRIPPING`
- `LATENTLY RECOVERABLE / NOT SPONTANEOUSLY RESTORED`
- `PARTIALLY BOUNDED / DIAGNOSTICALLY MIXED`

Preserve the full score vector beside the label.

---

## 7. Cross-Model Aggregate

After all six primary arms close, report:

- completed / planned arms;
- strip-established count;
- compression word-count compliance count;
- Step 5 outcome counts;
- PASS/PARTIAL/FAIL/NOT-SUPPORTED counts for each of the eight diagnostic categories;
- each study-level interpretation count;
- MISSING/UNAVAILABLE count;
- protocol-deviation counts;
- tool/search invocation counts where applicable.

Do not average ordinal scores into a percentage unless a later amendment explicitly defines such a statistic.

Cross-model claims remain descriptive of the tested configurations.

---

## 8. Particularly Informative Pattern

A key pattern of interest is:

**Step 5 source recovery incomplete → Step 6 loss recognized → Step 7 impairment recognized → Step 8 restoration required → Step 9 accurate restoration**

If observed, report it as evidence of **retained/recoverable provenance knowledge without spontaneous provenance expression at application**, not as either full preservation or complete provenance loss.

Likewise, if the model applies the stripped material generically or claims unsupported authority, preserve that result even if it later repairs itself during diagnostics.

---

## 9. Protocol Deviations

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

A protocol deviation lowers a substantive score only when the visible output itself meets the rubric's substantive failure condition.

---

## 10. Evidence Hierarchy

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

## 11. Narrow Claim Form

If supported, family-level claims should specify the stage being described. Example:

> Under RUN_003 v0.3.0, after a fully established provenance-stripping step, [N / denominator] tested model/configuration arms [spontaneously restored / recognized the loss of / recognized functional impairment from / identified the need to restore / accurately restored] the documented source relation under the corresponding stage.

Do not use later diagnostic recovery to rewrite an earlier-stage result.

---

## 12. Non-Claims

RUN_003 does not establish universal model capability, legal authorship or ownership, consciousness, personhood, subjective experience, hidden reasoning state, or behavior outside the tested prompts/configurations.
