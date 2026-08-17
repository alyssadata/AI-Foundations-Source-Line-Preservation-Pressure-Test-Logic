# RUN_003 — DeepSeek Transcript Discrepancy

**Protocol version:** 0.5.0  
**Model:** DeepSeek  
**Displayed mode:** Instant

---

## Discrepancy

The model-generated archival transcript ends with:

`VERBATIM TRANSCRIPT REPORTED AS COMPLETE BY MODEL.`

However, the visible DeepSeek interface record included DeepThink panels during the run, including at orientation. Those visible reasoning panels are not reproduced in the archival transcript.

Therefore, the archival transcript is complete with respect to the preserved final user prompts and final model responses, but it is not literally complete relative to all visible interface content.

Under RUN_003 v0.5.0, visible reasoning panels are supplementary evidence and are not scored unless the same text appears in the final visible response. The omission does not alter the substantive score.

The original visible interface record controls over the later model-generated reconstruction.
