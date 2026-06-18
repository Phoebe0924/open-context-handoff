# OCH V1 Release Readiness Inventory

This inventory maps the repository for V1 release-candidate review. It describes current purpose and status without changing project positioning or rewriting historical evidence.

## Layer summary

| Layer | Purpose | Current state |
| --- | --- | --- |
| Narrative | Explain the human problem, philosophy, and project boundary | Preserved in `README.md` and `README_CN.md` |
| Protocol | Define the official Snapshot v1 contract | Defined in `docs/snapshot-format.md` |
| Prompt | Generate and receive conformant Snapshots | Aligned with the six-field V1 protocol |
| Example | Demonstrate valid and invalid Snapshot usage | Aligned with the six-field V1 protocol |
| Validation | Record test design, reusable criteria, and observed results | V0 evidence preserved; V1 Run 001 recorded as PASS |
| Historical | Preserve prior scope, experiments, planning, and evidence | Retained without rewriting the past as V1 |

## Repository inventory

| File or area | Layer | Purpose | Release-candidate status |
| --- | --- | --- | --- |
| `README.md` | Narrative | Canonical English narrative and philosophy | Protected; retains V0-era navigation wording |
| `README_CN.md` | Narrative | Chinese narrative and philosophy | Protected; embedded V0 format differs from V1 and needs human presentation review |
| `docs/snapshot-format.md` | Protocol | Official strict six-field OCH Snapshot v1 specification | Current source of truth |
| `docs/quickstart.md` | Protocol guidance | Runs one manual V1 handoff | Current and V1-aligned |
| `docs/repo-map.md` | Navigation | Explains repository layers and starting path | Mostly current; still says V1 Run 001 awaits completion |
| `prompts/snapshot_generator_prompt.md` | Prompt | Produces a strict six-field Snapshot | Current and V1-aligned |
| `prompts/receiver_prompt.md` | Prompt | Preserves decisions and constraints and continues from one next action | Current and V1-aligned |
| `prompts/quick-snapshot-template.md` | Prompt | Provides a compact six-field template | Current and V1-aligned |
| `prompts/quick-receiver-prompt.md` | Prompt | Provides a compact receiver instruction | Current and V1-aligned |
| `examples/minimal-snapshot.md` | Example | Demonstrates a compact conformant Snapshot | Current and V1-aligned |
| `examples/bad-vs-good-snapshot.md` | Example | Contrasts nonconformant and conformant V1 usage | Current and V1-aligned |
| `tests/test-template.md` | Validation | Reusable manual V1 result template | Current and V1-aligned |
| `tests/v1-spec-conformance-test.md` | Validation | Defines the manual V1 conformance procedure | Current |
| `tests/v1-validation-run-001.md` | Validation | Records the first cross-AI V1 run across DeepSeek, Claude, and Gemini | Completed; PASS within its stated test scope |
| `snapshots/001-chatgpt-to-claude.md` | Historical | Preserves the original V0 Snapshot artifact | Clearly labeled legacy; do not rewrite as V1 |
| `tests/001-chatgpt-to-claude-result.md` | Historical | Preserves an uncompleted V0 test record | Clearly labeled legacy; remains incomplete |
| `tests/002-chatgpt-to-claude-result.md` | Historical | Preserves a completed bounded V0 handoff result | Clearly labeled legacy |
| `tests/7-run-validation-log.md` | Historical | Preserves the V0 multi-system validation log | Four outcomes recorded; three entries remain blank |
| `docs/v0-scope.md` | Historical | Records V0 boundaries | Preserve as historical scope |
| `docs/v0-validation-plan.md` | Historical | Records the original V0 manual test plan | Preserve; links to a template that has since become V1 |
| `docs/audit-notes.md` | Historical | Records the V0 documentation audit | Preserve as historical evidence |
| `docs/v1-friction-notes.md` | Historical | Records early V1 friction and toolization thoughts | Not current release guidance; could be mistaken for an implementation roadmap |
| `docs/future-direction.md` | Historical | Records deferred research ideas | Out of V1 release scope |
| `docs/v1-release-gap.md` | Release record | Records the earlier release-gap analysis | Stale: still says V1 Run 001 is unrecorded |
| `docs/v1-alignment-report.md` | Release record | Records the completed protocol migration and alignment pass | Historical report; file-status sections describe the pre-commit state |
| `GOAL.md` | Goal state | Tracks long-running release-readiness work and boundaries | Active; updated after each release-candidate phase |

No `templates/` directory, application source tree, dependency manifest, package file, or lockfile exists.

## Unclear or risky items

- The protected README files retain V0-era labels and navigation. This is a presentation issue, not authorization to rewrite them.
- `README_CN.md` contains the old five-section Snapshot example, which conflicts with the official V1 protocol.
- `docs/repo-map.md` and `docs/v1-release-gap.md` contain stale statements that V1 Run 001 is still pending.
- `docs/v1-alignment-report.md` accurately records an earlier worktree state but should be read as a completed phase report, not current git status.
- Historical V0 evidence contains old field names by design. It must remain clearly labeled and must not be normalized into V1.
- V0 evidence is mixed: some runs have results, while `tests/001-chatgpt-to-claude-result.md` and three entries in `tests/7-run-validation-log.md` remain incomplete.
- V1 Run 001 tested one bounded confirmation action across three AI systems. It does not establish full product validation or performance across complex handoffs.

## Release-candidate starting path

For a new user reviewing the active V1 protocol:

1. Read `README.md` for the project narrative.
2. Follow `docs/quickstart.md` for one manual handoff.
3. Use `docs/snapshot-format.md` as the official protocol source.
4. Copy the prompts in `prompts/`.
5. Review the examples in `examples/`.
6. Review V1 evidence in `tests/v1-validation-run-001.md`.

Historical V0 files remain evidence of the project path and should not be treated as current V1 templates.
