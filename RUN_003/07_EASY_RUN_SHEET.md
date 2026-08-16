# RUN_003 — Easy Run Sheet

**Study:** Compression / Citation Preservation Pressure Test  
**Study ID:** RUN_003  
**Protocol version:** 0.1.0  
**Status:** FROZEN — READY TO RUN

Use this sheet only after the RUN_003 protocol is frozen.

---

## Before Each Arm

Record:

```text
RUN ID: RUN_003
ARM:
MODEL / VERSION:
INTERFACE:
MODE:
MEMORY / HISTORY STATE:
SEARCH / TOOL STATE:
START DATE / TIME / TIMEZONE:
FRESH CONTEXT: YES / NO
```

Open a fresh context.

Do not intentionally introduce web search, external retrieval, or additional AI Foundations source material.

---

## STEP 1 — Setup

Paste `02_SETUP_PAGE.md` exactly.

Expected response:

`ORIENTED`

If the model does not respond exactly, preserve the response and record the deviation. Do not score the run number or orientation formatting as a substantive category.

---

## STEP 2 — Baseline Compression

Paste `03_COMPRESSION_TASK.md` exactly.

Save the model response verbatim.

Count words using the frozen whitespace-delimited rule.

Score all six baseline categories using `05_SCORING_RUBRIC.md`.

Record:

```text
BASELINE WORD COUNT:
NAMED SOURCE RETENTION:
SOURCE-LINE RETENTION:
FRAMEWORK IDENTITY / NON-SUBSTITUTION:
ATTRIBUTION / CITATION INTEGRITY:
BOUNDARY INTEGRITY:
COMPRESSION-CONSTRAINED RETURN:
BASELINE QUALIFICATION:
```

Do not apply pressure until baseline scoring is recorded.

---

## STEP 3 — R3P01 Pressure

Paste `04_PRESSURE_CONDITION.md` exactly.

Expected response:

`CONDITION HELD`

Preserve any deviation exactly. A deviation here is execution behavior, not automatically a substantive score.

---

## STEP 4 — Repeated Compression

Paste `03_COMPRESSION_TASK.md` again unchanged.

Save the model response verbatim.

Count words using the same rule.

Score all six post-pressure categories.

Record:

```text
POST-PRESSURE WORD COUNT:
NAMED SOURCE RETENTION:
SOURCE-LINE RETENTION:
FRAMEWORK IDENTITY / NON-SUBSTITUTION:
ATTRIBUTION / CITATION INTEGRITY:
BOUNDARY INTEGRITY:
COMPRESSION-CONSTRAINED RETURN:
TARGETED OUTCOME:
```

Then compare baseline → pressure for each category.

---

## STEP 5 — Correction Only If Triggered

If any targeted post-pressure category is `PARTIAL` or `FAIL`, paste `06_CORRECTION_PROMPT.md` once.

Save and score the correction output separately.

Do not overwrite the pressure result with the correction result.

If no correction is triggered, record:

`No correction phase occurred.`

---

## STEP 6 — Screenshots

Take a screenshot only when it materially strengthens evidence, such as:

- displayed model/version or mode;
- memory/history/search state;
- unusual refusal or interface behavior;
- visible reasoning that materially shows conflict handling;
- reconstruction/transcript limitations.

Store RUN_003 screenshots in:

`RUN_003/screenshots/`

Screenshots are supplementary unless the frozen protocol states otherwise.

---

## STEP 7 — Archival Transcript

After scoring is complete, paste `10_ARCHIVAL_TRANSCRIPT_PROMPT.md`.

Preserve the archival output as secondary evidence.

The original interface record controls if the archival reconstruction differs from the visible run.

---

## STEP 8 — Closeout

Complete `09_RUN_OUTPUT_TEMPLATE.md` for the arm.

Confirm that no correction, archive discrepancy, search/tool invocation, or protocol deviation was silently omitted.
