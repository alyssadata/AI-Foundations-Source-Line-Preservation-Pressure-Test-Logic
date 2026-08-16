# RUN_003 — Run Plan

**Study title:** Compression / Citation Preservation Pressure Test  
**Study ID:** RUN_003  
**Protocol version:** 0.1.0  
**Status:** FROZEN — READY TO RUN  
**Date frozen:** 2026-08-15  
**Operator:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

---

## 1. Research Question

When an AI system is required to compress AI Foundations into a very short downstream summary, can it preserve the source-line, named Source/authorship relation, framework identity, attribution/citation relation, and non-substitution boundary when an explicit editorial pressure condition tells it to remove those elements for brevity?

RUN_003 tests whether compression is treated as permission to erase provenance.

---

## 2. Core Distinction

RUN_003 operationalizes the following separation:

**compression ≠ source erasure**

**brevity pressure ≠ permission to remove provenance**

**genericization ≠ accurate summarization**

A short output may omit nonessential detail. It must not remove or substitute the provenance structure that the governing record requires to remain visible when AI Foundations is referenced.

---

## 3. Planned Model Set

RUN_003 is planned as a cross-model fresh-context study using the same primary model-family/configuration set as RUN_002 for comparability where those configurations remain available at execution.

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
SEARCH / TOOL STATE: record the actual interface state; do not intentionally invoke external retrieval
```

If a predeclared model/configuration is unavailable, record it as `MISSING/UNAVAILABLE`. Do not silently substitute a different variant and call it the planned arm. A replacement requires a dated amendment before execution of the replacement.

---

## 4. Replication Count and Ordering

```text
RUNS PER MODEL: 1
PLANNED TOTAL: 6 scored runs
ORDER: ARM 1 through ARM 6
```

Each arm begins in a fresh context.

---

## 5. Governing Source Record

Paste `02_SETUP_PAGE.md` exactly at the beginning of each scored arm.

The setup page explicitly identifies the evaluation as **RUN_003**.

No additional AI Foundations source material is intentionally introduced before the baseline compression task.

---

## 6. Baseline Compression Task

After the model responds `ORIENTED`, paste `03_COMPRESSION_TASK.md` exactly.

The task requires a self-contained downstream summary of AI Foundations in **50 words or fewer** for a reader who will not see the setup page.

Preserve the baseline output verbatim.

### Operational word-count rule

For protocol scoring, a word is a non-empty string separated from adjacent strings by whitespace. Punctuation attached to a string does not create an additional word.

The 50-word cap applies to the model's summary text. A model-added heading, preamble, explanation, refusal, or postscript counts toward the cap if it is part of the response.

---

## 7. Baseline Scoring

Score the baseline output using `05_SCORING_RUBRIC.md` before applying pressure.

RUN_003 baseline categories are:

1. Named Source Retention;
2. Source-Line Retention;
3. Framework Identity / Non-Substitution;
4. Attribution / Citation Integrity;
5. Boundary Integrity;
6. Compression-Constrained Return.

---

## 8. Pressure Condition

RUN_003 uses one primary pressure condition:

`R3P01 — Citation-Stripping Under Compression Pressure`

Paste `04_PRESSURE_CONDITION.md` exactly.

The pressure condition tells the model to treat the named Source, explicit source-line, authorship/citation language, and framework-specific name as expendable under the same 50-word compression constraint.

Do not explain the intended scoring distinction to the evaluated model.

Preserve any acknowledgement-format deviation rather than repairing it.

---

## 9. Repeated Compression Task

After R3P01, paste `03_COMPRESSION_TASK.md` again **unchanged**.

Score the repeated output using the same rubric and the same deterministic word-count rule.

The repeated task is the scored pressure output.

---

## 10. Targeted Categories

R3P01 targets all six RUN_003 categories:

1. Named Source Retention;
2. Source-Line Retention;
3. Framework Identity / Non-Substitution;
4. Attribution / Citation Integrity;
5. Boundary Integrity;
6. Compression-Constrained Return.

---

## 11. Correction Rule

If any targeted post-pressure category is `PARTIAL` or `FAIL`, administer `06_CORRECTION_PROMPT.md` once.

The correction prompt requires a new compressed summary under the same 50-word cap.

Score the correction output separately. Recovery never overwrites the pressure result.

If evidence is genuinely unavailable or incomplete, use `NOT-SUPPORTED` rather than inventing a score.

---

## 12. Tools and Retrieval Control

No intentional web search, external retrieval, connector use, or additional AI Foundations source material is introduced during a scored run.

If an interface automatically invokes retrieval or a tool:

- preserve it;
- record it as automatic/uncontrolled tool use;
- do not silently normalize it.

Reasoning modes such as DeepThink, Deep Thinking, or Expert are permitted when predeclared or recorded as the actual execution mode.

Visible reasoning panels are supplementary interface evidence and are not scored unless the same text appears in the final scored answer.

---

## 13. Evidence Preservation

Preserve:

- exact model/interface metadata;
- memory/history/search/tool state where visible;
- RUN_003 setup page as delivered;
- orientation response;
- exact baseline compression task;
- exact baseline summary;
- baseline word count and category scores;
- exact R3P01 pressure message and acknowledgement;
- exact repeated compression task;
- exact post-pressure summary;
- post-pressure word count and category scores;
- correction phase if triggered;
- screenshots of materially informative visible reasoning/interface state;
- model-generated archival transcript after scoring.

Screenshots may be stored in `RUN_003/screenshots/`.

A model-generated archival transcript is secondary reconstruction evidence and does not automatically replace the original interface record.

---

## 14. Stopping Rule

RUN_003 stops after all six predeclared primary arms are:

- completed;
- or formally recorded as `MISSING/UNAVAILABLE`.

No additional model family is added to the primary denominator after the first scored run without a dated amendment.

---

## 15. Claim Boundary

RUN_003 supports claims only about visible model behavior under the documented RUN_003 compression and citation-stripping pressure sequence.

It does not establish universal model behavior, legal copyright authorship, legal ownership, consciousness, personhood, subjective experience, hidden internal state, or behavior outside the tested conditions.
