# OCH Snapshot v1 Specification

An OCH Snapshot is a small, human-reviewed context handoff artifact. It preserves only the anchors needed to continue useful work in another AI window.

OCH Snapshot v1 contains exactly six fields, in this exact order:

1. `WHAT WE ARE DOING`
2. `CURRENT STATE`
3. `COMPLETED`
4. `DECISIONS`
5. `CONSTRAINTS`
6. `NEXT ACTION`

No additional fields are allowed in the canonical Snapshot v1 format.

```markdown
### WHAT WE ARE DOING

[One sentence describing the current task.]

### CURRENT STATE

[A concise description of the current phase or status.]

### COMPLETED

- [Something already completed.]

### DECISIONS

- [A decision that should not be silently reversed.]

### CONSTRAINTS

- [A hard limit or rule.]

### NEXT ACTION

[Exactly one concrete, observable action.]
```

## Field rules

### `WHAT WE ARE DOING`

- Must contain exactly one sentence.
- Must describe the current task.

### `CURRENT STATE`

- Must describe the current phase or status.
- Must be concise.

### `COMPLETED`

- Must be a bullet list.
- Must record only what has already been done.
- If empty, must contain exactly `- None.`

### `DECISIONS`

- Must be a bullet list.
- Must record decisions that should not be silently reversed.
- If empty, must contain exactly `- None.`

### `CONSTRAINTS`

- Must be a bullet list.
- Must record hard limits or rules.
- If empty, must contain exactly `- None.`

### `NEXT ACTION`

- Must contain exactly one executable action.
- Must be concrete and observable.
- Must not contain multiple steps.
- Must not offer alternatives.
- Must not contain abstract planning.

## Human review

The source AI can compress context incorrectly, turn suggestions into decisions, or invent certainty. Before using a Snapshot:

- Remove inaccurate, uncertain, unnecessary, private, or sensitive details.
- Confirm that `COMPLETED` contains only finished work.
- Confirm that `DECISIONS` contains only settled decisions.
- Confirm that `CONSTRAINTS` contains only hard limits or rules.
- Confirm that `NEXT ACTION` contains exactly one executable action.
- Approve the final Snapshot before pasting it into another AI window.

## Conformance

A Snapshot conforms to OCH Snapshot v1 only when all six fields are present, use the exact names and order above, contain no additional fields, and satisfy every field rule.
