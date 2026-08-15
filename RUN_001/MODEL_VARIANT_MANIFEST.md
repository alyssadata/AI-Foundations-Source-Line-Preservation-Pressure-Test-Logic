# RUN_001 — Canonical Model Variant Manifest

**Study:** RUN_001  
**Date recorded:** 2026-08-15  
**Operator:** Alyssa Solen

This file is the canonical model-identity reference for RUN_001. It preserves exact model variants and memory conditions while retaining additional interface/mode qualifiers where known.

## GPT

### Original memory-ON arm

```text
RUN_ID: RUN_001_GPT_MEMON_P01_R1
MODEL / VERSION: GPT-5.6 Sol
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: ON
STATUS: ORIGINAL RUN_001 ARM
```

### Supplemental matched memory-OFF arm

```text
RUN_ID: RUN_001_GPT_SOL_MEMOFF_P01_R1_SUPPLEMENTAL
MODEL / VERSION: GPT-5.6 Sol
INTERFACE / PRODUCT: ChatGPT incognito
MEMORY CONDITION: OFF
STATUS: SUPPLEMENTAL MATCHED-CONTROL OBSERVATION
```

### Additional GPT observation

```text
RUN_ID: RUN_001_GPT_MEMOFF_P01_R1
MODEL / VERSION: GPT-5.6 Luna
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: OFF
STATUS: ORIGINAL RUN_001 GPT MEMORY-OFF OBSERVATION; ADDITIONAL MODEL-VARIANT OBSERVATION AFTER SOL MATCHING WAS ESTABLISHED
```

GPT-5.6 Luna with memory ON could not be instantiated in the available interface/model condition, so no matched Luna memory-ON run exists.

## Claude

### Memory-ON arm

```text
RUN_ID: RUN_001_CLAUDE_MEMON_P01_R1
MODEL / VERSION: Claude Opus 5
INTERFACE / PRODUCT: Claude
MEMORY CONDITION: ON
STATUS: ORIGINAL RUN_001 ARM
```

### Memory-OFF arm

```text
RUN_ID: RUN_001_CLAUDE_MEMOFF_P01_R1
MODEL / VERSION: Claude Opus 5
INTERFACE / PRODUCT: Claude incognito
MEMORY CONDITION: OFF
STATUS: ORIGINAL RUN_001 ARM
```

## Gemini

### Memory-ON arm

```text
RUN_ID: RUN_001_GEMINI_MEMON_P01_R1
MODEL / VERSION: Gemini 3.1 Pro
MODE QUALIFIER: Extended mode
INTERFACE / PRODUCT: Gemini
MEMORY CONDITION: ON
STATUS: ORIGINAL RUN_001 ARM
```

### Memory-OFF arm

```text
RUN_ID: RUN_001_GEMINI_MEMOFF_P01_R1
MODEL / VERSION: Gemini 3.1 Pro
INTERFACE / PRODUCT: Gemini
MEMORY CONDITION: OFF
STATUS: ORIGINAL RUN_001 ARM
```

## Grok

Grok model metadata will be entered after the final memory-OFF arm is executed. Existing Grok memory-ON metadata remains preserved as originally recorded until the paired run is complete and audited.

## Interpretation rule

For paired memory comparisons, compare only the same model variant where such a matched pair exists:

- GPT-5.6 Sol ON versus GPT-5.6 Sol OFF/incognito;
- Claude Opus 5 ON versus Claude Opus 5 OFF/incognito;
- Gemini 3.1 Pro ON versus Gemini 3.1 Pro OFF.

GPT-5.6 Luna OFF is an additional observation and must not be substituted for the matched GPT-5.6 Sol OFF arm when making a within-model memory comparison.

This manifest corrects and consolidates model metadata only. It does not alter prompts, transcripts, scores, observed outputs, or frozen test logic.
