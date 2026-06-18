# OCH V0 Repository Map

OCH V0 is a manual-first, documentation-first protocol. A first-time user should begin with [`quickstart.md`](quickstart.md) and follow one complete handoff test.

## Root files

- [`README.md`](../README.md): English overview of OCH and its purpose.
- [`README_CN.md`](../README_CN.md): Chinese overview of OCH and its purpose.

## `docs/`

Guidance for understanding and validating V0:

- [`quickstart.md`](quickstart.md): first file to open; runs one manual Context Snapshot handoff.
- [`snapshot-format.md`](snapshot-format.md): defines the Context Snapshot structure and safeguards.
- [`repo-map.md`](repo-map.md): explains how to navigate the repository.
- [`v0-scope.md`](v0-scope.md): states what V0 includes and excludes.
- [`v0-validation-plan.md`](v0-validation-plan.md): defines the three manual validation tests.

## `prompts/`

Prompts used in a manual handoff:

- [`snapshot_generator_prompt.md`](../prompts/snapshot_generator_prompt.md): asks the source AI to draft a Context Snapshot.
- [`receiver_prompt.md`](../prompts/receiver_prompt.md): tells the target AI how to use the reviewed Context Snapshot.

## `examples/`

Reference examples:

- [`minimal-snapshot.md`](../examples/minimal-snapshot.md): a compact, valid Context Snapshot.
- [`bad-vs-good-snapshot.md`](../examples/bad-vs-good-snapshot.md): shows common problems and an improved version.

## `snapshots/`

Human-reviewed Context Snapshots used in specific manual tests:

- [`001-chatgpt-to-claude.md`](../snapshots/001-chatgpt-to-claude.md): the first ChatGPT-to-Claude test artifact.

## `tests/`

Manual test records:

- [`test-template.md`](../tests/test-template.md): copy this file for each new test.
- [`001-chatgpt-to-claude-result.md`](../tests/001-chatgpt-to-claude-result.md): result record for the first test.
