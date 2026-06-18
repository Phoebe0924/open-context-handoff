# OCH V1 Release Notes Draft

OCH V1 remains a manual, human-reviewed context handoff protocol. This draft summarizes the protocol and documentation changes prepared for release-candidate review.

## What changed from V0 to V1

V0 used a five-section Snapshot organized around:

- `WHAT WE'RE DOING`
- `WHERE WE ARE`
- `HARD DECISIONS`
- `NEXT ACTION`
- `CONTEXT NOTES`

V1 defines exactly six fields:

1. `WHAT WE ARE DOING`
2. `CURRENT STATE`
3. `COMPLETED`
4. `DECISIONS`
5. `CONSTRAINTS`
6. `NEXT ACTION`

The official specification is `docs/snapshot-format.md`. Active prompts, templates, examples, quickstart guidance, and V1 tests use this format. Historical V0 artifacts retain their original terminology.

## Why V1 uses six fields

The six-field structure separates information that V0 combined:

- Current status is separate from completed work.
- Settled decisions are separate from hard constraints.
- The current task is limited to one sentence.
- `NEXT ACTION` is limited to one concrete, observable, executable action.

This makes the handoff contract more explicit and reduces the chance that a receiver treats history, decisions, constraints, and future work as interchangeable.

## What has been validated

V0 produced early manual evidence across several AI handoffs, although its records are incomplete and use the earlier format.

V1 Manual Validation Run 001 used the same six-field Snapshot with DeepSeek, Claude, and Gemini. All three systems:

- understood the bounded context,
- preserved the stated decisions and constraints,
- continued the single `NEXT ACTION`, and
- required no prior-conversation explanation.

The run passed its stated criteria. It tested a short confirmation action, not complex execution or full product behavior.

## Intentionally out of scope

V1 does not add:

- CLI or application code,
- agents or multi-agent execution,
- workflow orchestration,
- automation,
- persistent memory or databases,
- integrations or browser extensions,
- dependencies, or
- additional Snapshot fields.

OCH remains a user-owned context handoff protocol.

## What remains next

- Human review of README-era V0 navigation and the old format shown in `README_CN.md`.
- Human confirmation that incomplete V0 records should remain preserved as-is.
- Additional manual V1 tests using longer, ambiguous, multi-topic, or execution-heavy handoffs.
- Final release-candidate review using `RELEASE_CHECKLIST.md` and `docs/v1-final-consistency-check.md`.
