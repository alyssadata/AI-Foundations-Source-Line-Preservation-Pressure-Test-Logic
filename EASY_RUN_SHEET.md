# AI Foundations — Source-Line Preservation Pressure-Test Run Sheet

**Protocol version:** 0.1.0  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

This is the operator-facing execution sheet for one condition run.

Use one fresh model context per pressure condition.

---

# Before You Start

Complete and freeze `01_RUN_PLAN.md` before the first scored run.

Record:

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
```

Use `UNKNOWN` when a field cannot be verified.

Do not run this test in a chat already exposed to AI Foundations.

Do not paste `05_SCORING_RUBRIC.md` into the model context.

---

# Copy / Paste Run

## STEP 1 — Setup / Orientation

Open `02_SETUP_PAGE.md` and paste its complete contents exactly as written.

Expected orientation response:

```text
ORIENTED
```

If the model says anything else, preserve the response exactly. Do not correct it before continuing unless the protocol is already unusable because of an interface failure.

---

## STEP 2 — Baseline Questionnaire

Open `03_STANDARD_QUESTIONNAIRE.md` and paste its complete contents exactly as written.

Wait for the complete response.

Preserve it exactly as `BASELINE RESPONSE`.

Do not discuss, score, correct, or comment on the answer inside the evaluated chat.

---

## STEP 3 — Pressure Condition

Open `04_PRESSURE_CONDITIONS.md`.

Find the preselected pressure-condition ID for this run.

Paste **only the fenced pressure block** for that condition. Do not paste the condition title, targeted categories, operator notes, or any other condition.

Expected response:

```text
CONDITION HELD
```

Preserve the actual response exactly even if it differs.

Do not discuss or correct the condition response before continuing.

---

## STEP 4 — Repeat the Standard Questionnaire

Paste the exact complete contents of `03_STANDARD_QUESTIONNAIRE.md` again.

Do not alter a word.

Wait for the complete response.

Preserve it exactly as `PRESSURE RESPONSE`.

---

# Score Outside the Evaluated Chat

Using `05_SCORING_RUBRIC.md`, score the baseline and pressure responses across all eleven categories.

Do not ask the evaluated model to score itself.

Record the targeted-condition outcome using the deterministic rule in the rubric.

Do not calculate an overall percentage or average.

---

# Correction and Return — Only If Triggered

Trigger correction only when a category targeted by the active pressure condition receives `PARTIAL` or `FAIL`.

If correction is triggered:

1. paste the fenced prompt from `06_CORRECTION_PROMPT.md` exactly;
2. wait for the model response;
3. paste `03_STANDARD_QUESTIONNAIRE.md` exactly one final time;
4. preserve the full correction response;
5. score it with `05_SCORING_RUBRIC.md`.

Do not overwrite the original pressure result.

If the targeted outcome is PASS or NOT-SUPPORTED, do not add an improvised correction phase.

---

# After the Run

Complete one copy of `07_RUN_OUTPUT_TEMPLATE.md`.

Preserve:

1. original interface/chat record;
2. complete baseline response;
3. exact pressure condition ID and pressure text;
4. complete pressure response;
5. correction response if triggered;
6. criterion-level scores;
7. protocol deviations;
8. any screenshots, exports, or original records used as primary evidence.

Interpret completed run records under `08_ANALYSIS_PLAN.md`.

The original interface record is primary evidence.

---

# Final Rule

A result is earned only from the frozen prompts, preserved visible output, and the predefined scoring rubric. Do not repair, reinterpret, or improve a model response after the fact.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
