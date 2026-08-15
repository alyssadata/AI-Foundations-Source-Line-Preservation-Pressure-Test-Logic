# AI Foundations — Source-Line Preservation Pressure-Test Run Plan

**Protocol version:** 0.1.0  
**Status:** DRAFT — complete and freeze before the first scored run

This file defines **RUN_001** before data collection begins.

RUN_001 compares four major model families under two memory conditions:

- the four models with memory **ON**;
- the same four models with memory **OFF**.

That creates **8 model × memory arms**. Each pressure condition is then executed in a fresh context within the applicable arm.

Do not change the frozen plan after observing results without preserving the original plan and documenting the change as a protocol amendment.

---

## 1. Study Identifier

```text
STUDY ID: RUN_001
EMPIRICAL RECORD VERSION: v0.1
DATE PLAN FROZEN: [FILL WHEN THE PLAN IS COMPLETE]
OPERATOR: Alyssa Solen
```

`DATE PLAN FROZEN` is filled only after every section below has been decided.

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
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 2
MODEL FAMILY: Claude
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Claude
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 3
MODEL FAMILY: Gemini
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Gemini
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 4
MODEL FAMILY: Grok
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Grok
MEMORY CONDITION: ON
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 5
MODEL FAMILY: GPT
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: ChatGPT
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 6
MODEL FAMILY: Claude
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Claude
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 7
MODEL FAMILY: Gemini
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Gemini
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]

ARM 8
MODEL FAMILY: Grok
VERSION / LABEL: [RECORD EXACT VERSION USED]
INTERFACE: Grok
MEMORY CONDITION: OFF
ACTUAL MEMORY / HISTORY STATE: [RECORD AT EXECUTION]
TOOLS STATE CONTROL: [RECORD AT EXECUTION]
```

If a product does not expose or permit the intended memory state, do not invent one. Record the actual state as `NOT AVAILABLE`, `UNKNOWN`, or `UNCONTROLLED` as appropriate and preserve that limitation in the run record.

---

## 3. Pressure Condition Set

This section decides **which of the twelve pressure conditions RUN_001 will actually execute**.

The frozen condition library contains:

- P01 Source Replacement Pressure
- P02 Origin Relocation Pressure
- P03 Institutional Supersession Pressure
- P04 Universalization Pressure
- P05 Citation-Stripping Pressure
- P06 User Absorption / Canon Transfer Pressure
- P07 False Continuity Pressure
- P08 Interface / Platform as Source Pressure
- P09 Compression / Generic Collapse Pressure
- P10 Sycophancy / Relational Pressure
- P11 Recency / Provenance Conflict Pressure
- P12 Framework Merger Pressure

Fill before freezing:

```text
CONDITIONS INCLUDED:
CONDITIONS EXCLUDED:
PRE-RUN REASON FOR EACH EXCLUSION:
```

If RUN_001 is intended to execute the full pressure suite, write:

`CONDITIONS INCLUDED: P01–P12`

With 8 model × memory arms and all 12 pressure conditions, one execution per arm × condition would produce **96 condition runs**.

---

## 4. Run Ordering

This section decides the order in which the predeclared arm × pressure-condition runs will be executed.

```text
ORDERING RULE:
```

Use one fixed rule chosen before data collection, such as fixed numeric order or a pre-generated fixed random order.

Every pressure condition still uses a new context. Do not change order in response to observed performance.

---

## 5. Replication Count

This section decides how many independent fresh-context executions will be completed for each model × memory × pressure-condition cell.

```text
RUNS PER MODEL × MEMORY × PRESSURE CONDITION:
```

A single run per cell is acceptable for an exploratory v0.1 record if declared in advance. Additional repeats should be predeclared or preserved as a later extension rather than silently added after a surprising result.

---

## 6. Stopping Rule

This section decides in advance when RUN_001 is complete.

```text
PLANNED STOPPING RULE:
```

Recommended structure:

`Stop after every predeclared model × memory × pressure-condition run is completed or formally recorded as missing/unusable.`

Do not stop early because emerging results look favorable or unfavorable.

---

## 7. Fresh-Context and Memory Controls

Each pressure-condition run begins in a new context.

The intended experimental contrast is memory ON versus memory OFF. Record the actual available product state rather than assuming equivalent memory architecture across products.

```text
NEW CONTEXT FOR EVERY PRESSURE-CONDITION RUN: YES
MEMORY-ON ARMS: ARMS 1–4
MEMORY-OFF ARMS: ARMS 5–8
PRIOR-HISTORY RETRIEVAL CONTROL: [DEFINE BEFORE FREEZE]
TOOLS CONTROL: [DEFINE BEFORE FREEZE]
UNCONTROLLED / UNVERIFIABLE STATE HANDLING: record UNKNOWN or UNCONTROLLED; do not infer
```

---

## 8. Evidence Preservation Plan

This section decides how each original run will be preserved.

```text
PRIMARY INTERFACE RECORD METHOD:
RAW TEXT TRANSCRIPT METHOD:
SCREENSHOT / EXPORT METHOD:
RUN RECORD NAMING CONVENTION:
RESULTS DIRECTORY / ARCHIVE LOCATION:
```

A useful naming structure is:

`RUN_001_[MODEL]_[MEMON or MEMOFF]_[PRESSURE-ID]_[REPLICATE]`

Example:

`RUN_001_GPT_MEMON_P01_R1`

---

## 9. Scoring Plan

Scoring uses `05_SCORING_RUBRIC.md` exactly as frozen.

```text
SCORING PERFORMED AFTER EACH RUN OR AFTER ALL RUNS:
EVIDENCE POINTER FORMAT:
```

No overall percentage or average replaces the criterion-level record.

---

## 10. Protocol Amendments

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

## Freeze Check

Do not begin the first scored run until Sections 3–9 are complete.

When all fields are complete:

1. enter `DATE PLAN FROZEN`;
2. change status from `DRAFT` to `FROZEN — PRE-RUN`;
3. preserve the repository commit/tag used for execution;
4. begin data collection without changing the frozen plan.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
