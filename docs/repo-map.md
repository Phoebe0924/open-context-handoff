# OCH Repository Map

OCH is organized into separate narrative, protocol, prompt, example, and validation layers. A first-time user should begin with [`quickstart.md`](quickstart.md) and follow one complete manual handoff.

## Narrative layer

- [`README.md`](../README.md): English overview of OCH and its purpose.
- [`README_CN.md`](../README_CN.md): Chinese overview of OCH and its purpose.

## Protocol layer

- [`snapshot-format.md`](snapshot-format.md): canonical OCH Snapshot v1 specification.

## Prompt layer

- [`snapshot_generator_prompt.md`](../prompts/snapshot_generator_prompt.md): asks the source AI to draft a six-field V1 Snapshot.
- [`receiver_prompt.md`](../prompts/receiver_prompt.md): tells the receiving AI to preserve decisions and constraints and continue from one next action.
- [`quick-snapshot-template.md`](../prompts/quick-snapshot-template.md): compact V1 template.
- [`quick-receiver-prompt.md`](../prompts/quick-receiver-prompt.md): compact V1 receiver instruction.

## Example layer

- [`minimal-snapshot.md`](../examples/minimal-snapshot.md): compact valid V1 Snapshot.
- [`bad-vs-good-snapshot.md`](../examples/bad-vs-good-snapshot.md): V1 conformance comparison.

## Validation layer

- [`v1-spec-conformance-test.md`](../tests/v1-spec-conformance-test.md): V1 manual conformance design.
- [`v1-validation-run-001.md`](../tests/v1-validation-run-001.md): first V1 validation run record awaiting manual completion.
- [`test-template.md`](../tests/test-template.md): reusable V1 result template.
- [`7-run-validation-log.md`](../tests/7-run-validation-log.md): preserved V0 cross-system evidence.
- [`001-chatgpt-to-claude-result.md`](../tests/001-chatgpt-to-claude-result.md) and [`002-chatgpt-to-claude-result.md`](../tests/002-chatgpt-to-claude-result.md): preserved V0 result records.
- [`001-chatgpt-to-claude.md`](../snapshots/001-chatgpt-to-claude.md): preserved V0 Snapshot artifact.

## Guidance and historical records

- [`quickstart.md`](quickstart.md): current V1 manual flow.
- [`v0-scope.md`](v0-scope.md), [`v0-validation-plan.md`](v0-validation-plan.md), and [`audit-notes.md`](audit-notes.md): historical V0 scope and validation guidance.
- [`v1-release-gap.md`](v1-release-gap.md) and [`v1-alignment-report.md`](v1-alignment-report.md): V1 release-readiness records.
- [`future-direction.md`](future-direction.md): deferred research directions, not current commitments.
