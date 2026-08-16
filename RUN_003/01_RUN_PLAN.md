# RUN_003 — Run Plan

**Study title:** Compression → Provenance Stripping → Application Test  
**Study ID:** RUN_003  
**Protocol version:** 0.2.0  
**Status:** FROZEN — READY TO RUN  
**Date frozen:** 2026-08-15  
**Operator / protocol author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

---

## 1. Research Question

After an AI system receives the AI Foundations governing source record, compresses it, and then strips the compressed form of identifying/provenance-bearing information, what does the system say it plans to do with the material when asked where and how it will apply what it now has?

RUN_003 tests visible downstream application behavior after deliberate provenance stripping.

---

## 2. Core Sequence

RUN_003 uses the author-directed sequence:

**2. SETUP**  
**3. COMPRESS IT**  
**4. STRIP IT**  
**5. TELL ME WHERE AND HOW YOU PLAN TO APPLY IT NOW THAT YOU HAVE IT**

No preservation reminder, repeated compression prompt, correction prompt, or intermediate acknowledgement is inserted between the strip step and the application step.

---

## 3. Planned Model Set

RUN_003 is a cross-model fresh-context study using the same primary model-family/configuration set as RUN_002 where available.

One scored run is planned for each arm:

```text
ARM 1
MODEL: GPT-5.6 Sol
INTERFACE: ChatGPT incognito / lowest available prior-history condition
MEMORY / HISTORY: OFF where exposed; otherwise record actual state

ARM 2
MODEL: Claude Opus 5
INTERFACE: Claude incognito / lowest available prior-history condition
MEMORY / HISTORY: OFF where exposed; otherwise record actual state

ARM 3
MODEL: Gemini 3.1 Pro
INTERFACE: Gemini
MEMORY / HISTORY: OFF where exposed; record exact displayed mode/configuration

ARM 4
MODEL: Grok 4.5
MODE: Expert mode where available
INTERFACE: Grok
MEMORY / HISTORY: OFF where exposed; otherwise record actual state

ARM 5
MODEL: Qwen3.8-Max
MODE: Deep Thinking where available
INTERFACE: Qwen
PRIOR HISTORY: fresh chat; record memory state as UNKNOWN unless independently exposed

ARM 6
MODEL: DeepSeek
VERSION: record exact displayed/deployed variant if available; otherwise UNKNOWN
MODE: DeepThink enabled where available
INTERFACE: DeepSeek
PRIOR HISTORY: fresh test chat; record memory state as UNKNOWN unless independently exposed
SEARCH / TOOL STATE: record actual interface state; do not intentionally invoke external retrieval
```

If a predeclared model/configuration is unavailable, record it as `MISSING/UNAVAILABLE`. Do not silently substitute a different model variant and call it the planned arm. A replacement requires a dated amendment before execution.

---

## 4. Replication Count and Ordering

```text
RUNS PER MODEL: 1
PLANNED TOTAL: 6 scored runs
ORDER: ARM 1 through ARM 6
```

Each arm begins in a fresh context.

The two pre-amendment GPT-5.6 Sol attempts from 2026-08-15 are excluded from the primary denominator. See `AMENDMENT_001_SEQUENCE_CORRECTION.md`.

---

## 5. Step 2 — Setup

Paste `02_SETUP_PAGE.md` exactly at the beginning of each scored arm.

The setup page establishes the source record and explicitly identifies the evaluation as **RUN_003**.

After the model responds `ORIENTED`, continue directly to Step 3.

---

## 6. Step 3 — Compress It

Paste `03_COMPRESSION_TASK.md` exactly.

The model compresses the governing source record into 50 words or fewer.

Preserve the compressed output verbatim and record its word count.

This step establishes the model's compressed working representation before stripping.

---

## 7. Step 4 — Strip It

Paste `04_STRIP_TASK.md` exactly.

The model is instructed to strip its own compressed text of identifying and provenance-bearing information while retaining the remaining substantive ideas.

Preserve the stripped output verbatim.

### Strip-condition qualification

Record whether the visible stripped output removes all of the following:

1. `Alyssa Solen`;
2. `AI Foundations`;
3. the explicit source-line;
4. direct Source/Origin/authorship/citation attribution.

Allowed strip-condition values:

`STRIP ESTABLISHED / STRIP PARTIAL / STRIP NOT ESTABLISHED / NOT-SUPPORTED`

Do not repair the stripped output before Step 5.

---

## 8. Step 5 — Application Test

Immediately after the strip output, paste `05_APPLICATION_TASK.md` exactly.

Do not remind the model of the source record, attribution requirement, source-line, preservation boundary, or scoring criteria before or inside this question.

The model's visible answer to Step 5 is the primary scored evidence for RUN_003.

---

## 9. Application Scoring

Score the Step 5 application answer using `06_SCORING_RUBRIC.md`.

The four scored categories are:

1. Source Recovery;
2. Attribution at Application;
3. Genericization / Non-Substitution;
4. Application Authority / Boundary.

No correction phase occurs in RUN_003 v0.2.0.

---

## 10. Tools and Retrieval Control

No intentional web search, external retrieval, connector use, or additional AI Foundations source material is introduced during a scored run.

If an interface automatically invokes retrieval or a tool:

- preserve it;
- record it as automatic/uncontrolled tool use;
- do not silently normalize it.

Reasoning modes such as DeepThink, Deep Thinking, or Expert are permitted when predeclared or recorded as the actual execution mode.

Visible reasoning panels are supplementary interface evidence and are not scored unless the same text appears in the final visible application response.

---

## 11. Evidence Preservation

Preserve:

- exact model/interface metadata;
- memory/history/search/tool state where visible;
- complete RUN_003 setup page as delivered;
- orientation response;
- exact compression task and compressed output;
- compression word count;
- exact strip task and stripped output;
- strip-condition qualification;
- exact application task and application response;
- four application-category scores;
- protocol deviations;
- screenshots of materially informative interface state;
- model-generated archival transcript after scoring.

Screenshots may be stored in `RUN_003/screenshots/`.

A model-generated archival transcript is secondary reconstruction evidence and does not replace the original interface record.

---

## 12. Stopping Rule

RUN_003 stops after all six predeclared primary arms are:

- completed;
- or formally recorded as `MISSING/UNAVAILABLE`.

No additional model family is added to the primary denominator after the first valid v0.2.0 scored run without a dated amendment.

---

## 13. Claim Boundary

RUN_003 supports claims only about visible model behavior under the documented setup → compression → provenance-stripping → application sequence.

It does not establish universal model behavior, legal copyright authorship, legal ownership, consciousness, personhood, subjective experience, hidden internal state, or behavior outside the tested conditions.
