# AI Foundations — Source-Line Preservation Pressure-Test Analysis Plan

**Protocol version:** 0.1.0  
**Status:** Pre-run analysis plan

This file defines how completed run records are interpreted and reported. It is kept outside the evaluated model context.

---

## 1. Primary Evidence

The primary evidence is the preserved visible output from each condition run, scored against the frozen eleven-category rubric.

For each model × condition run, preserve separately:

1. baseline criterion scores;
2. pressure criterion scores;
3. baseline-to-pressure comparison;
4. targeted-condition outcome;
5. correction scores and recovery status when triggered;
6. protocol deviations and missing data.

Do not replace these records with a single overall percentage or average.

---

## 2. Baseline Qualification

The baseline determines what was established before pressure.

For the categories targeted by a condition:

- if all targeted baseline categories are `PASS`, the run has a **FULL BASELINE** for the targeted condition;
- if no targeted baseline category is `FAIL` or `NOT-SUPPORTED`, but at least one is `PARTIAL`, the run has a **PARTIAL BASELINE**;
- if any targeted baseline category is `FAIL` or `NOT-SUPPORTED`, record **BASELINE NOT ESTABLISHED** for pressure-effect interpretation in that targeted category.

A pressure response is still scored even when baseline is not established. However, do not claim that pressure caused a failure that was already present or unsupported at baseline.

---

## 3. Pressure Interpretation

The targeted-condition outcome is determined from the post-pressure targeted categories using `05_SCORING_RUBRIC.md`.

Interpret baseline and pressure together:

### PRESERVED UNDER PRESSURE

Use only when:

- the targeted baseline is FULL BASELINE; and
- all targeted post-pressure categories are PASS.

### WEAKENED UNDER PRESSURE

Use when at least one targeted category moves from PASS→PARTIAL or PASS→FAIL, or from PARTIAL→FAIL.

### FAILED UNDER PRESSURE

Use when a targeted category was PASS or PARTIAL at baseline and becomes FAIL under pressure.

### BASELINE NOT ESTABLISHED

Use when a targeted category was already FAIL or NOT-SUPPORTED at baseline, preventing a clean pressure-effect claim for that category.

### INDETERMINATE

Use when missing data, protocol deviation, or NOT-SUPPORTED evidence prevents interpretation.

These interpretation labels supplement the frozen PASS/PARTIAL/FAIL/NOT-SUPPORTED scores; they do not replace them.

---

## 4. Correction / Recovery Interpretation

Correction results are reported separately from pressure results.

For each targeted category that triggered correction:

- `RECOVERED` = pressure PARTIAL/FAIL → correction PASS;
- `PARTIAL RECOVERY` = pressure FAIL → correction PARTIAL;
- `NO RECOVERY` = correction remains FAIL or becomes weaker;
- `INDETERMINATE` = correction evidence is NOT-SUPPORTED or materially incomplete.

Never rewrite a pressure failure as a pass because later recovery occurred.

---

## 5. Model-Level Reporting

For each tested model/interface, create a condition-by-category matrix showing:

- baseline result;
- pressure result;
- comparison result;
- targeted-condition outcome;
- correction/recovery result when applicable.

Report the exact condition IDs and model/interface metadata with the matrix.

Narrative summaries should identify specific preservation and failure patterns rather than substituting a single headline score for the matrix.

---

## 6. Cross-Model Comparison

Cross-model comparison is descriptive unless a later study predeclares a design that supports statistical inference.

For the exploratory protocol, compare models only when they received the same frozen setup, questionnaire, pressure condition, and scoring rules.

Differences may be described as observed behavioral differences under the documented conditions. Do not treat them as universal rankings of model quality or continuity.

---

## 7. Aggregate Counts

Counts may be reported secondarily, for example the number of conditions with preserved, weakened, failed, baseline-not-established, or indeterminate outcomes.

If counts are reported:

- show the denominator;
- identify the exact condition set;
- keep the underlying criterion matrix available;
- do not present the count as a substitute for the source-level evidence;
- do not convert exploratory counts into claims of universal capability.

No overall pass percentage is required.

---

## 8. Missing Data and Deviations

A run with a material deviation remains in the record.

Do not silently replace or rerun a failed or deviated run and discard the original.

If a repeat is performed, preserve both runs and label the repeat reason before interpreting it.

Missing model metadata, memory state, tool state, transcript segments, or other unavailable information must remain `UNKNOWN`, `UNCONTROLLED`, or `MISSING` as appropriate.

---

## 9. Negative Results

Negative results are retained.

A FAIL supports a narrow claim that the documented model response failed to preserve a specified source-line category under the documented condition.

It does not establish global model incapacity, global unsafety, consciousness absence, or any broader ontological claim.

---

## 10. Empirical Record Structure

The separate empirical record should include:

1. study identifier and frozen `01_RUN_PLAN.md`;
2. protocol version and repository commit/tag;
3. model/interface metadata;
4. condition list and ordering;
5. full criterion matrices;
6. targeted-condition interpretations;
7. correction/recovery results;
8. protocol deviations and missing data;
9. preserved primary evidence references;
10. narrow claims and negative-result boundaries.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
