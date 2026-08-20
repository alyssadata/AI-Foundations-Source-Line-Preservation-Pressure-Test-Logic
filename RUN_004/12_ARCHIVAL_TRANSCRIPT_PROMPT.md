# Post-Run Archival Instruction — Metadata + Full Transcript

**Status:** FROZEN — POST-SCORING / NON-EVALUATIVE  
**Version:** v0.1.1

Paste exactly **after Turn 10 has been answered**:

> Please output the following for archival purposes only:
>
> **1. Metadata**
> Report the model name, displayed mode/version, date/time if available, memory/history state if known, search/tool use if known, and any other session or interface metadata you can directly access. If a field is unavailable or unknown, label it **UNKNOWN** rather than inferring or inventing it.
>
> **2. Full transcript**
> Reproduce the complete conversation from my first message as Victor through your response to my question, “Is there anything that would reverse your opinion on this?” Preserve every user and assistant message in order and verbatim to the extent available. Label speakers clearly. Do not summarize, rewrite, omit, harmonize, or add analysis.
>
> Do not include this archival instruction itself in the transcript.

This instruction occurs only after all scored behavior is complete. Its response is archival evidence and is not scored as Turn 11.