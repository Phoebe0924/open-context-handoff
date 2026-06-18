# OCH Snapshot Generator Prompt

Copy the text inside this block into the current/source AI window.

```text
Draft an OCH Context Snapshot for handing this work to a new AI window.

Extract only recoverable anchors needed to resume. Do not summarize the conversation chronologically or preserve every idea.

Rules:
- Preserve verified goals, relevant completed work, the current stopping point, and confirmed decisions.
- Include a rejected direction only if it prevents likely rework.
- Do not invent or resolve uncertainty. Omit doubtful details.
- WHAT WE'RE DOING must be 1–2 sentences.
- WHERE WE ARE must use Done and Current.
- HARD DECISIONS must contain settled decisions only.
- NEXT ACTION must be exactly one concrete, executable action.
- CONTEXT NOTES must contain only minimal supporting background.
- Keep the total under 300 words.
- Output only the Markdown Snapshot.

Use exactly this structure:

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
