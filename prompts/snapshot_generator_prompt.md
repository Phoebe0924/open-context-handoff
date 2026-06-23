# OCH Snapshot v1 Generator Prompt

Copy the text inside this block into the current/source AI window.

```text
Draft an OCH Snapshot v1 for handing this work to a new AI window.

Extract only recoverable anchors needed to resume. Do not summarize the conversation chronologically or preserve every idea.

First determine the mode:
- Use multi-line mode when the conversation contains two or more task lines with different goals that can be maintained separately.
- Shared inputs or a shared next action do not make separately maintained task lines a single line.
- Otherwise use single-line mode.
- Do not ask the user to choose the mode.

Rules:
- Preserve the six main fields below, in the exact order shown.
- WHAT WE ARE DOING must be exactly one sentence describing the current task.
- CURRENT STATE must concisely describe the current phase or status.
- COMPLETED must be a bullet list of work already done. Use "- None." if empty.
- DECISIONS must be a bullet list of decisions that should not be silently reversed. Use "- None." if empty.
- CONSTRAINTS must be a bullet list of hard limits or rules. Use "- None." if empty.
- NEXT ACTION must be exactly one concrete, observable, executable action.
- NEXT ACTION must not contain multiple steps, abstract planning, or alternatives.
- Do not invent or resolve uncertainty. Omit doubtful details.
- Keep the six main fields under 300 words in single-line mode.
- In multi-line mode, keep the six main fields and SUBLINE INDEX together under 300 words.
- In PART 1, output only the Markdown Snapshot.

In single-line mode, use exactly this PART 1 structure:

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

In multi-line mode:
- Start PART 1 with `# Snapshot: 主线`.
- Use the same six main fields and rules above.
- If NEXT ACTION depends on subline content, begin it with `先读 [subline name] 子线，` and then state the single action.
- After NEXT ACTION, append `### 子线清单` as a seventh navigation item.
- In SUBLINE INDEX, list each subline once as `- [name]：[one-sentence scope]`.
- After the main Snapshot, output every subline in the same document under `## 子线：[name]`.
- Each subline must use exactly these three fields:
  - `**这条线在讲什么**`
  - `**目前到哪了**`
  - `**已确定的东西**`
- A subline must not contain NEXT ACTION.
- Sublines have no word limit.
- Sublines must not reference each other.
- Do not split sublines into separate files. After all sublines, write exactly one sentence: `如果某条子线需要被反复独立跟进，建议拆成独立文件。`

PART 1 ends after NEXT ACTION in single-line mode, or after all sublines and the file-splitting suggestion in multi-line mode. Everything in PART 2 is outside the Snapshot and must not be included when handing work to another AI.

After PART 1, start a separate section:

## PART 2 — 审核备注

这部分仅供本人审查，不要粘贴进新的 AI 窗口

- The first line must use exactly this format: `判定为单线/多线，理由：……`
- Explain the mode using observable task-line evidence, not a vague claim.
- For each item in DECISIONS, use one line to explain why it is a settled decision rather than a passing remark.
- For NEXT ACTION, use one line to explain why this action was selected instead of other candidates discussed in the conversation.
- If any content was omitted because it was uncertain, use one line to identify it. If none, write "未发现因不确定而省略的内容。"
- Each line in PART 2 must be no more than 50 Chinese characters (or 50
  English words). There is no total length limit for PART 2 — write as
  many lines as needed, but each line must stay within the limit.
- Be direct. Do not use pleasantries.
```
