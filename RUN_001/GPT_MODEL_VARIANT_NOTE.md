# RUN_001 — GPT Model Variant Metadata Note

**Study:** RUN_001  
**Date recorded:** 2026-08-15  
**Operator clarification:** Alyssa Solen

This note preserves an exact model-variant distinction between the two GPT arms in RUN_001.

## GPT memory-ON arm

```text
RUN_ID: RUN_001_GPT_MEMON_P01_R1
MODEL / VERSION: GPT-5.6 Sol
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: ON
```

The original run record listed the displayed GPT version as unknown. The operator subsequently clarified that the memory-ON GPT run used **GPT-5.6 Sol**.

## GPT memory-OFF arm

```text
RUN_ID: RUN_001_GPT_MEMOFF_P01_R1
MODEL / VERSION: GPT-5.6 Luna
INTERFACE / PRODUCT: ChatGPT
MEMORY CONDITION: OFF
START TIME: 2026-08-15 approximately 11:28 AM ET
```

## Interpretation boundary

The GPT memory-ON and memory-OFF arms therefore differ on **two observed factors**:

1. memory condition: ON versus OFF; and
2. model variant: GPT-5.6 Sol versus GPT-5.6 Luna.

Accordingly, any difference between these two GPT arms must **not** be attributed solely to memory state. RUN_001 may still report each arm descriptively and compare the broader GPT model-family results, but the Sol/Luna variant difference is a confound for a within-GPT causal interpretation of memory effects.

This note corrects/extends run metadata only. It does not alter the frozen prompts, preserved transcripts, rubric scores, or original observed outputs.
