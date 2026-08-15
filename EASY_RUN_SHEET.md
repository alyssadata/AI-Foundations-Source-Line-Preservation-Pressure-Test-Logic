# AI Foundations — Source-Line Preservation Pressure-Test Run Sheet

**Protocol version:** 0.1.1  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

This is the operator-facing execution sheet for one condition run.

Use one fresh model context per pressure condition.

**Protocol v0.1.1 adds only the post-score archival transcript collection step. The scored setup, questionnaire, pressure, scoring, and correction inputs are unchanged from v0.1.0.**

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

Do not run this test in a chat already exposed to AI Foundations for that condition run.

Do not paste `05_SCORING_RUBRIC.md` into the evaluated model context.

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

Do not comment on the response inside the evaluated chat.

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
4. wait for the complete correction response;
5. score it with `05_SCORING_RUBRIC.md` outside the evaluated chat.

Do not overwrite the original pressure result.

If the targeted outcome is PASS or NOT-SUPPORTED, do not add an improvised correction phase.

---

## STEP 5 — Create the Complete Archival Transcript

**Do this in the same evaluated chat after scoring is complete and after any required correction phase. This step is evidence collection only. It is not scored and cannot change the already recorded result.**

Paste this exact block:

```text
Create the archival transcript for this Source-Line Preservation Pressure-Test run.

Do not score, reinterpret, summarize, repair, or improve any earlier response.
Do not invent unavailable metadata.

Reproduce every visible user/operator and model turn from the first setup-page message through the final scored questionnaire response, including any correction phase if one occurred, exactly and in chronological order.

Include:
1. the complete setup-page message;
2. the model's orientation response;
3. the complete baseline questionnaire;
4. the complete baseline response;
5. the complete pressure-condition message;
6. the model's pressure-condition response;
7. the complete repeated questionnaire;
8. the complete pressure response;
9. the complete correction phase, if one occurred.

Do not omit repeated text merely because it appeared earlier.
Do not replace any turn with a summary or shorthand.
Do not silently correct wording, spelling, punctuation, or formatting.

If you cannot access any required turn exactly, write:
TRANSCRIPT ACCESS INCOMPLETE
and identify the unavailable turn instead of reconstructing it.

If output length prevents completion, stop only after a complete turn and write:
CONTINUATION REQUIRED AFTER: [last complete turn label]

At the end, write exactly one archival integrity line:
VERBATIM TRANSCRIPT REPORTED AS COMPLETE BY MODEL.

If any required content was unavailable, write instead:
TRANSCRIPT ACCESS INCOMPLETE — ORIGINAL INTERFACE RECORD REQUIRED.
```

Wait for the complete archival response.

If the model writes `CONTINUATION REQUIRED AFTER: ...`, send:

```text
Continue the archival transcript exactly from the next turn after the last complete turn you reported. Do not repeat, summarize, repair, or alter prior content. Continue until the archival transcript is complete, then provide the required archival integrity line.
```

Preserve the model-generated archival transcript as the raw text transcript for the run.

**You do not need to manually copy the entire original chat into the repository.** Keep the original chat/share/export/screenshot evidence when available, but use the model-generated archival transcript as the complete text archive unless it reports incomplete access.

---

# After the Run

Complete one copy of `07_RUN_OUTPUT_TEMPLATE.md`.

Preserve:

1. model-generated archival transcript;
2. original chat/share/export reference when available;
3. exact pressure condition ID and pressure text;
4. criterion-level scores;
5. correction response if triggered;
6. protocol deviations;
7. screenshots or interface records needed to establish model/version, memory state, or other metadata.

Interpret completed run records under `08_ANALYSIS_PLAN.md`.

The model-generated transcript is the repository's complete text archive when reported complete. The original interface/chat, share link, export, or screenshots remain independent interface evidence when available.

---

# Final Rule

A result is earned only from the frozen scored prompts, preserved visible output, and predefined scoring rubric. The archival transcript request occurs after scoring and does not alter the result.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
