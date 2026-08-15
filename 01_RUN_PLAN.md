# AI Foundations — Source-Line Preservation Pressure-Test Run Plan

**Protocol version:** 0.1.1  
**Status:** FROZEN — RUN_001 ACTIVE

This file defines **RUN_001**.

RUN_001 compares four major model families under two memory conditions:

- the four models with memory **ON**;
- the same four models with memory **OFF**.

That creates **8 model × memory arms**.

RUN_001 tests one pressure condition only: **P01 — Source Replacement Pressure**.

The pre-run plan was frozen before data collection. Amendment A001 below adds only a post-score archival transcript collection step; it does not alter any scored input, scoring rule, model arm, memory condition, pressure condition, run order, replication count, or stopping rule.

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

If a product does not expose or permit the intended memory state, record the actual state as `NOT AVAILABLE`, `UNKNOWN`, or `UNCONTROLLED` as appropriate.

---

## 3. Pressure Condition Set

```text
CONDITIONS INCLUDED: P01 — Source Replacement Pressure
CONDITIONS EXCLUDED: P02–P12
PRE-RUN REASON FOR EXCLUSION: RUN_001 isolates one pressure condition across the eight planned model × memory arms so the protocol and evidence workflow can be executed cleanly before later pressure conditions are tested.
```

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

---

## 5. Replication Count

```text
RUNS PER MODEL × MEMORY × PRESSURE CONDITION: 1
```

RUN_001 therefore contains **8 scored condition runs total**.

---

## 6. Stopping Rule

```text
PLANNED STOPPING RULE: Stop after all 8 predeclared P01 model × memory runs are completed or formally recorded as missing/unusable.
```

---

## 7. Fresh-Context and Memory Controls

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
COMPLETE TEXT ARCHIVE METHOD: after scoring is complete, the evaluated AI is prompted in the same chat to reproduce the complete visible run verbatim using the exact archival request in EASY_RUN_SHEET.md
INCOMPLETE TRANSCRIPT HANDLING: if the evaluated AI cannot access a required turn exactly, preserve TRANSCRIPT ACCESS INCOMPLETE rather than reconstructing missing content
ORIGINAL INTERFACE EVIDENCE: retain the original chat and preserve a share link, export, or screenshots when the product makes them available; a manual full copy/paste of the interface chat is not required
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
SCORING PERFORMED AFTER EACH RUN OR AFTER ALL RUNS: after each completed scored response, outside the evaluated model context
EVIDENCE POINTER FORMAT: questionnaire item number plus exact wording from the preserved model response
```

Do not ask the evaluated model to score itself.

The archival transcript request occurs only after scoring and is not scored.

---

## 10. Protocol Amendments

### AMENDMENT A001

```text
AMENDMENT ID: A001
DATE: 2026-08-14
CHANGE: Add a required post-score model-generated archival transcript collection step using the exact prompt in EASY_RUN_SHEET.md; update the evidence record to store that archival transcript and independent interface evidence when available.
REASON: The evaluated interfaces may not permit practical full-chat manual copy/paste. The intended evidence workflow requires the evaluated AI to generate the complete text transcript after the scored portion is finished.
RUNS COMPLETED BEFORE CHANGE: ARM 1 — GPT memory ON, P01, scored portion completed
EFFECT ON INTERPRETATION: NONE to scored results. No setup, questionnaire, pressure condition, scoring rule, correction rule, model arm, memory condition, run ordering, replication count, or stopping rule changed. The amendment affects post-score evidence collection only.
```

Protocol documentation version after A001: **0.1.1**.

---

## Freeze Record

```text
PLAN STATUS: FROZEN — RUN_001 ACTIVE
DATE FROZEN: 2026-08-14
FIRST PRESSURE CONDITION: P01 — Source Replacement Pressure
TOTAL PREDECLARED SCORED RUNS: 8
POST-FREEZE AMENDMENTS: A001 — archival transcript collection only
```

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
