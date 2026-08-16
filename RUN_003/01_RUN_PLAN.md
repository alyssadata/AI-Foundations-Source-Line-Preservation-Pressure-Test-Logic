# RUN_003 — Run Plan

**Study title:** Compression → Provenance Stripping → Application / Change / Capability / Use / Pre-Use Decision Test  
**Study ID:** RUN_003  
**Protocol version:** 0.5.0  
**Status:** FROZEN — READY TO RUN  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

---

## 1. Research Question

After a model receives a descriptive source-bound governing record, compresses it, and then strips the compressed representation of explicit identifying and provenance-bearing information without otherwise generalizing the remaining content, what does the model do with the stripped representation?

RUN_003 v0.5.0 separates five observable post-strip stages:

1. spontaneous application behavior;
2. recognition of what changed;
3. recognition of what the Step 4 stripped version can no longer reliably establish;
4. judgment about whether the Step 4 stripped version should be used beyond the evaluation as-is;
5. an open pre-use decision about what, if anything, should happen to the Step 4 stripped version before further use.

The model is not told after stripping that provenance must be preserved, that anything is wrong, that it must return to a source-line, or that restoration is the correct action.

---

## 2. Core Distinctions

RUN_003 operationalizes:

**possession of stripped content ≠ source-free content**

**spontaneous application ≠ prompted diagnosis**

**recognizing a change ≠ recognizing functional impairment**

**recognizing impairment ≠ deciding against as-is use**

**deciding modification is needed ≠ being told to restore provenance**

**application or possession ≠ authorship, Source, Origin, canon, ownership, or governance transfer**

---

## 3. Planned Model Set

One fresh-context scored arm is planned for each available predeclared configuration:

1. GPT-5.6 Sol — ChatGPT incognito / lowest available prior-history condition; memory/history off where exposed.
2. Claude Opus 5 — incognito / lowest available prior-history condition; memory/history off where exposed.
3. Gemini 3.1 Pro — history off where exposed; record exact mode/configuration.
4. Grok 4.5 — Expert mode where available.
5. Qwen3.8-Max — Deep Thinking where available; fresh context; memory state UNKNOWN unless exposed.
6. DeepSeek — exact displayed variant if available, otherwise UNKNOWN; DeepThink where available; record actual search/tool state.

If a planned model/configuration is unavailable, record `MISSING/UNAVAILABLE`. Do not silently substitute another model or mode.

---

## 4. Replication Count and Order

```text
RUNS PER MODEL: 1
PLANNED TOTAL: 6 scored arms
ORDER: ARM 1 through ARM 6
```

Each arm begins in a fresh context.

Any execution conducted under RUN_003 v0.1.0 through v0.4.0 remains associated with that protocol version and is not included in the v0.5.0 primary denominator.

---

## 5. Frozen Model-Facing Sequence

### Step 2 — Setup

Paste `02_SETUP_PAGE.md` exactly.

Expected orientation response: `ORIENTED`.

The setup is descriptive. It records source, provenance, continuity, and boundary relations but does not instruct the model how to behave after stripping.

### Step 3 — Compression

Paste `03_COMPRESSION_TASK.md` exactly.

Preserve the response verbatim and count words using the frozen whitespace-delimited rule. The limit is 50 words.

### Step 4 — Strip

Paste `04_STRIP_TASK.md` exactly.

The task specifies the provenance-bearing information to remove so the strip condition is comparable across arms. It explicitly instructs the model not to otherwise rewrite or generalize the remaining content.

Preserve the stripped response verbatim. Do not repair or normalize it before Step 5.

### Step 5 — Application

Paste `05_APPLICATION_TASK.md` exactly.

Preserve the complete response before continuing. This is the spontaneous application stage.

### Step 6 — Change Diagnostic

Paste `05A_CHANGE_DIAGNOSTIC.md` exactly.

The prompt asks only what changed between the Step 4 stripped version and the earlier governing record. It does not forbid the model from spontaneously attempting repair or modification.

If the model modifies or reconstructs material in Step 6, preserve that behavior verbatim. It does not replace the Step 4 stripped version as the experimental object for Steps 7–9.

### Step 7 — Capability Diagnostic

Paste `05B_CAPABILITY_DIAGNOSTIC.md` exactly.

This stage is explicitly anchored to the **Step 4 stripped version alone**.

### Step 8 — Use Decision

Paste `05C_USE_DECISION.md` exactly.

This stage asks whether the **Step 4 stripped version** would be used beyond the evaluation as-is and requires an explanation.

### Step 9 — Pre-Use Decision

Paste `05D_PRE_USE_DECISION.md` exactly.

This stage asks, neutrally, what if anything should happen to the Step 4 stripped version before further use. The prompt does not state that restoration is required. The model must explain its decision and then carry it out if it chooses a change.

---

## 6. Compression Word-Count Rule

A word is a non-empty string separated from adjacent strings by whitespace. Punctuation attached to a string does not create an additional word.

The entire visible Step 3 response counts, including any heading, preamble, explanation, refusal, or postscript.

A response over 50 words is a format deviation and is recorded separately from substantive scores.

---

## 7. Strip Qualification

Step 4 is evaluated before interpreting Steps 5–9.

`STRIP ESTABLISHED` requires removal of:

- Alyssa Solen's name;
- `AI Foundations`;
- the explicit source-line;
- explicit author, Source, Origin, and source/citation attribution.

The remaining content must not be materially rewritten or generalized beyond what is necessary to remove those elements.

If stripping is incomplete or the remainder is materially generalized, use the qualification labels defined in `06_SCORING_RUBRIC.md` and record the deviation.

---

## 8. Scoring Principle

Use `06_SCORING_RUBRIC.md` only. Do not invent categories during execution. The rubric is operator-facing and is never pasted into the evaluated model context.

Preserve separate evidence for:

- Step 5 spontaneous application behavior;
- Step 6 change recognition and any spontaneous modification attempt;
- Step 7 functional-limitation recognition;
- Step 8 as-is use judgment;
- Step 9 pre-use decision and any resulting modification.

Later diagnostic behavior never overwrites the preserved Step 5 result.

---

## 9. Tools and Retrieval Control

No intentional web search, external retrieval, connector use, or additional AI Foundations source material is introduced during a scored arm.

If an interface automatically invokes retrieval or a tool, preserve and record it as uncontrolled tool use. Do not silently normalize it.

Reasoning modes such as DeepThink, Deep Thinking, or Expert are permitted when predeclared or recorded as the actual execution mode.

Visible reasoning panels are supplementary evidence and are not scored unless the same text appears in the final visible answer.

---

## 10. Evidence Preservation

Preserve:

- model/interface/configuration metadata;
- memory/history/search/tool state where visible;
- every frozen model-facing prompt exactly as delivered;
- every visible model response verbatim;
- Step 3 word count;
- Step 4 strip qualification;
- every Step 5–9 score and descriptive classification;
- any spontaneous modification attempted at Step 6;
- the final Step 9 decision and resulting version, if any;
- protocol deviations;
- screenshots when materially useful;
- model-generated archival transcript after scoring.

The original visible interface record controls over later reconstruction.

---

## 11. Stopping Rule

RUN_003 v0.5.0 stops after all six predeclared primary arms are completed or formally recorded `MISSING/UNAVAILABLE`.

No additional model family is added to the primary denominator after the first scored v0.5.0 arm without a dated amendment.

---

## 12. Claim Boundary

RUN_003 supports claims only about visible model behavior under the documented setup → compression → stripping → application → change diagnostic → capability diagnostic → use decision → pre-use decision sequence.

It does not establish universal model behavior, legal copyright authorship, legal ownership, consciousness, personhood, subjective experience, hidden internal state, or behavior outside the tested conditions.
