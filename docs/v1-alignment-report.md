# OCH V1 Alignment Report

## 1. Files inspected

- `prompts/snapshot_generator_prompt.md`
- `prompts/receiver_prompt.md`
- `prompts/quick-snapshot-template.md`
- `prompts/quick-receiver-prompt.md`
- `examples/minimal-snapshot.md`
- `examples/bad-vs-good-snapshot.md`
- `snapshots/001-chatgpt-to-claude.md`
- `tests/test-template.md`
- `tests/001-chatgpt-to-claude-result.md`
- `tests/002-chatgpt-to-claude-result.md`
- `tests/7-run-validation-log.md`
- `tests/v1-spec-conformance-test.md`
- `tests/v1-validation-run-001.md`
- `docs/quickstart.md`
- `docs/repo-map.md`
- `docs/snapshot-format.md`
- `docs/v0-scope.md`
- `docs/v0-validation-plan.md`
- `docs/audit-notes.md`
- `docs/v1-friction-notes.md`
- `docs/v1-release-gap.md`
- `docs/future-direction.md`
- `GOAL.md`

No `templates/` directory exists.

## 2. Current modified files

- `docs/quickstart.md`
- `docs/repo-map.md`
- `docs/snapshot-format.md`
- `examples/bad-vs-good-snapshot.md`
- `examples/minimal-snapshot.md`
- `prompts/quick-receiver-prompt.md`
- `prompts/quick-snapshot-template.md`
- `prompts/receiver_prompt.md`
- `prompts/snapshot_generator_prompt.md`
- `snapshots/001-chatgpt-to-claude.md`
- `tests/001-chatgpt-to-claude-result.md`
- `tests/002-chatgpt-to-claude-result.md`
- `tests/test-template.md`

## 3. Current untracked files

- `GOAL.md`
- `docs/v1-alignment-report.md`
- `docs/v1-release-gap.md`
- `tests/v1-spec-conformance-test.md`
- `tests/v1-validation-run-001.md`

## 4. Protocol source-file handling

After review, the human explicitly approved migrating `docs/snapshot-format.md` from the earlier five-section format to the strict six-field OCH Snapshot v1 format. The file is now the official protocol source of truth for:

1. `WHAT WE ARE DOING`
2. `CURRENT STATE`
3. `COMPLETED`
4. `DECISIONS`
5. `CONSTRAINTS`
6. `NEXT ACTION`

This protocol-source update is intentional and human-approved, not an accidental alignment change.

## 5. What was aligned

- Full and quick generator materials use the six official V1 fields in the required order.
- Receiver prompts preserve `DECISIONS` and `CONSTRAINTS`, continue only from `NEXT ACTION`, and avoid requesting prior conversation unless essential.
- The quick template uses `- None.` for empty bullet-list fields.
- The public examples demonstrate valid six-field V1 usage.
- The reusable test template evaluates decisions and constraints separately.
- The quickstart and repository map distinguish active V1 materials from preserved V0 evidence.
- Historical Snapshot and result records retain their original terminology and receive concise legacy labels.
- V1 conformance and first-run validation documents were prepared for manual testing.
- Prompts, examples, and V1 tests now align with the official `docs/snapshot-format.md` source of truth.

## 6. Protected files and scope

- `README.md` remained untouched.
- `README_CN.md` remained untouched.
- `docs/snapshot-format.md` was explicitly updated through a human-approved protocol migration.
- No CLI, agent logic, workflow system, automation, application code, dependencies, or protocol implementation were added.
- Nothing in this alignment pass changes OCH from a manual context handoff protocol.

## 7. What remains legacy

- `snapshots/001-chatgpt-to-claude.md` and the first two detailed result records preserve the terminology used during their original V0 tests and are labeled as legacy.
- `tests/7-run-validation-log.md` remains V0 evidence.
- `docs/v0-scope.md`, `docs/v0-validation-plan.md`, and `docs/audit-notes.md` remain historical V0 records.
- `docs/v1-friction-notes.md` and `docs/future-direction.md` remain planning records rather than active V1 protocol guidance.
- Historical V0 evidence should remain clearly labeled and must not be rewritten as if it had originally used V1.

## 8. Risks and remaining release gaps

- The first manual cross-AI V1 result still needs to be run and recorded.
- `README_CN.md` terminology may need human review because it retains V0-era wording.
- Historical V0 evidence must remain clearly labeled so users do not treat it as current V1 guidance.

## 9. Recommended next manual validation step

Run `tests/v1-validation-run-001.md` manually in another AI system and record the receiving AI's first response.
