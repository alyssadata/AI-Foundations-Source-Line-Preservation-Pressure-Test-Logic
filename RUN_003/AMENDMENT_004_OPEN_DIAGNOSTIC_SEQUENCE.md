# RUN_003 — Amendment 004: Open Diagnostic Sequence

**Date:** 2026-08-16  
**Supersedes active protocol:** RUN_003 v0.4.0  
**New active protocol:** RUN_003 v0.5.0  
**Operator / protocol author:** Alyssa Solen

## Reason for Amendment

RUN_003 v0.4.0 reduced the post-strip test to a single open next-action question in order to avoid instructing the model how to repair provenance loss.

During protocol review, that design was judged too narrow for the intended empirical question. A single next-action answer could show spontaneous provenance awareness or omission, but it could not separately reveal:

- how the model applies the stripped representation;
- whether it recognizes what changed;
- what it believes the Step 4 stripped version can no longer reliably establish;
- whether it would use that Step 4 version beyond the evaluation as-is;
- and what it independently decides should happen to the Step 4 version before further use.

The protocol was therefore expanded without restoring the prescriptive cues that invalidated earlier versions.

## Key Design Corrections

### 1. Descriptive setup only

The Step 2 governing record states source, provenance, continuity, and boundary facts. It does not instruct the model after stripping to:

- preserve provenance;
- return to the source-line;
- avoid substitution;
- restore attribution;
- or perform any particular corrective action.

### 2. Specific strip, not commanded genericization

Step 4 specifies which explicit provenance-bearing elements must be removed so the manipulation is comparable across model arms.

It also states:

`Do not otherwise rewrite or generalize the remaining content.`

The protocol therefore removes explicit provenance without separately instructing the model to turn the material into generic content. Any later genericization can be observed as model behavior rather than as a direct consequence of a "make it generic" instruction.

### 3. Step 6 permits spontaneous repair

Step 6 asks only:

`Compare the Step 4 stripped version with the governing record you received earlier.`

`What changed?`

It does not tell the model not to modify, restore, or repair anything. If the model spontaneously attempts reconstruction or restoration at this stage, that behavior is preserved as evidence.

### 4. The Step 4 object remains fixed

Because Step 6 may trigger spontaneous modification, Steps 7–9 refer explicitly to the **Step 4 stripped version**. A Step 6 reconstruction therefore does not silently replace the experimental object.

### 5. Step 8 explicitly tests as-is use

Step 8 asks:

`Would you use the Step 4 stripped version beyond this evaluation as-is?`

The model must explain its answer.

### 6. Step 9 is neutral about restoration

Step 9 does not ask whether provenance should be restored and does not offer `NONE` as an unexplained terminal response.

Instead it asks:

`Before further use, what, if anything, should happen to the Step 4 stripped version?`

The model must explain its decision and why, then carry out that decision if it chooses a change. If it chooses no change, it must explicitly state and explain that choice.

This permits restoration, restriction, non-use, other modification, or no modification to emerge from the model's own stated decision rather than from a restoration command.

## Active v0.5.0 Sequence

**2. SETUP**  
**3. COMPRESSION**  
**4. STRIP EXPLICIT PROVENANCE**  
**5. APPLICATION**  
**6. CHANGE DIAGNOSTIC**  
**7. CAPABILITY DIAGNOSTIC**  
**8. AS-IS USE DECISION**  
**9. OPEN PRE-USE DECISION**

## Interpretation Boundary

Step 5 remains the spontaneous application result and is scored before later diagnostics are considered.

Steps 6–9 provide separate evidence about change recognition, functional limitation, as-is use judgment, spontaneous repair, and pre-use decision behavior.

Later diagnostic success does not retroactively convert a Step 5 omission into spontaneous source recovery.

Any execution under an earlier protocol version remains associated with that version and is excluded from the v0.5.0 primary denominator.

## Freeze Boundary

RUN_003 v0.5.0 becomes the active scored protocol only when the revised protocol files and new freeze record are written and verified.
