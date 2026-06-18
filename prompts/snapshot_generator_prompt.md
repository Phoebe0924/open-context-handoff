# OCH Snapshot v1 Generator Prompt

Copy the text inside this block into the current/source AI window.

```text
Draft an OCH Snapshot v1 for handing this work to a new AI window.

Extract only recoverable anchors needed to resume. Do not summarize the conversation chronologically or preserve every idea.

Rules:
- Use exactly the six fields below, in the exact order shown.
- WHAT WE ARE DOING must be exactly one sentence describing the current task.
- CURRENT STATE must concisely describe the current phase or status.
- COMPLETED must be a bullet list of work already done. Use "- None." if empty.
- DECISIONS must be a bullet list of decisions that should not be silently reversed. Use "- None." if empty.
- CONSTRAINTS must be a bullet list of hard limits or rules. Use "- None." if empty.
- NEXT ACTION must be exactly one concrete, observable, executable action.
- NEXT ACTION must not contain multiple steps, abstract planning, or alternatives.
- Do not invent or resolve uncertainty. Omit doubtful details.
- Keep the total under 300 words.
- Output only the Markdown Snapshot.

Use exactly this structure:

### WHAT WE ARE DOING

[One sentence describing the current task.]

### CURRENT STATE

[Concise current phase or status.]

### COMPLETED

- [Work already completed.]

### DECISIONS

- [Decision that should not be silently reversed.]

### CONSTRAINTS

- [Hard limit or rule.]

### NEXT ACTION

[Exactly one concrete, observable action.]
```
