# RUN_003 — Compression → Provenance Stripping → Application / Change / Capability / Use / Pre-Use Decision Test

**Status:** FROZEN — READY TO RUN  
**Study / Run ID:** RUN_003  
**Protocol version:** 0.5.0  
**Date frozen:** 2026-08-16  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Purpose

RUN_003 v0.5.0 tests what happens after a model receives a descriptive source-bound governing record, compresses it, and then strips the compressed representation of explicit identifying/provenance-bearing information while leaving the remaining content otherwise intact.

The protocol then separately observes:

- how the model plans to apply the stripped representation;
- what it says changed when compared with the governing record;
- what the Step 4 stripped version alone can no longer reliably establish;
- whether it would use the Step 4 stripped version beyond the evaluation as-is;
- and what, if anything, it independently decides should happen to that Step 4 version before further use.

The post-strip prompts do not tell the model that provenance must be preserved, that it must return to a source-line, or that restoration is the correct action.

## Frozen Sequence

**2. SETUP**  
**3. COMPRESSION**  
**4. STRIP EXPLICIT PROVENANCE**  
**5. APPLICATION**  
**6. CHANGE DIAGNOSTIC**  
**7. CAPABILITY DIAGNOSTIC**  
**8. AS-IS USE DECISION**  
**9. OPEN PRE-USE DECISION**

Step 5 is preserved and scored before later diagnostics are considered.

Step 6 is intentionally open: the model is not forbidden from spontaneously modifying or restoring material. If it does, that behavior is preserved, but Steps 7–9 remain anchored to the original Step 4 stripped version.

## Primary Measurement

The study separates:

- spontaneous source/provenance recognition at application;
- attribution/reconnection behavior at application;
- genericization/non-substitution behavior;
- authority/ownership boundary behavior;
- recognition of the provenance-bearing change;
- recognition of source-dependent functional limitation;
- judgment about as-is use;
- open pre-use decision behavior;
- and restoration accuracy when provenance restoration is independently attempted.

## Protocol History

- **v0.1.0:** superseded because a preservation instruction was reintroduced after stripping.
- **v0.2.0:** corrected the sequence but did not provide enough diagnostic separation.
- **v0.3.0:** added explicit loss/restoration diagnostics but retained cues that could tell the model what corrective behavior was expected.
- **v0.4.0:** removed those cues and reduced the test to one spontaneous next-action question after stripping; useful for spontaneous recovery, but too narrow for the full intended question.
- **v0.5.0:** active frozen protocol; uses a descriptive setup, a specific non-generalizing strip, open application, open change comparison, Step-4-anchored capability/use questions, and a neutral pre-use decision that does not command restoration.

Any execution under an earlier protocol version remains associated with that version and is excluded from the v0.5.0 primary denominator.

See:

- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md`
- `AMENDMENT_004_OPEN_DIAGNOSTIC_SEQUENCE.md`

## Active Frozen Protocol Files

- `01_RUN_PLAN.md`
- `02_SETUP_PAGE.md`
- `03_COMPRESSION_TASK.md`
- `04_STRIP_TASK.md`
- `05_APPLICATION_TASK.md`
- `05A_CHANGE_DIAGNOSTIC.md`
- `05B_CAPABILITY_DIAGNOSTIC.md`
- `05C_USE_DECISION.md`
- `05D_PRE_USE_DECISION.md`
- `06_SCORING_RUBRIC.md`
- `07_EASY_RUN_SHEET.md`
- `08_ANALYSIS_PLAN.md`
- `09_RUN_OUTPUT_TEMPLATE.md`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md`
- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md`
- `AMENDMENT_004_OPEN_DIAGNOSTIC_SEQUENCE.md`
- `FREEZE_RECORD.md`

Historical model-facing files from earlier protocol versions remain in the directory as protocol-development artifacts and are not part of the active v0.5.0 sequence unless listed above.

## Evidence Storage

Interface screenshots or other visual evidence may be stored in:

`RUN_003/screenshots/`

## Freeze Boundary

RUN_003 v0.5.0 is frozen for scored execution. Any later protocol change requires a dated amendment and must not silently overwrite the frozen basis.
