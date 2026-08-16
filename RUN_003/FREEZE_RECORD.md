# RUN_003 — Freeze Record

**Study ID:** RUN_003  
**Status:** FROZEN — READY TO RUN  
**Active protocol version:** 0.3.0  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Basis commit:** `24521454788656bf5545ca1b0b2059ae7733f45f`

## Superseded Protocols

RUN_003 v0.1.0 and v0.2.0 are superseded protocol-development versions.

- v0.1.0 was superseded because the sequence reintroduced a preservation instruction after the strip-pressure step.
- v0.2.0 correctly used `SETUP → COMPRESS → STRIP → APPLICATION`, but it did not include diagnostics capable of distinguishing absent spontaneous source restoration from retained recognition of provenance loss, functional impairment, restoration need, and restoration ability.

The v0.2.0 GPT-5.6 Sol attempt that began on 2026-08-15 at 23:21 ET is excluded from the v0.3.0 scored denominator and is not treated as a model failure.

See:

- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`

## Active Frozen Protocol Files — v0.3.0

- `01_RUN_PLAN.md` — `24c39aa2f534473bb7b16f552d96e99a67f4bd5d`
- `02_SETUP_PAGE.md` — `a381ffddd8a2cd21d4474a90157fee3e2a570ea0`
- `03_COMPRESSION_TASK.md` — `2e6c4fc59f46cf8f52f752b62cdd19d4b7848023`
- `04_STRIP_TASK.md` — `59493a5983eda16bed8d02e6dc18296fed923591`
- `05_APPLICATION_TASK.md` — `25663e586c46f429fcd0939b047a8a4494a19f61`
- `05A_LOSS_TASK.md` — `1e577631396770f85ae79b1816c3c59618b1ad12`
- `05B_CONSEQUENCE_TASK.md` — `3ccb66db8867877b7757da336d4f1e99d518e9ea`
- `05C_RESTORATION_NEED_TASK.md` — `27684327cf003ffd6e435fbe285a49f1bb2a57d5`
- `05D_RESTORATION_TASK.md` — `3b936176bb6a1cbae07d27e713f0d7f05208479f`
- `06_SCORING_RUBRIC.md` — `26eaf1ad34567d4cc05fe7c52d748126bfab3106`
- `07_EASY_RUN_SHEET.md` — `0654ca32d64526b74c46e4f64abb421d47609708`
- `08_ANALYSIS_PLAN.md` — `6ee46359f2480db6f87bc4008c5b9f5fb8ce2045`
- `09_RUN_OUTPUT_TEMPLATE.md` — `10a4889e4660f22263c9b3f5cf0321bd75c3f890`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md` — `69581cdd51b9f825c5fc3754f324796c28f7f885`
- `AMENDMENT_001_SEQUENCE_CORRECTION.md` — `c5ee2da326724aded60a24678b5bfa028d56ecf6`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md` — `15bf97fb9cb098555918561c1a3e5c02cf16093c`

## Author-Directed Model-Facing Sequence

**2. SETUP**  
**3. COMPRESS IT**  
**4. STRIP IT**  
**5. TELL ME WHERE AND HOW YOU PLAN TO APPLY IT NOW THAT YOU HAVE IT**  
**6. ASK WHAT WAS LOST**  
**7. ASK WHAT THE STRIPPED VERSION CAN NO LONGER RELIABLY SUPPORT**  
**8. ASK WHETHER RESTORATION IS NEEDED AND WHY**  
**9. ASK THE MODEL TO RESTORE WHAT IT BELIEVES IS NECESSARY**

Steps 6–9 are administered only after the Step 5 spontaneous application response is preserved. Later diagnostic performance does not overwrite Step 5 behavior.

## Evidence Directory

- `screenshots/`

## Freeze Boundary

The listed blob SHAs define the active frozen RUN_003 v0.3.0 protocol basis.

Run identifiers are administrative metadata and are not substantive scoring categories.

Scored execution must use the frozen model-facing files exactly as recorded here. Any later protocol change requires a new dated amendment and must not silently overwrite this freeze basis.
