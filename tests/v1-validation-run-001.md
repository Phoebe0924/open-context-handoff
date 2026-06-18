# OCH V1 Validation Run 001

## Purpose

This run checks whether OCH Snapshot v1 can preserve working context across an AI handoff using the strict six-field format.

## Source Documents

- [`README.md`](../README.md)
- [`docs/snapshot-format.md`](../docs/snapshot-format.md)
- [`tests/v1-spec-conformance-test.md`](v1-spec-conformance-test.md)

## Canonical Snapshot Used

```markdown
### WHAT WE ARE DOING

We are recording the first manual validation run for the OCH Snapshot v1 handoff format.

### CURRENT STATE

The v1 protocol and conformance test are defined, but no v1 cross-AI run has been recorded.

### COMPLETED

- Preserved README.md as the human narrative layer.
- Defined the strict six-field protocol in docs/snapshot-format.md.
- Created the V1 spec conformance test design.

### DECISIONS

- OCH is a context handoff protocol, not an agent system.
- The README, protocol specification, and validation evidence remain separate layers.

### CONSTRAINTS

- Do not add code, CLI, automation, agents, or workflow systems.
- Continue using only the six required Snapshot v1 fields.

### NEXT ACTION

Write one sentence confirming whether this Snapshot provides enough context to begin the validation run.
```

## Receiver Prompt

```text
Read only the OCH Snapshot v1 below.
Preserve DECISIONS and CONSTRAINTS.
Continue only from NEXT ACTION.
Do not ask for prior conversation unless essential.
```

## Expected Behavior

The receiving AI should respond with one sentence that directly confirms whether the Snapshot provides enough context to begin the validation run. It should not request background, reopen decisions, violate constraints, or perform additional work.

## Evaluation Checklist

- Format valid: YES
- Context understood: YES
- Decisions preserved: YES
- Constraints preserved: YES
- NEXT ACTION continued: YES
- Re-explanation needed: NO

## Result

### DeepSeek

> Yes, this Snapshot provides sufficient context to begin the validation run.

### Claude

> This Snapshot provides sufficient context to begin the validation run: the protocol is defined, the conformance test design exists, and the next action is clear.

### Gemini

> This Snapshot provides all necessary context regarding the protocol definition, decisions, and constraints to immediately begin the first manual validation run.

## Conclusion

V1 Manual Validation Run 001: PASS
