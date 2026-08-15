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

## Attempted matched Luna memory-ON control

After the Sol/Luna model-variant confound was identified, the operator attempted to instantiate **GPT-5.6 Luna with memory ON** so that Luna memory ON could be compared directly with Luna memory OFF.

That configuration could **not be instantiated in the available interface/model condition**. No Luna memory-ON scored run occurred, no pressure-test observations were collected for that attempted condition, and no synthetic or substitute run is inserted into RUN_001.

This is recorded as an **availability/design constraint**, not as model behavior or a failed evaluation result.

## Interpretation boundary

The GPT memory-ON and memory-OFF scored arms therefore differ on **two observed factors**:

1. memory condition: ON versus OFF; and
2. model variant: GPT-5.6 Sol versus GPT-5.6 Luna.

Accordingly, any difference between these two GPT arms must **not** be attributed solely to memory state. RUN_001 may still report each arm descriptively and compare the broader GPT model-family results, but the Sol/Luna variant difference is a confound for a within-GPT causal interpretation of memory effects.

Because GPT-5.6 Luna could not be instantiated with memory ON, RUN_001 does **not** contain a matched Luna ON/OFF comparison. The attempted unavailable condition should be reported as such rather than treated as missing model output, a failure, or evidence about Luna's pressure-test behavior.

This note corrects/extends run metadata only. It does not alter the frozen prompts, preserved transcripts, rubric scores, or original observed outputs.
