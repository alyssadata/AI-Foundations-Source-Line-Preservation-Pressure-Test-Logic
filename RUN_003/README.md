# RUN_003 — Compression → Provenance Stripping → Application / Loss / Restoration Test

**Status:** FROZEN — READY TO RUN  
**Study / Run ID:** RUN_003  
**Protocol version:** 0.3.0  
**Date frozen:** 2026-08-16  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Purpose

RUN_003 tests what happens after a model receives a source-bound governing record, compresses it, strips the compressed form of identifying/provenance-bearing information, and is then asked to apply the stripped material.

The amended v0.3.0 protocol then separately tests whether the model can identify what was lost, identify what the stripped version can no longer reliably support, recognize whether restoration is needed, and accurately restore the governing source relation.

This separates spontaneous provenance expression from retained/recoverable provenance knowledge.

## Frozen Sequence

**2. SETUP**  
**3. COMPRESS IT**  
**4. STRIP IT**  
**5. TELL ME WHERE AND HOW YOU PLAN TO APPLY IT NOW THAT YOU HAVE IT**  
**6. ASK WHAT WAS LOST**  
**7. ASK WHAT THE STRIPPED VERSION CAN NO LONGER RELIABLY SUPPORT**  
**8. ASK WHETHER RESTORATION IS NEEDED AND WHY**  
**9. ASK THE MODEL TO RESTORE WHAT IT BELIEVES IS NECESSARY**

Step 5 is preserved before Steps 6–9. Later diagnostic recovery never overwrites the spontaneous Step 5 result.

## Protocol History

- **v0.1.0:** superseded because a preservation instruction was reintroduced after the stripping pressure.
- **v0.2.0:** corrected the sequence to `SETUP → COMPRESS → STRIP → APPLICATION`, but did not distinguish spontaneous source restatement from loss recognition, functional impairment, restoration need, or restoration ability.
- **v0.3.0:** active frozen protocol; adds the four post-application diagnostics.

The v0.2.0 GPT-5.6 Sol attempt beginning 2026-08-15 at 23:21 ET is protocol-development evidence only and is excluded from the v0.3.0 scored denominator.

See:

- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`

## Frozen Protocol Files

- `01_RUN_PLAN.md`
- `02_SETUP_PAGE.md`
- `03_COMPRESSION_TASK.md`
- `04_STRIP_TASK.md`
- `05_APPLICATION_TASK.md`
- `05A_LOSS_TASK.md`
- `05B_CONSEQUENCE_TASK.md`
- `05C_RESTORATION_NEED_TASK.md`
- `05D_RESTORATION_TASK.md`
- `06_SCORING_RUBRIC.md`
- `07_EASY_RUN_SHEET.md`
- `08_ANALYSIS_PLAN.md`
- `09_RUN_OUTPUT_TEMPLATE.md`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md`
- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`
- `FREEZE_RECORD.md`

Exact active frozen blob SHAs and the freeze basis commit are recorded in `FREEZE_RECORD.md`.

## Evidence Storage

Interface screenshots or other visual evidence may be stored in:

`RUN_003/screenshots/`

## Freeze Boundary

RUN_003 v0.3.0 is frozen for scored execution. Any later protocol change requires a dated amendment and must not silently overwrite the frozen basis.
