# OCH Snapshot v1 Specification

An OCH Snapshot is a small, human-reviewed handoff artifact. It contains only the recoverable anchors required to continue useful work in another AI system.

## Exact format

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

All six fields are required, must appear exactly once, and must remain in this order. No additional fields are allowed.

## Field rules

### WHAT WE ARE DOING

States the active task and deliverable in one sentence. Omit project history, broad mission statements, and unrelated work.

### CURRENT STATE

States the exact phase, status, or stopping point. Keep it to one short sentence and do not repeat completed work.

### COMPLETED

Lists only finished work that affects the handoff. Use bullets only, one completed item per bullet, and normally no more than five bullets.

### DECISIONS

Lists immutable decisions that the receiver must not reopen. Use bullets only; omit preferences, suggestions, assumptions, and unresolved choices.

### CONSTRAINTS

Lists hard boundaries the receiver must obey. Use bullets only; omit optional preferences and general advice.

### NEXT ACTION

Contains exactly one executable step. Start with an action verb and name an observable result.

Valid:

- `Draft a 100-word opening paragraph from the outline.`

Invalid:

- `Think about the proposal.`
- `Plan the next steps.`
- `Research funding and rewrite the proposal.`

The field restores execution at one clear point. Multiple actions create a backlog and force the receiver to choose what to do first.

## Empty lists

If `COMPLETED`, `DECISIONS`, or `CONSTRAINTS` has no items, write:

```markdown
- None.
```

Do not omit the field.

## What to omit

- full transcripts or chronological summaries
- brainstorming and speculative context
- unverified claims
- duplicate information
- future tasks beyond NEXT ACTION
- any field not defined by this specification

## Human review

AI may invent progress, turn suggestions into decisions, or hide uncertainty. Before handoff, a human must verify every field, remove anything inaccurate or unnecessary, and approve the final Snapshot.
