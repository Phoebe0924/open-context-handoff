# OCH Context Snapshot Format

An OCH Context Snapshot is a small, human-reviewed handoff artifact. It preserves only the anchors needed to continue useful work in another AI window.

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

Use 1–2 sentences to state the goal and relevant scope.

### WHERE WE ARE

Include both:

- **Done:** completed work that matters to the handoff
- **Current:** the exact present state or stopping point

### HARD DECISIONS

Include settled decisions only. Do not turn assumptions, suggestions, or unresolved questions into decisions.

### NEXT ACTION

Include one concrete action only. It should tell the receiving AI or user where to resume.

### CONTEXT NOTES

Include background only. Keep it minimal and do not treat it as a place for extra decisions or a conversation summary.

## Required safeguards

- If a detail is uncertain, omit it.
- A human must review and approve the snapshot before using it for a handoff.
