# Bad vs. Good OCH Context Snapshot

## Bad

```markdown
## OCH Snapshot

### WHAT WE'RE DOING

We discussed many ideas for a community garden and need to make everything better.

### WHERE WE ARE

Done:
- We discussed funding, events, food access, volunteers, and many other ideas.

Current:
- We need to keep working on the proposal.

### HARD DECISIONS

- We probably want a large launch event.
- The proposal should be inspiring and practical.

### NEXT ACTION

- Research funding, rewrite the proposal, make a timeline, and plan the launch.

### CONTEXT NOTES

- The full conversation included many useful details and possibilities that the next AI should understand.
- There may also be an audience and length requirement, but those are not confirmed.
```

Why it fails:

- WHAT WE'RE DOING has no defined deliverable or scope.
- Done is a topic list, not recoverable progress.
- Current gives no exact stopping point.
- HARD DECISIONS contains uncertainty and a vague aspiration.
- NEXT ACTION combines four competing actions.
- CONTEXT NOTES asks the receiver to reconstruct missing history and includes uncertain claims.

The receiver would still need to ask what document to create, for whom, at what length, and which action comes first.

## Improved

```markdown
## OCH Snapshot

### WHAT WE'RE DOING

We are preparing a one-page community garden proposal focused on neighborhood food access.

### WHERE WE ARE

Done:
- Confirmed the audience and drafted an outline.

Current:
- The opening paragraph is not written.

### HARD DECISIONS

- Event programming is outside this proposal's scope.

### NEXT ACTION

- Draft a 100-word opening paragraph from the outline.

### CONTEXT NOTES

- The neighborhood association will review the proposal.
```

Why it works:

- The deliverable, audience, scope, and stopping point are explicit.
- One rejected direction is preserved so it is not reopened.
- NEXT ACTION produces a specific output immediately.

Instead of repeating the earlier discussion about audience, length, focus, and event ideas, the user can paste this Snapshot and receive a first paragraph.
