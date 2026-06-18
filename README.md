# OCH — Open Context Handoff

## 1. Problem

We move between ChatGPT, Claude, Gemini, Cursor, Claude Code, and other AI systems. Each switch breaks continuity: the user must re-explain the task, current state, decisions, constraints, and next step.

OCH exists so work can continue without reconstructing the full conversation.

## 2. Core Idea

Thinking should be portable even when context breaks across AI systems.

OCH turns the minimum human-approved context needed to continue into a **Context Snapshot**. The user owns and reviews that Snapshot before handing it to another AI.

## 3. OCH Snapshot Spec (STRICT)

### OCH Snapshot v1

```markdown
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

Rules:

- Use every field exactly once and in this order.
- Do not add fields.
- `WHAT WE ARE DOING` must be one sentence.
- `COMPLETED`, `DECISIONS`, and `CONSTRAINTS` must use bullet lists. Use `- None.` when a list is empty.
- `NEXT ACTION` must contain exactly one executable step with an observable result.
- Do not put planning, multiple steps, alternatives, or abstract thinking in `NEXT ACTION`.
- A human must review and approve the Snapshot before handoff.

## 4. Example

ChatGPT produces:

```markdown
## OCH Snapshot v1

WHAT WE ARE DOING:
Prepare a one-page community garden proposal.

CURRENT STATE:
The outline is complete; the opening paragraph is missing.

COMPLETED:
- Confirmed the audience and one-page limit.

DECISIONS:
- Focus on neighborhood food access.

CONSTRAINTS:
- Exclude event programming.

NEXT ACTION:
- Draft a 100-word opening paragraph from the outline.
```

Claude receives the reviewed Snapshot and drafts the paragraph without asking for the prior conversation.

## 5. Status

- V0 validated
- V1 in refinement
