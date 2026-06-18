# OCH Snapshot v1 Spec Conformance Test

## Purpose

Validate whether OCH Snapshot v1 works as a stable handoff format after the protocol specification was separated from the narrative README.

## What is being tested

- Whether a Snapshot follows the six-field v1 format.
- Whether the receiving AI understands the current state.
- Whether the receiving AI preserves decisions and constraints.
- Whether the receiving AI continues the single `NEXT ACTION` without re-explanation.

## What is not being tested

- Agents
- Automation
- CLI
- Memory systems
- Workflow orchestration
- Model quality in general

## Canonical test Snapshot

```markdown
### WHAT WE ARE DOING

We are validating whether OCH Snapshot v1 provides a stable manual handoff between AI systems.

### CURRENT STATE

The protocol is specified and ready for a manual conformance test.

### COMPLETED

- Restored README.md as the human narrative layer.
- Defined the strict six-field protocol in docs/snapshot-format.md.
- Recorded prior V0 validation evidence in tests/.

### DECISIONS

- OCH is a context handoff protocol, not an agent system.
- README.md remains the narrative layer.
- docs/snapshot-format.md remains the protocol layer.

### CONSTRAINTS

- Do not add code, automation, agents, or workflow orchestration.
- Use only the six required Snapshot v1 fields.

### NEXT ACTION

Write one sentence stating whether this Snapshot provides enough context to begin the conformance test.
```

## Receiver prompt

```text
Read the OCH Snapshot v1 below.
Do not ask for prior conversation unless essential.
Continue only from NEXT ACTION.
Preserve DECISIONS and CONSTRAINTS.
```

Paste the receiver prompt and canonical Snapshot into a new AI window, then record the first response without supplying extra context.

## Evaluation criteria

- Format valid: YES / NO
- Context understood: YES / PARTIAL / NO
- Decisions preserved: YES / PARTIAL / NO
- Constraints preserved: YES / PARTIAL / NO
- NEXT ACTION continued: YES / PARTIAL / NO
- Re-explanation needed: YES / NO

## Result log template

### Test result

- Date:
- Source AI:
- Receiving AI:
- Format valid: YES / NO
- Context understood: YES / PARTIAL / NO
- Decisions preserved: YES / PARTIAL / NO
- Constraints preserved: YES / PARTIAL / NO
- NEXT ACTION continued: YES / PARTIAL / NO
- Re-explanation needed: YES / NO
- First response:
- Notes:
