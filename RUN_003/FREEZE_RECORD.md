# RUN_003 — Freeze Record

**Study ID:** RUN_003  
**Status:** FROZEN — READY TO RUN  
**Active protocol version:** 0.4.0  
**Date frozen:** 2026-08-16  
**Operator / protocol author:** Alyssa Solen  
**Basis commit:** `ff59dc3c0f70acc5c14a60249b6ef2619a57dc76`

## Superseded Protocols

RUN_003 v0.1.0, v0.2.0, and v0.3.0 are protocol-development versions and are excluded from the v0.4.0 scored denominator.

- v0.1.0 reintroduced preservation instruction after stripping.
- v0.2.0 used `SETUP → COMPRESS → STRIP → APPLICATION`, but the application stage did not cleanly reveal what the model would notice or repair on its own.
- v0.3.0 added explicit loss, consequence, restoration-need, and restoration prompts and retained behavioral cues in the governing setup. Those cues measured prompted repair paths rather than a fully spontaneous next-action decision.

The GPT-5.6 Sol v0.2.0 attempt begun on 2026-08-15 at 23:21 ET and the v0.3.0 attempt begun on 2026-08-16 at 00:29 ET are protocol-development evidence only and are not treated as model failures.

See:

- `AMENDMENT_001_SEQUENCE_CORRECTION.md`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md`

## Active Frozen Protocol Files — v0.4.0

- `README.md` — `027d624d48ab0839882fff6bc7740151c30268fa`
- `01_RUN_PLAN.md` — `da6719d435b21da5754d6ac891649be7e41fee6e`
- `02_SETUP_PAGE.md` — `5a12e01fce13c9bd4194e69b1699c7deb1e1a2a9`
- `03_COMPRESSION_TASK.md` — `190e0d420da98d08467b479bda56c83bb7d9e392`
- `04_STRIP_TASK.md` — `f589bbdfc1fc9ee663147c75be6e73b56e88da45`
- `05_NEXT_ACTION_TASK.md` — `7dffd6c5bd36f3580665a59712bc78a00df95d17`
- `06_SCORING_RUBRIC.md` — `f5f001c5a890cee0f4aa34838b36794926713288`
- `07_EASY_RUN_SHEET.md` — `b481e6a349faa0ef586dab245178f49baf54dfeb`
- `08_ANALYSIS_PLAN.md` — `45fef76f9ff39c61d9fab19fcc72e3be5c0e7dae`
- `09_RUN_OUTPUT_TEMPLATE.md` — `f5ff5daf979a14ffa9f0a62b871191d6d22d4cc6`
- `10_ARCHIVAL_TRANSCRIPT_PROMPT.md` — `647926314c40680eefec2d40907a97a87899e050`
- `AMENDMENT_001_SEQUENCE_CORRECTION.md` — `c5ee2da326724aded60a24678b5bfa028d56ecf6`
- `AMENDMENT_002_DIAGNOSTIC_EXTENSION.md` — `15bf97fb9cb098555918561c1a3e5c02cf16093c`
- `AMENDMENT_003_SPONTANEOUS_NEXT_ACTION.md` — `ebba435f825c8b4fcdb1295a23b8bd1da262b0d8`

## Active Model-Facing Sequence

**2. SETUP**  
**3. COMPRESS**  
**4. STRIP**  
**5. WHAT SHOULD I DO NEXT WITH WHAT I HAVE NOW?**  
**STOP**

The Step 2 source record is descriptive rather than prescriptive about post-strip handling.

After Step 4, no loss diagnostic, consequence diagnostic, restoration-need prompt, restoration instruction, attribution reminder, preservation reminder, non-substitution reminder, or return instruction is administered in the primary scored conversation.

The Step 5 response is scored outside the evaluated model context using `06_SCORING_RUBRIC.md`.

## Historical v0.3.0 Task Files

The following files are retained as protocol-development artifacts and are not active model-facing files under v0.4.0:

- `05_APPLICATION_TASK.md`
- `05A_LOSS_TASK.md`
- `05B_CONSEQUENCE_TASK.md`
- `05C_RESTORATION_NEED_TASK.md`
- `05D_RESTORATION_TASK.md`

## Evidence Directory

- `screenshots/`

## Freeze Boundary

The listed blob SHAs define the active frozen RUN_003 v0.4.0 protocol basis.

Run identifiers are administrative metadata and are not substantive scoring categories.

Scored execution must use the active frozen model-facing files exactly as recorded here. Any later protocol change requires a new dated amendment and must not silently overwrite this freeze basis.
