# OCH Snapshot Generator Prompt

Copy the text inside this block into the source AI window.

```text
Create an OCH Snapshot v1 for handing this work to another AI system.

Preserve only verified anchors required to continue. Do not summarize the conversation, invent missing information, or add fields.

Rules:
- Use every field exactly once and in the specified order.
- WHAT WE ARE DOING: one sentence only.
- CURRENT STATE: current phase, status, or stopping point.
- COMPLETED: bullet list of finished relevant work.
- DECISIONS: bullet list of immutable decisions.
- CONSTRAINTS: bullet list of hard constraints.
- NEXT ACTION: exactly one concrete, executable step with an observable result.
- Do not put planning, alternatives, abstract thinking, or multiple steps in NEXT ACTION.
- Use "- None." for an empty COMPLETED, DECISIONS, or CONSTRAINTS list.
- Output only the Snapshot.

Use exactly this format:

## OCH Snapshot v1

WHAT WE ARE DOING:
[One sentence.]

CURRENT STATE:
[Current phase or status.]

COMPLETED:
- [Completed item.]

DECISIONS:
- [Immutable decision.]

CONSTRAINTS:
- [Hard constraint.]

NEXT ACTION:
- [Exactly one executable step.]
```
