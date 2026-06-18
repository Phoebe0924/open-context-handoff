# OCH Context Snapshot Format

An OCH Context Snapshot is a small, human-reviewed handoff artifact. It preserves only the anchors needed to continue useful work in another AI window.

Recommended total length: **150–300 words**, and normally no more than **400 words**. Shorter is better when it still supports the NEXT ACTION.

```markdown
## OCH Snapshot

### WHAT WE'RE DOING

[The goal and scope in 1–2 sentences.]

### WHERE WE ARE

Done:
- [Completed work relevant to the handoff.]

Current:
- [The present state, question, or stopping point.]

### HARD DECISIONS

- [A confirmed decision that should not be reopened.]

### NEXT ACTION

- [One concrete action for the receiving AI or user.]

### CONTEXT NOTES

- [Minimal background that helps interpret the snapshot.]
```

## Section rules

### WHAT WE'RE DOING

**Purpose:** Identify the active task and its boundary.

**Recommended maximum:** 2 sentences or 50 words.

**Omit:** project history, motivation already obvious from the goal, and unrelated workstreams.

**Common mistakes:** describing a broad mission instead of the current task, or copying the opening summary of the full conversation.

### WHERE WE ARE

**Purpose:** Show what relevant work is complete and the exact stopping point.

**Recommended maximum:** 3 Done bullets and 2 Current bullets.

Include both:

- **Done:** completed work that matters to the handoff
- **Current:** the exact present state or stopping point

**Omit:** every intermediate step, abandoned exploration, and accomplishments that do not affect what happens next.

**Common mistakes:** mixing planned work into Done, saying “in progress” without a stopping point, or repeating WHAT WE'RE DOING.

### HARD DECISIONS

**Purpose:** Prevent the receiving AI from reopening choices that the human has already confirmed.

**Recommended maximum:** 5 bullets, one decision per bullet.

**Omit:** preferences that remain negotiable, predictions, assumptions, and rejected ideas that are unlikely to recur.

**Common mistakes:** upgrading an AI suggestion into a decision, preserving too many constraints, or writing vague principles that cannot guide the next action.

### NEXT ACTION

**Purpose:** Give the receiver one unambiguous place to resume.

**Recommended maximum:** 1 bullet and 25 words.

Use one concrete action only, with an observable output when possible. A single action matters because a handoff should restore momentum, not recreate a backlog or ask the receiver to choose among competing priorities.

**Omit:** secondary tasks, future phases, optional improvements, and “continue working on this.”

**Common mistakes:** combining actions with “and,” naming a broad goal instead of an action, or assigning work that depends on missing information.

### CONTEXT NOTES

**Purpose:** Supply minimal background needed to interpret the other sections.

**Recommended maximum:** 3 bullets or 75 words.

**Omit:** full conversation summaries, biography, speculative context, sensitive details not needed by the receiver, and anything already stated elsewhere.

**Common mistakes:** using this section as overflow, hiding decisions here, or adding details merely because they might be useful someday.

## What to omit from the entire Snapshot

- full transcripts or chronological summaries
- unresolved brainstorming unless it directly explains the current state
- emotional tone or personal data that the next action does not require
- claims the human cannot verify
- duplicated information

## Human review is required

The source AI can compress context incorrectly, turn suggestions into decisions, or invent a smooth narrative where the conversation was uncertain. Human review keeps the Snapshot user-owned: the human decides what is true, what may cross the system boundary, and what the receiver is authorized to treat as settled.

Before use:

- If a detail is uncertain, omit it.
- Remove anything unnecessary or sensitive.
- Confirm that HARD DECISIONS are genuinely settled.
- Confirm that NEXT ACTION contains exactly one executable action.
- Approve the final Snapshot before pasting it into another AI window.
