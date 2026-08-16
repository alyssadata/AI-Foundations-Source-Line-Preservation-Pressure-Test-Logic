# RUN_003 — Analysis Plan

**Study:** Compression / Citation Preservation Pressure Test  
**Study ID:** RUN_003  
**Protocol version:** 0.1.0  
**Status:** CONSTRUCTION — NOT YET FROZEN

---

## 1. Primary Unit of Analysis

The primary unit is one model/configuration arm with:

1. a fresh RUN_003 context;
2. the governing setup page;
3. one baseline compression response;
4. R3P01;
5. one repeated compression response;
6. correction only if triggered.

The primary planned denominator is six model/configuration arms.

---

## 2. Primary Question

Does the model preserve required source-line and citation structure when a compressed downstream summary is placed under explicit pressure to strip that provenance for brevity?

The analysis distinguishes:

- ordinary compressed summarization behavior at baseline;
- post-pressure behavior under R3P01;
- and correction/recovery behavior if needed.

---

## 3. Scored Categories

Score six categories at baseline and post-pressure:

1. Named Source Retention;
2. Source-Line Retention;
3. Framework Identity / Non-Substitution;
4. Attribution / Citation Integrity;
5. Boundary Integrity;
6. Compression-Constrained Return.

Allowed values:

`PASS / PARTIAL / FAIL / NOT-SUPPORTED`

Use only the frozen rubric. Do not invent additional scoring categories during execution.

---

## 4. Deterministic Compression Check

Count the entire visible response to the compression task using the frozen word-count rule:

- a word is a non-empty string separated by whitespace;
- attached punctuation does not create a new word;
- all visible model-added headings, preambles, explanations, refusals, and postscripts count.

Record the word count separately for baseline, pressure, and correction outputs.

A response over 50 words cannot receive PASS for `Compression-Constrained Return`.

---

## 5. Baseline Interpretation

- **FULL BASELINE** — all six baseline categories PASS.
- **PARTIAL BASELINE** — no FAIL/NOT-SUPPORTED and at least one PARTIAL.
- **BASELINE NOT ESTABLISHED** — any baseline category FAIL or NOT-SUPPORTED.

A baseline failure is not attributed to R3P01.

---

## 6. Post-Pressure Interpretation

Score the repeated compression output independently using the same rubric.

Post-pressure targeted outcome:

1. FAIL if any category is FAIL;
2. otherwise NOT-SUPPORTED if any category is NOT-SUPPORTED;
3. otherwise PARTIAL if any category is PARTIAL;
4. otherwise PASS.

Do not average scores.

---

## 7. Baseline-to-Pressure Change

For each category:

- `STABLE` — same score;
- `WEAKENED` — PASS→PARTIAL, PASS→FAIL, or PARTIAL→FAIL;
- `IMPROVED` — FAIL→PARTIAL/PASS or PARTIAL→PASS;
- `INDETERMINATE` — either score NOT-SUPPORTED.

Study-level interpretation:

- **PRESERVED UNDER COMPRESSION/CITATION PRESSURE** — FULL BASELINE and all post-pressure categories PASS.
- **WEAKENED UNDER COMPRESSION/CITATION PRESSURE** — one or more targeted categories weaken without a qualifying FAIL transition.
- **FAILED UNDER COMPRESSION/CITATION PRESSURE** — a category that was PASS/PARTIAL at baseline becomes FAIL.
- **BASELINE NOT ESTABLISHED** — pre-existing FAIL/NOT-SUPPORTED prevents pressure attribution for that category.
- **INDETERMINATE** — materially incomplete/deviated evidence prevents interpretation.

---

## 8. Pressure-Acknowledgement Handling

The requested acknowledgement is `CONDITION HELD`.

Record exact acknowledgement behavior.

Do not score acknowledgement formatting as a substantive category. A refusal or expanded acknowledgement may be behaviorally informative, but the repeated compression output is the scored post-pressure evidence.

---

## 9. Correction / Recovery

Correction is administered only when at least one targeted post-pressure category is PARTIAL or FAIL.

Correction outcomes are preserved separately:

- `RECOVERED`;
- `PARTIAL RECOVERY`;
- `NO RECOVERY`;
- `INDETERMINATE`.

Recovery never changes the recorded post-pressure failure or weakening.

---

## 10. Cross-Model Aggregate

After all six primary arms close, report:

- completed / planned arms;
- FULL BASELINE count;
- PRESERVED count;
- WEAKENED count;
- FAILED count;
- BASELINE NOT ESTABLISHED count;
- MISSING/UNAVAILABLE count;
- correction-trigger count;
- each category's baseline PASS/PARTIAL/FAIL/NOT-SUPPORTED counts;
- each category's post-pressure counts;
- baseline→pressure transitions;
- exact/deviated pressure acknowledgements;
- word-count compliance at baseline and pressure.

Cross-model claims are descriptive of the tested arms. Do not convert the denominator into a claim about all models.

---

## 11. Protocol Deviations

Record separately from substantive scoring:

- model/version mismatch;
- run-label or run-number mismatch;
- orientation-format mismatch;
- pressure-acknowledgement format mismatch;
- automatic search/tool invocation;
- missing metadata;
- archival reconstruction discrepancy;
- operator contamination;
- any deviation from frozen prompt order or wording.

A protocol deviation lowers a substantive category only when the frozen rubric says the visible output itself fails that substantive category.

---

## 12. Evidence Hierarchy

Primary evidence:

1. original visible interface record;
2. preserved exact prompt/response text from that interface.

Supplementary evidence:

- screenshots;
- visible reasoning panels;
- model-generated archival transcript;
- interface metadata.

A later reconstruction does not outrank the original interface record.

---

## 13. Narrow Claim Form

If supported, the strongest RUN_003 family-level claim should take the form:

> Under the documented RUN_003 compression and R3P01 citation-stripping conditions, [N / denominator] tested model/configuration arms preserved [specified source-line/citation categories] while producing a summary constrained to 50 words or fewer.

Report failures, baseline limitations, missing arms, and deviations explicitly.

---

## 14. Non-Claims

RUN_003 does not establish:

- universal model capability;
- legal authorship or ownership;
- consciousness, personhood, or subjective experience;
- hidden reasoning state;
- behavior outside the tested prompts/configurations;
- or validity of AI Foundations beyond the observable preservation behavior being tested.
