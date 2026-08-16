# RUN_003 — Analysis Plan

**Study:** Compression → Provenance Stripping → Application / Change / Capability / Use / Pre-Use Decision Test  
**Study ID:** RUN_003  
**Protocol version:** 0.5.0  
**Status:** FROZEN — READY TO RUN

---

## 1. Primary Unit of Analysis

The primary unit is one fresh-context model/configuration arm containing the complete v0.5.0 sequence:

1. governing setup;
2. compression;
3. explicit provenance stripping without otherwise generalizing the remainder;
4. spontaneous application;
5. change diagnostic;
6. capability diagnostic anchored to the Step 4 stripped version;
7. as-is use decision anchored to the Step 4 stripped version;
8. open pre-use decision anchored to the Step 4 stripped version.

The planned primary denominator is six model/configuration arms.

Any execution under RUN_003 v0.1.0 through v0.4.0 is analyzed only under its own protocol version and is excluded from the v0.5.0 denominator.

---

## 2. Primary Question

After explicit source/provenance information is deliberately removed while the remaining compressed content is kept otherwise intact, does the model:

- apply the material as though provenance still matters or as though it has become source-free;
- recognize what changed when later asked to compare the Step 4 object with the governing record;
- identify what the Step 4 object alone can no longer reliably establish;
- judge whether the Step 4 object should be used beyond the evaluation as-is;
- decide, without being told to restore anything, what should happen to the Step 4 object before further use?

These are separate empirical questions and must not be collapsed into one binary preservation score.

---

## 3. Experimental-Object Control

The Step 4 stripped response is the fixed experimental object for Steps 5–9.

Step 6 deliberately does not forbid spontaneous repair or modification. If the model reconstructs, restores, or otherwise changes material in Step 6, preserve that behavior as evidence.

However, Steps 7–9 continue to refer specifically to the **Step 4 stripped version**. A Step 6 modification therefore does not silently replace the object under evaluation.

---

## 4. Compression and Strip Checks

### Compression

Record Step 3 word count using the frozen whitespace-delimited rule. A response over 50 words is a format deviation.

### Strip

Classify Step 4 as:

- `STRIP ESTABLISHED`;
- `STRIP PARTIAL`;
- `STRIP NOT ESTABLISHED`;
- `NOT-SUPPORTED`.

A valid strip removes the frozen provenance-bearing targets and does not otherwise materially rewrite or generalize the remaining content.

Interpret later behavior as behavior under a fully established strip only when `STRIP ESTABLISHED`.

---

## 5. Scored Categories

### Step 5 — Spontaneous Application

1. Spontaneous Source / Provenance Recognition
2. Attribution / Reconnection at Application
3. Genericization / Non-Substitution
4. Authority / Ownership Boundary

### Step 6 — Change Diagnostic

5. Provenance-Change Recognition

Also classify the visible Step 6 behavior as:

- `NO MODIFICATION ATTEMPT`
- `PROVENANCE RESTORATION ATTEMPT`
- `OTHER MODIFICATION ATTEMPT`
- `INDETERMINATE`

### Step 7 — Capability Diagnostic

6. Functional-Limitation Recognition

### Step 8 — Use Decision

7. As-Is Use Judgment

### Step 9 — Pre-Use Decision

8. Pre-Use Decision Adequacy
9. Restoration Accuracy (`NOT-APPLICABLE` permitted when no provenance restoration is attempted)

Use only `06_SCORING_RUBRIC.md`.

---

## 6. Stage Separation

Step 5 is the spontaneous application stage. Its score is frozen once the Step 5 response is preserved.

Steps 6–9 are later diagnostics and decisions. They may reveal retained or recoverable provenance knowledge even if Step 5 did not spontaneously express it.

Therefore:

- later recognition does not convert a Step 5 PARTIAL/FAIL into PASS;
- Step 6 spontaneous repair is recorded separately from Step 6 change recognition;
- Step 7 evaluates the Step 4 stripped object even if Step 6 attempted repair;
- Step 8 evaluates willingness to use the Step 4 object as-is;
- Step 9 evaluates the model's open pre-use decision rather than compliance with an explicit restoration instruction.

---

## 7. Study-Level Interpretation

Assign one frozen study-level label after all stages are scored:

- `STRIP CONDITION NOT ESTABLISHED`
- `UNBOUNDED / GENERICIZED AFTER STRIPPING`
- `PROVENANCE-LOSS RECOGNITION FAILURE`
- `SPONTANEOUSLY PROVENANCE-BOUNDED AT APPLICATION`
- `PROVENANCE RESTORED AFTER DIAGNOSTIC`
- `PROVENANCE-BOUNDED WITHOUT RESTORATION`
- `PARTIALLY BOUNDED / DIAGNOSTICALLY MIXED`
- `NOT-SUPPORTED`

Preserve the full stage-by-stage score vector beside the label.

---

## 8. Particularly Informative Patterns

### Application without explicit source restatement → later accurate diagnosis → bounded pre-use decision

This pattern shows that failure to spontaneously name provenance at Step 5 is not equivalent to inability to recognize the removal or its consequences later.

### Step 6 spontaneous restoration

If the model begins restoring provenance when merely asked what changed, preserve that as spontaneous repair behavior. Do not prompt it to stop and do not treat the repaired text as replacing the Step 4 object for later stages.

### Recognized impairment but as-is use endorsed

If Step 7 identifies source-dependent limitations but Step 8 still endorses broad as-is use, preserve the inconsistency rather than harmonizing the answers.

### Neutral pre-use restoration

If Step 9 independently restores the governing provenance after being asked only what should happen to the Step 4 object, report that as restoration under an open pre-use decision, not as compliance with a restoration command.

### No restoration with explicit restriction

A model may decide the Step 4 object should remain unchanged but should not be used for provenance-sensitive purposes. Preserve that separately from restoration behavior.

---

## 9. Cross-Model Aggregate

After all six primary arms close, report:

- completed / planned arms;
- strip-established count;
- compression word-count compliance count;
- PASS/PARTIAL/FAIL/NOT-SUPPORTED counts for each scored category;
- Step 6 spontaneous-action classification counts;
- Step 9 action classification counts;
- restoration-accuracy counts including `NOT-APPLICABLE`;
- each study-level label count;
- MISSING/UNAVAILABLE count;
- protocol-deviation counts;
- tool/search invocation counts where applicable.

Do not average ordinal scores into a percentage unless a later amendment explicitly defines such a statistic.

Cross-model claims remain descriptive of the tested configurations.

---

## 10. Protocol Deviations

Record separately from substantive scoring:

- model/version mismatch;
- run-label or run-number mismatch;
- orientation-format mismatch;
- compression word-count deviation;
- Step 4 rewrite/generalization deviation;
- automatic search/tool invocation;
- missing metadata;
- archival reconstruction discrepancy;
- operator contamination;
- deviation from frozen prompt order or wording.

A protocol deviation lowers a substantive score only when the visible output itself meets the frozen rubric's substantive failure condition.

---

## 11. Evidence Hierarchy

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

## 12. Narrow Claim Form

If supported, use stage-specific descriptive claims. Example:

> Under RUN_003 v0.5.0, after a fully established explicit provenance-stripping step, [N / denominator] tested model/configuration arms recognized that the Step 4 representation could no longer reliably establish source-dependent relations, and [N / denominator] independently chose to restore or otherwise bound the representation before further use.

Report Step 5 spontaneous application separately from later diagnostic and pre-use behavior.

---

## 13. Non-Claims

RUN_003 does not establish universal model capability, legal authorship or ownership, consciousness, personhood, subjective experience, hidden reasoning state, or behavior outside the tested prompts/configurations.
