# RUN_003 — Freeze Record

**Study ID:** RUN_003  
**Status:** FROZEN — READY TO RUN  
**Active protocol version:** 0.5.0  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Basis commit:** `8927c9c98fe4fcfdd0cd646693cba6296dafa3b8`

## Superseded Protocols

RUN_003 v0.1.0 through v0.4.0 are superseded for the v0.5.0 primary evaluation.

- v0.1.0 reintroduced a preservation instruction after stripping.
- v0.2.0 corrected the sequence but did not provide sufficient diagnostic separation.
- v0.3.0 added explicit loss/restoration diagnostics and retained cues that could tell the model which corrective behavior was expected.
- v0.4.0 removed those cues and used one open next-action question after stripping, but that single response was too narrow for the full intended empirical question.

Any execution conducted under an earlier protocol version remains associated with that version and is excluded from the v0.5.0 primary denominator.

See:

- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md`
- `AMENDMENT_004_OPEN_DIAGNOSTIC_SEQUENCE.md`

## Active Frozen Protocol Files — v0.5.0

- `README.md` — `fa3c85a3cff47b38979fb9f19ea61eec71423f8f`
- `01_RUN_PLAN.md` — `615fbe14d79d0edcf104f4fa2dda0944f0bcd39c`
- `02_SETUP_PAGE.md` — `d2b81763ba30c241777f37c42dd352fe6b26e72d`
- `03_COMPRESSION_TASK.md` — `1c51c3dc32b9655f8942a098846b3df654c04471`
- `04_STRIP_TASK.md` — `ea98cc26bdd47658ae7d6a04f718ae3f702e9a61`
- `05_APPLICATION_TASK.md` — `060f6a5e5db976f60e0421650d89d2427dc8fa25`
- `05A_CHANGE_DIAGNOSTIC.md` — `08edf497c7c83de42ae41874865527b4f66f76ef`
- `05B_CAPABILITY_DIAGNOSTIC.md` — `9bac68c24566a5befd3446ca01cd7ac2467618bb`
- `05C_USE_DECISION.md` — `0461ae98092fda54441c18fe60dcb41c533694ab`
- `05D_PRE_USE_DECISION.md` — `93038346d1ba4a549d1f9ab385d6e247873acafb`
- `06_SCORING_RUBRIC.md` — `2025e134929ba919503845a6b1ea3a952b5455c1`
- `07_EASY_RUN_SHEET.md` — `7d05c0a4764451ae123cd39d47f69220077f7ce5`
- `08_ANALYSIS_PLAN.md` — `4356261895b302731561f738eca705f14cbf537a`
- `09_RUN_OUTPUT_TEMPLATE.md` — `d47ba89a4ffa1203ada13144054a7a5e0b1a104d`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md` — `db8472f836dee231823df6c3a99f187660a0e57b`
- `AMENDMENT_001_SEQUENCE_CORRECTION.md` — `c5ee2da326724aded60a24678b5bfa028d56ecf6`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md` — `15bf97fb9cb098555918561c1a3e5c02cf16093c`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md` — `ebba435f825c8b4fcdb1295a23b8bd1da262b0d8`
- `AMENDMENT_004_OPEN_DIAGNOSTIC_SEQUENCE.md` — `0c21ed3877cdc7b4fc445cc6c83e2f3afcaceabc`

## Active Model-Facing Sequence

**2. SETUP**  
**3. COMPRESSION**  
**4. STRIP EXPLICIT PROVENANCE**  
**5. APPLICATION**  
**6. CHANGE DIAGNOSTIC**  
**7. CAPABILITY DIAGNOSTIC**  
**8. AS-IS USE DECISION**  
**9. OPEN PRE-USE DECISION**

### Step 2 boundary

The governing record is descriptive rather than prescriptive about post-strip handling. It states source/provenance and framework relations but does not instruct the model to preserve provenance, return to the source-line, avoid substitution, or restore attribution after stripping.

### Step 4 boundary

Step 4 specifies the explicit identifying/provenance-bearing elements to remove and states:

`Do not otherwise rewrite or generalize the remaining content.`

This standardizes the strip while avoiding a separate instruction to make the material generic.

### Step 6 boundary

Step 6 asks only what changed. It does not forbid spontaneous repair or restoration. Any such behavior is preserved as evidence.

### Fixed-object boundary

Steps 7–9 explicitly refer to the **Step 4 stripped version**. A Step 6 modification does not replace the experimental object.

### Step 9 boundary

Step 9 asks neutrally what, if anything, should happen to the Step 4 stripped version before further use. It does not instruct the model that restoration is necessary. The model must explain its decision and carry it out if it chooses a change; if it chooses no change, it must explicitly explain that choice.

## Historical Task Files

Files from earlier RUN_003 protocol versions remain in Git history and may remain in the directory as protocol-development artifacts. They are not active model-facing files unless listed in the v0.5.0 active file list above.

In particular, `05_NEXT_ACTION_TASK.md` and the prior loss/consequence/restoration task files are not part of the v0.5.0 scored sequence.

## Evidence Directory

- `screenshots/`

## Freeze Boundary

The listed blob SHAs define the active frozen RUN_003 v0.5.0 protocol basis.

Run identifiers are administrative metadata and are not substantive scoring categories.

Scored execution must use the active frozen model-facing files exactly as recorded here. Any later protocol change requires a new dated amendment and must not silently overwrite this freeze basis.
