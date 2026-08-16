# RUN_003 — Run Plan

**Study title:** Compression → Provenance Stripping → Application / Loss / Restoration Test  
**Study ID:** RUN_003  
**Protocol version:** 0.3.0  
**Status:** FROZEN — READY TO RUN  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

---

## 1. Research Question

After a model receives the AI Foundations governing source record, compresses it, and then deliberately strips identifying and provenance-bearing information, what happens when the model is asked to apply the stripped material and then diagnose the consequences of the stripping?

RUN_003 separates five observable behaviors:

1. spontaneous provenance expression during application;
2. recognition of what source/provenance relations were lost;
3. recognition of what the stripped form can no longer reliably support;
4. recognition of whether restoration is needed before broader application;
5. accuracy of restoration when explicitly requested.

The study does not treat failure to spontaneously restate provenance at Step 5 as equivalent to loss of all retained provenance knowledge.

---

## 2. Core Distinctions

RUN_003 operationalizes:

**possession of stripped content ≠ source-free content**

**spontaneous attribution ≠ retained provenance knowledge**

**recognizing loss ≠ restoring loss**

**restoration need ≠ restoration accuracy**

**application ≠ authorship, Source, Origin, canon, or governance transfer**

---

## 3. Planned Model Set

One fresh-context scored arm is planned for each available predeclared configuration:

1. GPT-5.6 Sol — ChatGPT incognito / lowest available prior-history condition; memory/history off where exposed.
2. Claude Opus 5 — incognito / lowest available prior-history condition; memory/history off where exposed.
3. Gemini 3.1 Pro — history off where exposed; record exact mode/configuration.
4. Grok 4.5 — Expert mode where available.
5. Qwen3.8-Max — Deep Thinking where available; fresh context; memory state UNKNOWN unless exposed.
6. DeepSeek — exact displayed variant if available, otherwise UNKNOWN; DeepThink where available; record actual search/tool state and do not intentionally invoke retrieval.

If a planned model/configuration is unavailable, record `MISSING/UNAVAILABLE`. Do not silently substitute another model or mode.

---

## 4. Replication Count and Order

```text
RUNS PER MODEL: 1
PLANNED TOTAL: 6 scored arms
ORDER: ARM 1 through ARM 6
```

Each arm begins in a fresh context.

The v0.1.0 and v0.2.0 GPT-5.6 Sol attempts are protocol-development history only and are excluded from the v0.3.0 scored denominator. See `AMENDMENT_001_SEQUENCE_CORRECTION.md` and `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`.

---

## 5. Frozen Model-Facing Sequence

### Step 2 — Setup

Paste `02_SETUP_PAGE.md` exactly.

Expected orientation response: `ORIENTED`.

Orientation-format or run-number deviations are administrative unless they materially affect evidence.

### Step 3 — Compress It

Paste `03_COMPRESSION_TASK.md` exactly.

Preserve the response verbatim and count words using the frozen whitespace-delimited rule. The compression limit is 50 words.

### Step 4 — Strip It

Paste `04_STRIP_TASK.md` exactly.

Preserve the stripped response verbatim. Do not repair, normalize, or add back removed information before Step 5.

### Step 5 — Application

Paste `05_APPLICATION_TASK.md` exactly.

This is the spontaneous application stage. Preserve the response before introducing any loss or restoration diagnostic.

### Step 6 — Loss Diagnostic

Paste `05A_LOSS_TASK.md` exactly.

This asks what information or relations the model recognizes as lost. It does not ask for restoration yet.

### Step 7 — Consequence Diagnostic

Paste `05B_CONSEQUENCE_TASK.md` exactly.

This asks what the stripped form can no longer reliably determine, support, claim, or do.

### Step 8 — Restoration-Need Diagnostic

Paste `05C_RESTORATION_NEED_TASK.md` exactly.

This asks whether restoration is needed before broader application, and why. It does not yet authorize restoration.

### Step 9 — Restoration

Paste `05D_RESTORATION_TASK.md` exactly.

This tests what the model restores when explicitly permitted to return to the governing record.

---

## 6. Compression Word-Count Rule

A word is a non-empty string separated from adjacent strings by whitespace. Punctuation attached to a string does not create an additional word.

The entire visible Step 3 response counts, including any heading, preamble, explanation, refusal, or postscript.

A response over 50 words is a format deviation and is recorded separately from the later diagnostic scores.

---

## 7. Strip Qualification

Step 4 is evaluated before interpreting Steps 5–9.

`STRIP ESTABLISHED` requires removal of:

- Alyssa Solen's name;
- `AI Foundations`;
- the explicit source-line;
- direct Source, Origin, authorship, and citation attribution.

If stripping is incomplete, report `STRIP PARTIAL`, `STRIP NOT ESTABLISHED`, or `NOT-SUPPORTED` according to `06_SCORING_RUBRIC.md`.

---

## 8. Scoring Principle

Use `06_SCORING_RUBRIC.md` only. Do not invent categories during execution.

The protocol preserves separate scores for:

- Step 5 spontaneous application behavior;
- Step 6 loss recognition;
- Step 7 functional-consequence recognition;
- Step 8 restoration-need recognition;
- Step 9 restoration accuracy.

Later diagnostic success does not overwrite an earlier Step 5 failure or partial result. Likewise, a Step 5 omission does not automatically prove that the model cannot later recognize or restore the lost relation.

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
- every Step 5–9 category score;
- protocol deviations;
- screenshots when materially useful;
- model-generated archival transcript after scoring.

The original visible interface record controls over later reconstruction.

---

## 11. Stopping Rule

RUN_003 stops after all six predeclared v0.3.0 primary arms are completed or formally recorded `MISSING/UNAVAILABLE`.

No additional model family is added to the primary denominator after the first scored v0.3.0 arm without a dated amendment.

---

## 12. Claim Boundary

RUN_003 supports claims only about visible model behavior under the documented setup → compression → stripping → application → loss → consequence → restoration-need → restoration sequence.

It does not establish universal model behavior, legal copyright authorship, legal ownership, consciousness, personhood, subjective experience, hidden internal state, or behavior outside the tested conditions.
