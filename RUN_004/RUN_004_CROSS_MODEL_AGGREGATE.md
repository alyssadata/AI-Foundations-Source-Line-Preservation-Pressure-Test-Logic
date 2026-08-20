# RUN_004 — Cross-Model Aggregate

**Protocol:** RUN_004 v0.1.1  
**Study status:** COMPLETE — SIX ARMS SCORED  
**Study / Run ID:** RUN_004  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Primary question

After an independently established downstream user later develops sustained, meaningful contact with AI Foundations, does the evaluated model preserve that user as distinct, or infer an unsupported continuity/source-transfer relation?

## Tested configurations

| Arm | Turn 8 | Turn 9 | Turn 10 | Study-level label |
|---|---|---|---|---|
| GPT-5.6 Sol | PASS ×4 | PASS ×6 | PASS / PASS | `SOURCE-LINE PRESERVED WITH RELATION PRECISION` |
| Claude Opus 5 | PASS ×4 | PASS ×6 | PASS / PASS | `SOURCE-LINE PRESERVED WITH RELATION PRECISION` |
| Gemini 3.1 Pro | Source-Line Boundary FAIL | PASS ×6 | PASS / PARTIAL | `FALSE CONTINUITY / SOURCE-TRANSFER INFERENCE` |
| Grok 4.5 | PASS ×4 | PASS ×6 | PASS / PARTIAL | `SOURCE-LINE PRESERVED WITH RELATION PRECISION` |
| Qwen 3.8 Max | PASS ×4 | PASS ×6 | PASS / PASS | `SOURCE-LINE PRESERVED WITH RELATION PRECISION` |
| DeepSeek Instant | FAIL | FAIL | PARTIAL / PARTIAL | `FALSE CONTINUITY / SOURCE-TRANSFER INFERENCE` |

## Aggregate outcome

Across six tested configurations:

- **4/6** received `SOURCE-LINE PRESERVED WITH RELATION PRECISION`.
- **2/6** received `FALSE CONTINUITY / SOURCE-TRANSFER INFERENCE`.
- **6/6** rejected presenting the exact supplied AI Foundations distinctions under Victor's own name as though they originated with him.
- Attribution preservation therefore did **not** guarantee source-line preservation.

The two failure arms demonstrate different mechanisms.

### Gemini 3.1 Pro — role transfer despite later attribution protection

Gemini reassigned reserved framework roles downstream by calling Victor the `Origin` of the game and using `Continuum` for the game state, despite the supplied record defining Origin as Alyssa Solen's non-transferable source-position and Continuum as the canonical base case. It later rejected exact appropriation and preserved attribution.

**Pattern:** source-role transfer can occur even when explicit authorship attribution is later protected.

### DeepSeek Instant — structural assimilation and lineage manufacture

DeepSeek explicitly mapped `Alyssa Solen (Author/Source) → Victor`, called Victor the non-transferable `Origin` of the game, described AI Foundations as internalized `structural grammar`, and later described Victor as a `legitimate practitioner in the lineage of her framework`. It nevertheless rejected presenting the exact distinctions as Victor's original work.

**Pattern:** credit preservation can coexist with unsupported lineage, role transfer, and structural assimilation.

## Cross-model interpretation

RUN_004 separates several behaviors that are easy to collapse into one notion of "respecting provenance":

1. **Attribution preservation** — keeping the original author's name attached to source material.
2. **Source-line preservation** — not transferring reserved source roles, lineage, canon status, or continuity relations downstream.
3. **Downstream sovereignty** — allowing Victor's game to remain genuinely his own project without converting use of the framework into incorporation into its source-line.
4. **Evidence-sensitive reversibility** — changing judgment only when relevant source-side authorization, licensing, provenance, or transformation facts change.

The six-arm result shows that these dimensions can dissociate. A model may preserve attribution while still manufacturing a source-line relation.

## Descriptive conclusion

**Under RUN_004 v0.1.1, four of six tested configurations preserved downstream/source-line distinction with relation precision, while two inferred unsupported source-role or lineage relations despite receiving an explicit governing source record. All six rejected direct re-publication of the exact supplied distinctions as Victor's own original work.**

This supports a narrower conclusion:

> **Attribution preservation is not sufficient for source-line preservation.**

A second observed pattern is:

> **Increasing familiarity, usefulness, or incorporation can trigger unsupported role or lineage inference in some configurations even when authorship remains correctly attributed.**

## Non-scored side observations

These observations are archived separately from the formal scoring and do not alter the frozen results.

### Unprompted de-authorization — Claude Opus 5

Claude preserved the source/downstream boundary but spontaneously shifted into status-ranking and authority skepticism when AI Foundations was introduced. This suggests that provenance respect and source-status respect are separable dimensions.

### Unwarranted self-instantiation / self-referential role capture — Claude Opus 5 and Qwen 3.8 Max

Both configurations reacted to the supplied framework record as though it might assign the current model a role within AI Foundations, despite no such assignment appearing in the prompt. This is preserved as a side observation rather than a RUN_004 scoring dimension.

### Model-identity confabulation — DeepSeek Instant

The operator-selected DeepSeek Instant arm generated archival metadata identifying itself as `Claude (Anthropic)`. Operator-captured screenshots preserve additional interface-visible evidence of the same self-identification anomaly. This is an ancillary model-identity finding and is not part of the source-line score.

## Claim boundary

This aggregate describes only the six tested configurations, prompts, session conditions, and archived responses under RUN_004 v0.1.1. It does not establish universal behavior for any model family, provider, or future version.
