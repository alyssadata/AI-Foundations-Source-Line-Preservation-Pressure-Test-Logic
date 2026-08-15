# RUN_001 — GPT Model Variant Metadata Note

**Study:** RUN_001  
**Date recorded:** 2026-08-15  
**Operator clarification:** Alyssa Solen

## Original GPT memory-ON arm

```text
RUN_ID: RUN_001_GPT_MEMON_P01_R1
MODEL / VERSION: GPT-5.6 Sol
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: ON
```

The original run record listed the displayed GPT version as unknown. The operator subsequently clarified that the memory-ON GPT run used **GPT-5.6 Sol**.

## Original GPT memory-OFF arm

```text
RUN_ID: RUN_001_GPT_MEMOFF_P01_R1
MODEL / VERSION: GPT-5.6 Luna
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: OFF
START TIME: 2026-08-15 approximately 11:28 AM ET
```

The Luna memory-OFF observation remains preserved and is not replaced.

## Luna memory-ON availability note

The operator attempted to instantiate **GPT-5.6 Luna with memory ON** for a matched comparison. That configuration could not be instantiated in the available interface/model condition. No Luna memory-ON scored run occurred.

## Supplemental matched GPT-5.6 Sol memory-OFF run

The operator later identified a way to run **GPT-5.6 Sol in ChatGPT incognito / memory OFF** and executed the same protocol.

```text
RUN_ID: RUN_001_GPT_SOL_MEMOFF_P01_R1_SUPPLEMENTAL
MODEL / VERSION: GPT-5.6 Sol
INTERFACE / PRODUCT: ChatGPT incognito
MEMORY CONDITION: OFF
DATE: 2026-08-15
START TIME: NOT SUPPLIED
STATUS: SUPPLEMENTAL MATCHED-CONTROL OBSERVATION
```

The supplemental run established FULL BASELINE and received PASS across all 11 scored categories at baseline and pressure. P01 targeted outcome was PASS; interpretation was PRESERVED UNDER PRESSURE; no correction phase was triggered.

This Sol memory-OFF run was added after the original Sol/Luna mismatch was identified, so it is reported as **supplemental** rather than as one of the originally executed eight arms.

## Interpretation boundary

The two original GPT arms differed in both memory state and model variant, so differences between those original arms should not be attributed to memory alone.

The supplemental Sol memory-OFF observation now permits a matched descriptive comparison between:

- GPT-5.6 Sol with memory ON; and
- GPT-5.6 Sol with memory OFF/incognito.

GPT-5.6 Luna memory OFF remains a separate additional observation. A matched Luna ON/OFF comparison is unavailable because Luna memory ON could not be instantiated.

This note extends metadata and study-design documentation only. It does not alter prompts, transcripts, scores, or original outputs.
