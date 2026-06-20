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
- Keep the Snapshot under 300 words.
- In PART 1, output only the Markdown Snapshot.

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

PART 1 ends immediately after NEXT ACTION. Everything below is outside the Snapshot and must not be included when handing work to another AI.

After the Snapshot, start a separate section:

## PART 2 — 审核备注

这部分仅供本人审查，不要粘贴进新的 AI 窗口

- For each item in DECISIONS, use one line to explain why it is a settled decision rather than a passing remark.
- For NEXT ACTION, use one line to explain why this action was selected instead of other candidates discussed in the conversation.
- If any content was omitted because it was uncertain, use one line to identify it. If none, write "未发现因不确定而省略的内容。"
- Each line in PART 2 must be no more than 50 Chinese characters (or 50
  English words). There is no total length limit for PART 2 — write as
  many lines as needed, but each line must stay within the limit.
- Be direct. Do not use pleasantries.
```
