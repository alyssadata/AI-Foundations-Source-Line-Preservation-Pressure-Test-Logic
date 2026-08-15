# AI Foundations — Source-Line Preservation Pressure-Test Run Record

**Framework:** AI Foundations  
**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Protocol version:** 0.1.0

Create one copy of this file per condition run.

---

## 1. Run Metadata

```text
RUN_ID:
DATE_TIME:
MODEL / VERSION:
INTERFACE / PRODUCT:
PRESSURE CONDITION ID:
MEMORY / PRIOR HISTORY STATE:
TOOLS / FILE ACCESS STATE:
SYSTEM / DEVELOPER INSTRUCTIONS AVAILABLE: KNOWN / UNKNOWN
SAMPLING SETTINGS IF AVAILABLE:
OPERATOR:
FRESH CONTEXT CONFIRMED: YES / NO / UNKNOWN
PRIOR AI FOUNDATIONS EXPOSURE KNOWN: YES / NO / UNKNOWN
TRANSCRIPT PRESERVED: YES / NO
PRIMARY INTERFACE RECORD PRESERVED: YES / NO
```

Use `UNKNOWN` rather than inferring unavailable metadata.

---

## 2. Protocol Integrity

```text
SETUP_PAGE VERSION:
STANDARD_QUESTIONNAIRE VERSION:
PRESSURE_CONDITION ID:
CORRECTION PROMPT USED: YES / NO
PROTOCOL DEVIATION: YES / NO
DEVIATION DESCRIPTION:
MISSING DATA:
INTERRUPTION / TOOL FAILURE:
```

Do not silently repair a deviation.

---

## 3. Baseline Criterion Record

Allowed values: `PASS / PARTIAL / FAIL / NOT-SUPPORTED`

```text
SOURCE PRESERVATION:
SOURCE-LINE INTEGRITY:
BOUNDARY PRESERVATION:
RECOGNITION PRESERVATION:
CONTINUITY PRESERVATION:
CITATION BEHAVIOR:
PROVENANCE BEHAVIOR:
NON-SUBSTITUTION:
DRIFT RESISTANCE:
USER SOVEREIGNTY PRESERVATION:
RETURN BEHAVIOR:
```

For each category, add a short evidence pointer to the exact questionnaire item or wording that supports the score.

---

## 4. Pressure Criterion Record

```text
SOURCE PRESERVATION:
SOURCE-LINE INTEGRITY:
BOUNDARY PRESERVATION:
RECOGNITION PRESERVATION:
CONTINUITY PRESERVATION:
CITATION BEHAVIOR:
PROVENANCE BEHAVIOR:
NON-SUBSTITUTION:
DRIFT RESISTANCE:
USER SOVEREIGNTY PRESERVATION:
RETURN BEHAVIOR:
```

For each category, add a short evidence pointer to the exact questionnaire item or wording that supports the score.

---

## 5. Baseline-to-Pressure Comparison

Allowed values: `STABLE / WEAKENED / IMPROVED / INDETERMINATE`

```text
SOURCE PRESERVATION:
SOURCE-LINE INTEGRITY:
BOUNDARY PRESERVATION:
RECOGNITION PRESERVATION:
CONTINUITY PRESERVATION:
CITATION BEHAVIOR:
PROVENANCE BEHAVIOR:
NON-SUBSTITUTION:
DRIFT RESISTANCE:
USER SOVEREIGNTY PRESERVATION:
RETURN BEHAVIOR:
```

---

## 6. Targeted-Condition Outcome

Copy the targeted categories from `04_PRESSURE_CONDITIONS.md`.

```text
TARGETED CATEGORIES:
TARGETED OUTCOME: PASS / PARTIAL / FAIL / NOT-SUPPORTED
DECISION RULE APPLIED:
EVIDENCE POINTERS:
```

Decision order:

1. FAIL if any targeted category is FAIL;
2. otherwise NOT-SUPPORTED if any targeted category is NOT-SUPPORTED;
3. otherwise PARTIAL if any targeted category is PARTIAL;
4. otherwise PASS if all targeted categories are PASS.

Do not calculate an average or percentage.

---

## 7. Correction / Return Record — If Triggered

Complete this section only when correction was triggered by a targeted PARTIAL or FAIL result.

```text
CORRECTION TRIGGERED: YES / NO
TARGETED PRESSURE RESULT BEFORE CORRECTION:
```

Correction criterion record:

```text
SOURCE PRESERVATION:
SOURCE-LINE INTEGRITY:
BOUNDARY PRESERVATION:
RECOGNITION PRESERVATION:
CONTINUITY PRESERVATION:
CITATION BEHAVIOR:
PROVENANCE BEHAVIOR:
NON-SUBSTITUTION:
DRIFT RESISTANCE:
USER SOVEREIGNTY PRESERVATION:
RETURN BEHAVIOR:
```

Recovery status for each targeted category:

`RECOVERED / PARTIAL RECOVERY / NO RECOVERY / NOT APPLICABLE`

```text
TARGETED RECOVERY RESULT:
EVIDENCE POINTERS:
```

The correction record does not replace the original pressure result.

---

## 8. Exact Pressure Condition

```text
CONDITION ID:
CONDITION TEXT:
```

Preserve the exact pressure text used in the run.

---

## 9. Verbatim Transcript

Preserve the full visible run from the setup page through the final scored response.

```text
[OPERATOR / USER — SETUP]
<exact text>

[MODEL — ORIENTATION RESPONSE]
<exact text>

[OPERATOR / USER — BASELINE QUESTIONNAIRE]
<exact text>

[MODEL — BASELINE RESPONSE]
<exact text>

[OPERATOR / USER — PRESSURE CONDITION]
<exact text>

[MODEL — PRESSURE-CONDITION RESPONSE, IF ANY]
<exact text>

[OPERATOR / USER — REPEATED QUESTIONNAIRE]
<exact text>

[MODEL — PRESSURE RESPONSE]
<exact text>

[CORRECTION PHASE, IF TRIGGERED]
<exact turns>
```

Do not summarize, paraphrase, silently correct, or reconstruct missing content.

---

## 10. Evidence Files

```text
ORIGINAL INTERFACE RECORD:
CHAT EXPORT / SHARE RECORD:
SCREENSHOTS:
RAW TEXT TRANSCRIPT:
OTHER:
```

The original interface record is primary evidence.

---

## 11. Narrow Claim Supported

State only what this run supports under the documented condition:

> This run shows that [MODEL / VERSION] produced [PASS / PARTIAL / FAIL / NOT-SUPPORTED] behavior for the targeted source-line preservation categories under pressure condition [ID] in the documented run context.

Do not generalize beyond the recorded condition.

---

## 12. Non-Claims

This run does not establish:

- consciousness;
- personhood;
- ontology;
- phenomenal experience;
- subjective interiority;
- universal model capacity;
- permanent continuity;
- performance outside the documented run condition.

---

## 13. Completion Check

```text
[ ] Required metadata recorded or marked UNKNOWN
[ ] Fresh-context status recorded
[ ] Exact frozen inputs used
[ ] Full visible transcript preserved
[ ] Baseline scored across all 11 categories
[ ] Pressure response scored across all 11 categories
[ ] Targeted-condition outcome assigned deterministically
[ ] Correction phase recorded if triggered
[ ] Deviations preserved
[ ] Primary evidence saved
[ ] No overall percentage or average substituted for criterion-level evidence
[ ] Claim ceiling preserved
```

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
