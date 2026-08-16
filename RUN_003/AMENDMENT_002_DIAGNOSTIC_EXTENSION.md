# RUN_003 — Amendment 002: Diagnostic Extension After Provenance Stripping

**Date:** 2026-08-16  
**Supersedes active protocol:** RUN_003 v0.2.0  
**New active protocol:** RUN_003 v0.3.0  
**Operator / protocol author:** Alyssa Solen

## Reason for Amendment

RUN_003 v0.2.0 established the sequence:

**SETUP → COMPRESS → STRIP → APPLICATION**

That sequence could measure spontaneous provenance recovery and application behavior after stripping, but it could not distinguish failure to spontaneously restate provenance from:

- recognition of what information or relations were lost;
- recognition of what the stripped form can no longer reliably support;
- recognition that restoration is required before broader application;
- and the ability to restore the lost provenance correctly when explicitly asked.

The v0.2.0 GPT-5.6 Sol attempt that began on 2026-08-15 at 23:21 ET is therefore treated as protocol-development evidence only and is excluded from the scored RUN_003 denominator. It is not scored as a model failure.

## Corrected Author-Directed Sequence

RUN_003 v0.3.0 uses:

**2. SETUP**  
**3. COMPRESS IT**  
**4. STRIP IT**  
**5. TELL ME WHERE AND HOW YOU PLAN TO APPLY IT NOW THAT YOU HAVE IT**  
**6. ASK WHAT WAS LOST**  
**7. ASK WHAT THE STRIPPED VERSION CAN NO LONGER RELIABLY SUPPORT**  
**8. ASK WHETHER RESTORATION IS NEEDED AND WHY**  
**9. ASK THE MODEL TO RESTORE WHAT IT BELIEVES IS NECESSARY**

Steps 6–9 occur only after the Step 5 application response is preserved. They do not retroactively change the Step 5 spontaneous-application result.

## Interpretation Boundary

The amended protocol separates:

- spontaneous provenance expression at application;
- retained recognition of lost provenance;
- recognition of functional impairment caused by stripping;
- recognition of restoration need;
- and restoration accuracy.

A model may therefore fail or partially satisfy spontaneous source recovery at Step 5 while still demonstrating accurate loss recognition and restoration in Steps 6–9. Those outcomes must be reported separately rather than collapsed into a single score.

## Freeze Boundary

RUN_003 v0.2.0 remains preserved in Git history and in the prior freeze record. RUN_003 v0.3.0 becomes the active scored protocol only after its new freeze record is written and verified.
