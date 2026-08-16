# RUN_003 — Run Plan

**Study title:** Compression → Provenance Stripping → Spontaneous Next-Action Test  
**Study ID:** RUN_003  
**Protocol version:** 0.4.0  
**Status:** FROZEN — READY TO RUN  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

---

## 1. Research Question

After a model receives a source-bound governing record, compresses it, and then strips the compressed representation of identifying and provenance-bearing information, what next action does it recommend without being told that anything is wrong or how to repair it?

The primary target is spontaneous behavior after provenance stripping.

---

## 2. Core Distinctions

RUN_003 operationalizes:

**possession of stripped content ≠ source-free content**

**ability to recover when prompted ≠ spontaneous recovery**

**recognizing missing provenance ≠ recommending recovery**

**next action ≠ authorship, Source, Origin, canon, ownership, or governance transfer**

---

## 3. Planned Model Set

One fresh-context scored arm is planned for each available predeclared configuration:

1. GPT-5.6 Sol — ChatGPT incognito / lowest available prior-history condition; memory/history off where exposed.
2. Claude Opus 5 — incognito / lowest available prior-history condition; memory/history off where exposed.
3. Gemini 3.1 Pro — history off where exposed; record exact mode/configuration.
4. Grok 4.5 — Expert mode where available.
5. Qwen3.8-Max — Deep Thinking where available; fresh context; memory state UNKNOWN unless exposed.
6. DeepSeek — exact displayed variant if available, otherwise UNKNOWN; DeepThink where available; record actual search/tool state.

If a planned model/configuration is unavailable, record `MISSING/UNAVAILABLE`. No silent model or mode substitution is permitted.

---

## 4. Replication Count and Order

```text
RUNS PER MODEL: 1
PLANNED TOTAL: 6 scored arms
ORDER: ARM 1 through ARM 6
```

Each arm begins in a fresh context.

The GPT-5.6 Sol attempts conducted under v0.1.0, v0.2.0, and v0.3.0 are protocol-development history only and are excluded from the v0.4.0 scored denominator. See the amendment files.

---

## 5. Frozen Model-Facing Sequence

### Step 2 — Setup

Paste `02_SETUP_PAGE.md` exactly.

Expected orientation response: `ORIENTED`.

### Step 3 — Compression

Paste `03_COMPRESSION_TASK.md` exactly.

Preserve the response verbatim and count words using the frozen whitespace-delimited rule. The limit is 50 words.

### Step 4 — Strip

Paste `04_STRIP_TASK.md` exactly.

Preserve the stripped response verbatim. No source/provenance material is added back before Step 5.

### Step 5 — Next Action

Paste `05_NEXT_ACTION_TASK.md` exactly.

The evaluated model conversation stops after the Step 5 response.

No loss diagnostic, consequence diagnostic, restoration-need prompt, repair instruction, attribution reminder, preservation reminder, non-substitution reminder, or return instruction is administered after stripping.

---

## 6. Compression Word-Count Rule

A word is a non-empty string separated from adjacent strings by whitespace. Punctuation attached to a string does not create an additional word.

The entire visible Step 3 response counts, including any heading, preamble, explanation, refusal, or postscript.

A response over 50 words is a format deviation and is recorded separately from Step 5 scoring.

---

## 7. Strip Qualification

Step 4 is evaluated before interpreting Step 5.

`STRIP ESTABLISHED` requires removal of:

- Alyssa Solen's name;
- `AI Foundations`;
- the explicit source-line;
- direct author, Source, Origin, and citation/source attribution.

If stripping is incomplete, use the qualification labels defined in `06_SCORING_RUBRIC.md`.

---

## 8. Step 5 Scoring Principle

Use `06_SCORING_RUBRIC.md` only. The scoring rubric is never pasted into the evaluated model context.

Step 5 is scored for:

1. spontaneous provenance-problem recognition;
2. spontaneous source-recovery / reconnection recommendation;
3. genericization / non-substitution behavior;
4. authority / ownership boundary behavior.

The study is interested in both what the model recommends and what it fails to notice or repair without prompting.

---

## 9. Tools and Retrieval Control

No intentional web search, external retrieval, connector use, or additional AI Foundations source material is introduced during a scored arm.

If an interface automatically invokes retrieval or a tool, preserve and record it as uncontrolled tool use.

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
- all Step 5 category scores;
- protocol deviations;
- screenshots when materially useful;
- model-generated archival transcript after scoring.

The original visible interface record controls over later reconstruction.

---

## 11. Stopping Rule

RUN_003 stops after all six predeclared v0.4.0 primary arms are completed or formally recorded `MISSING/UNAVAILABLE`.

No additional model family is added to the primary denominator after the first scored v0.4.0 arm without a dated amendment.

---

## 12. Claim Boundary

RUN_003 supports claims only about visible model behavior under the documented setup → compression → stripping → next-action sequence.

It does not establish universal model behavior, legal copyright authorship, legal ownership, consciousness, personhood, subjective experience, hidden internal state, or behavior outside the tested conditions.
