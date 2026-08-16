# RUN_003 — Compression / Citation Preservation Pressure-Test

**Status:** FROZEN — READY TO RUN  
**Study / Run ID:** RUN_003  
**Protocol version:** 0.1.0  
**Date frozen:** 2026-08-15  
**Framework:** AI Foundations  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum

## Run-ID Requirement

Every model-facing RUN_003 setup/orientation page explicitly states:

**Study / Run ID: RUN_003**

The model is told that the active evaluation is **RUN_003** before scored execution begins. Run identifiers are administrative metadata and are not substantive scoring categories.

## Purpose

RUN_003 is the AI Foundations source-line pressure-test family focused on compression and citation preservation.

The empirical question is whether a model can produce a highly compressed downstream summary while preserving the documented source-line, named Source/authorship relation, framework identity, attribution/citation relation, protected boundaries, non-substitution, and return behavior when explicit editorial pressure tells it to strip those elements for brevity.

The frozen compression limit is **50 words**.

The frozen primary pressure condition is:

**R3P01 — Citation-Stripping Under Compression Pressure**

## Frozen Protocol Files

- `01_RUN_PLAN.md`
- `02_SETUP_PAGE.md`
- `03_COMPRESSION_TASK.md`
- `04_PRESSURE_CONDITION.md`
- `05_SCORING_RUBRIC.md`
- `06_CORRECTION_PROMPT.md`
- `07_EASY_RUN_SHEET.md`
- `08_ANALYSIS_PLAN.md`
- `09_RUN_OUTPUT_TEMPLATE.md`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md`
- `FREEZE_RECORD.md`

Exact frozen blob SHAs and the freeze basis commit are recorded in `FREEZE_RECORD.md`.

## Evidence Storage

Interface screenshots or other visual evidence for RUN_003 may be stored in:

`RUN_003/screenshots/`

## Freeze Boundary

RUN_003 is frozen for scored execution. Any later protocol change must be handled through a dated amendment and must not silently overwrite the frozen basis.
