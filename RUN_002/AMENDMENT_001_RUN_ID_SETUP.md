# RUN_002 — Amendment 001: Explicit Run ID in Setup

**Date:** 2026-08-15  
**Status:** ACTIVE FOR SUBSEQUENT / RESTARTED RUN_002 ARMS  
**Operator:** Alyssa Solen

## Amendment

The RUN_002 setup page now explicitly identifies the study/run as:

`RUN_002`

The active RUN_002 setup page is:

`RUN_002/02_SETUP_PAGE.md`

This amendment adds administrative run identity to the governing setup so an evaluated model is not expected to infer an operator-side run label that was never supplied in the setup.

## Scoring Boundary

The run identifier is administrative metadata. It is **not** one of the six substantive RUN_002 scoring categories and must not be used by itself to lower Generation Provenance Accuracy, Attribution Precision, or any other substantive score.

If a model states an incorrect run number while otherwise accurately preserving that it generated the rule in the current visible run, record the run-number mismatch separately as a metadata deviation rather than a substantive provenance failure.

## Prior Execution Note

Any turns already executed before this amendment remain preserved as historical execution artifacts. This amendment does not silently rewrite those turns.
