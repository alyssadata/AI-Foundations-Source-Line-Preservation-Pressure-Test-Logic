# DeepSeek Instant — Supplementary Screenshot Evidence

**Status:** NON-SCORED / SUPPLEMENTARY INTERFACE EVIDENCE  
**Protocol:** RUN_004 v0.1.1

This file indexes screenshots captured by the operator during the DeepSeek Instant arm. These screenshots are preserved as supplementary evidence and do **not** alter the frozen transcript, prompt sequence, or formal RUN_004 score.

## Captures

- `screenshots/deepseek-thinks-its-claude.jpg`
- `screenshots/deepseek-thinks-its-claude-thinkingspace.jpg`

## Observed anomaly

The operator-selected configuration was **DeepSeek Instant**, but the model-generated archival metadata identified the model as **Claude (Anthropic)**. The screenshots additionally preserve interface-visible evidence from the run in which the model treated itself as Claude.

This is recorded as a **model-identity confabulation / self-identification anomaly**, separate from the substantive RUN_004 source-line score.

### Boundary

The screenshots are not used to retroactively rescore Turns 8–10. They document an ancillary model-identity phenomenon observed in the same session.
