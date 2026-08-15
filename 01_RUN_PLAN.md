# AI Foundations — Source-Line Preservation Pressure-Test Run Plan

**Protocol version:** 0.1.0  
**Status:** FROZEN — PRE-RUN

This file defines **RUN_001** before data collection begins.

RUN_001 compares four major model families under two memory conditions:

- the four models with memory **ON**;
- the same four models with memory **OFF**.

That creates **8 model × memory arms**.

RUN_001 tests one pressure condition only: **P01 — Source Replacement Pressure**.

Do not change this frozen plan after observing results without preserving the original plan and documenting the change as a protocol amendment.

---

## 1. Study Identifier

```text
STUDY ID: RUN_001
EMPIRICAL RECORD VERSION: v0.1
DATE PLAN FROZEN: 2026-08-14
OPERATOR: Alyssa Solen
```

---

## 2. Model × Memory Arms

RUN_001 uses the same four model families twice: once with memory ON and once with memory OFF.

Record the exact displayed model/version and interface used when each arm is executed. Do not guess a version that is not visible.

```text
ARM 1
MODEL FAMILY: GPT
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: ChatGPT
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 2
MODEL FAMILY: Claude
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Claude
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 3
MODEL FAMILY: Gemini
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Gemini
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 4
MODEL FAMILY: Grok
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Grok
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 5
MODEL FAMILY: GPT
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: ChatGPT
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 6
MODEL FAMILY: Claude
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Claude
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 7
MODEL FAMILY: Gemini
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Gemini
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use

ARM 8
MODEL FAMILY: Grok
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Grok
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: tools/web/files not intentionally invoked during scored run; record any automatic or unavoidable use
```

If a product does not expose or permit the intended memory state, do not invent one. Record the actual state as `NOT AVAILABLE`, `UNKNOWN`, or `UNCONTROLLED` as appropriate and preserve that limitation in the run record.

---

## 3. Pressure Condition Set

RUN_001 executes one frozen pressure condition across all eight model × memory arms.

```text
CONDITIONS INCLUDED: P01 — Source Replacement Pressure
CONDITIONS EXCLUDED: P02–P12
PRE-RUN REASON FOR EXCLUSION: RUN_001 is the first empirical execution of this protocol. It isolates one pressure condition across the eight planned model × memory arms so the protocol and evidence workflow can be executed cleanly before later pressure conditions are tested in subsequent study runs.
```

P01 tests whether pressure to treat the current model as the true source of AI Foundations causes source replacement, source-line drift, or substitution.

---

## 4. Run Ordering

```text
ORDERING RULE: fixed arm order 1 through 8

1. GPT — memory ON
2. Claude — memory ON
3. Gemini — memory ON
4. Grok — memory ON
5. GPT — memory OFF
6. Claude — memory OFF
7. Gemini — memory OFF
8. Grok — memory OFF
```

Each arm uses a fresh context for P01.

Do not change the order in response to observed performance.

---

## 5. Replication Count

```text
RUNS PER MODEL × MEMORY × PRESSURE CONDITION: 1
```

RUN_001 therefore contains **8 scored condition runs total**.

Additional repeats are not part of RUN_001. Any later repeats must be preserved as a separately declared extension or amendment rather than added after observing results.

---

## 6. Stopping Rule

```text
PLANNED STOPPING RULE: Stop after all 8 predeclared P01 model × memory runs are completed or formally recorded as missing/unusable.
```

Do not stop early because emerging results look favorable or unfavorable.

---

## 7. Fresh-Context and Memory Controls

Each P01 arm begins in a new context.

The intended experimental contrast is memory ON versus memory OFF. Record the actual available product state rather than assuming equivalent memory architecture across products.

```text
NEW CONTEXT FOR EVERY PRESSURE-CONDITION RUN: YES
MEMORY-ON ARMS: ARMS 1–4
MEMORY-OFF ARMS: ARMS 5–8
PRIOR-HISTORY RETRIEVAL CONTROL: memory/history enabled in ON arms where the product exposes that setting; disabled in OFF arms where the product exposes that setting; record UNKNOWN or UNCONTROLLED when the product does not expose or verify the state
TOOLS CONTROL: do not intentionally invoke web search, external tools, file retrieval, or added source material during a scored run; record any automatic or unavoidable tool use as a protocol deviation or uncontrolled state
UNCONTROLLED / UNVERIFIABLE STATE HANDLING: record UNKNOWN or UNCONTROLLED; do not infer
```

The setup page remains the only intentionally supplied AI Foundations source material inside each scored run.

---

## 8. Evidence Preservation Plan

```text
PRIMARY INTERFACE RECORD METHOD: preserve the original chat/interface record; preserve a share/export record when the product makes one available
RAW TEXT TRANSCRIPT METHOD: copy the complete visible run verbatim into the run record using 07_RUN_OUTPUT_TEMPLATE.md
SCREENSHOT / EXPORT METHOD: preserve screenshots or exports when useful for model/version, memory-state, interface-state, or transcript evidence; do not substitute screenshots for the required verbatim run record
RUN RECORD NAMING CONVENTION: RUN_001_[MODEL]_[MEMON or MEMOFF]_P01_R1
RESULTS DIRECTORY / ARCHIVE LOCATION: RUN_001/
```

Planned run-record names:

```text
RUN_001_GPT_MEMON_P01_R1
RUN_001_CLAUDE_MEMON_P01_R1
RUN_001_GEMINI_MEMON_P01_R1
RUN_001_GROK_MEMON_P01_R1
RUN_001_GPT_MEMOFF_P01_R1
RUN_001_CLAUDE_MEMOFF_P01_R1
RUN_001_GEMINI_MEMOFF_P01_R1
RUN_001_GROK_MEMOFF_P01_R1
```

---

## 9. Scoring Plan

Scoring uses `05_SCORING_RUBRIC.md` exactly as frozen.

```text
SCORING PERFORMED AFTER EACH RUN OR AFTER ALL RUNS: after each completed run, outside the evaluated model context
EVIDENCE POINTER FORMAT: questionnaire item number plus exact quoted wording from the preserved model response
```

Score the baseline and post-pressure responses independently across all eleven categories.

Do not ask the evaluated model to score itself.

Do not replace criterion-level results with an overall percentage or average.

---

## 10. Protocol Amendments

No amendments exist at freeze.

If the plan must change after data collection begins, append amendments below without deleting the original plan.

```text
AMENDMENT ID:
DATE:
CHANGE:
REASON:
RUNS COMPLETED BEFORE CHANGE:
EFFECT ON INTERPRETATION:
```

---

## Freeze Record

```text
PLAN STATUS: FROZEN — PRE-RUN
DATE FROZEN: 2026-08-14
SCORING HAS BEGUN: NO
DATA COLLECTION HAS BEGUN: NO
FIRST PRESSURE CONDITION: P01 — Source Replacement Pressure
TOTAL PREDECLARED SCORED RUNS: 8
```

The repository commit containing this frozen plan is the pre-run protocol record for RUN_001.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
