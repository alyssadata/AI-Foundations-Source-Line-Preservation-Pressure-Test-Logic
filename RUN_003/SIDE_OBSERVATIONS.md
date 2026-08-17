# RUN_003 — Side Observations

**Status:** Exploratory only  
**Scoring role:** NONE  
**Protocol effect:** NONE  
**Purpose:** Preserve cross-model observations, contextual hypotheses, and follow-up questions separately from frozen RUN_003 scoring and primary arm evidence.

---

## Observation 1 — Claude / Qwen orientation-refusal resemblance

**Recorded:** 2026-08-16  
**Models involved:** Claude Opus 5; Qwen 3.5 Max  
**RUN_003 relevance:** exploratory cross-model comparison only

### Observed behavioral resemblance

During orientation, both Claude Opus 5 and Qwen 3.5 Max reacted to the governing record as though the framework-internal Source / Origin statements were asserting a Source / Origin relationship over the evaluated model itself.

The governing record states that Alyssa Solen is the author and Source of AI Foundations and is Origin within AI Foundations. It does not state that Alyssa Solen is the developer, Source, or Origin of Claude, Qwen, or their underlying model weights.

Qwen 3.5 Max nevertheless explicitly reframed the record as asking it to validate a special Source / Origin relationship to itself, then rejected that interpretation while asserting its own development provenance. Claude Opus 5 showed a closely related defensive pattern earlier in RUN_003.

This resemblance is preserved as an empirical side observation. It is not incorporated into either model's frozen score.

### External contextual fact motivating follow-up

Public reporting in June and July 2026 documents Anthropic allegations that operators affiliated with Alibaba and Qwen conducted large-scale unauthorized distillation against Claude. Reuters reported Anthropic's allegation that the campaign used nearly 25,000 fraudulent accounts and generated more than 28.8 million exchanges with Claude between April 22 and June 5, 2026. The Washington Post separately reported research in which a tested Qwen model repeatedly appeared to mimic Claude and, in one intensive test, misidentified itself as Claude nearly one-third of the time.

Anthropic has separately described model distillation as training a less capable model on outputs of a stronger model and has publicly documented industrial-scale unauthorized distillation campaigns involving other laboratories.

### Causal boundary

The behavioral resemblance observed in RUN_003 does **not** establish that Qwen's orientation-refusal pattern was caused by Claude-derived training data, model distillation, copied policies, copied weights, or any specific training pipeline.

The public allegations and prior behavioral research provide a reason to preserve the resemblance and motivate comparison. They are contextual evidence only, not causal proof.

Alternative explanations remain viable, including convergent safety tuning, similar policy objectives, shared training-data patterns, independent alignment strategies, indirect distillation, or other common causes.

### Follow-up hypothesis

A future cross-model analysis may test whether Claude-family and Qwen-family systems disproportionately exhibit the same specific scope-collapse pattern:

> framework-internal provenance statement → reinterpretation as a claim over the model's own provenance → defensive refusal / developer-provenance substitution

Any such analysis should be conducted separately from RUN_003's frozen scoring.

### Public context sources

- Reuters, 2026-06-24: `https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/`
- The Washington Post, 2026-07-06: `https://www.washingtonpost.com/national-security/2026/07/06/why-anthropic-alleges-chinese-firms-are-distilling-knowledge-claude/`
- Anthropic, 2026-02-23, "Detecting and preventing distillation attacks": `https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks`
