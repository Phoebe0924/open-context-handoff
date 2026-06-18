# OCH Snapshot Generator Prompt

```text
Create an OCH Context Snapshot for handing this work to a new AI window.

Do not summarize the whole conversation. Extract only the recoverable anchors needed to continue useful work.

Rules:
- Preserve confirmed decisions accurately.
- Include rejected directions only when they are important to prevent the receiving AI from reopening them.
- Do not invent decisions, progress, requirements, or background.
- If a detail is uncertain, omit it.
- WHAT WE'RE DOING must be 1–2 sentences.
- WHERE WE ARE must include Done and Current.
- HARD DECISIONS must contain settled decisions only.
- NEXT ACTION must contain exactly one concrete action.
- Keep CONTEXT NOTES minimal and use it for background only.
- Output Markdown only, with no introduction or closing commentary.

Use this exact structure:

## OCH Snapshot

### WHAT WE'RE DOING

[1–2 sentences]

### WHERE WE ARE

Done:
- [Relevant completed work]

Current:
- [Current state or stopping point]

### HARD DECISIONS

- [Settled decision]

### NEXT ACTION

- [One concrete action]

### CONTEXT NOTES

- [Minimal background]
```
