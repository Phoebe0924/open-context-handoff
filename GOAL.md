# OCH First-User Readiness Goal

## Current Product Goal

Make OCH understandable in 30 seconds and usable in 15 minutes by a first-time GitHub visitor, while preserving OCH as a context handoff protocol and leaving the protected narrative and protocol source unchanged except for a minimal README entry link if needed.

## Current Phase

First-User Readiness — Phase 2 complete

## First-User Readiness Progress

### Phase 0 — Preflight

- Worktree was clean.
- Local `main` matched `origin/main` with no commits ahead or behind.
- Existing V1 release-readiness history and commits were preserved.
- No human decision was required to begin the first-visitor audit.

### Phase 1 — First visitor audit

- Created `docs/first-visitor-audit.md`.
- Confirmed that the README communicates the problem and protocol quickly.
- Identified entry-point ambiguity, V0/V1 wording noise, fragmented trial navigation, missing first-trial scoring, and missing troubleshooting as the main journey breaks.
- Identified the README narrative, core principle, protocol specification, and historical V0 evidence as protected project soul.

### Phase 2 — Start guide

- Created `START_HERE.md`.
- Reduced the first-use path to one purpose, one 15-minute outcome, and four practical steps.
- Linked directly to the existing generator and receiver prompts.
- Kept human review explicit and avoided adding new protocol claims.

### Next Action

Create the exact 15-minute trial and scoring guide.

---

# Previous Goal — OCH V1 Release Readiness

## Final Goal

Move OCH from a validated V0 experiment into a clean V1 release-ready GitHub project while preserving its narrative voice and keeping OCH a context handoff protocol.

Release readiness requires clear separation between the narrative, protocol, prompt, example, and validation layers.

## Previous Final Phase

V1 Release Candidate Preparation — Phase 5: Complete, stopped for human review

## Completed

- Established this long-running goal state.
- Confirmed that README.md remains the protected human narrative layer.
- Confirmed that no implementation, automation, CLI, dependency, or agent work belongs in this task.
- Audited all current repository files.
- Classified the important files by narrative, protocol, prompt, example, validation, or legacy/unclear layer.
- Created `docs/v1-release-gap.md`.
- Identified the minimal release blockers without implementing them.
- Received human approval to perform the V1 Alignment Pass.
- Inventoried prompts, examples, snapshots, tests, templates, and supporting docs against `docs/snapshot-format.md`.
- Recorded and reviewed the minimal per-file alignment plan.
- Aligned all active prompts and templates with the strict six-field V1 format.
- Converted the public examples to V1 field names and rules.
- Aligned the generic validation template and active manual guidance.
- Preserved historical V0 artifacts and labeled ambiguous records as legacy.
- Updated the release gap analysis to reflect resolved alignment gaps.
- Created `docs/v1-alignment-report.md`.
- Verified that active prompts and examples contain the six V1 fields in the required order.
- Verified that active aligned materials contain no old Snapshot field names.
- Verified that README files were untouched during the alignment pass.
- Preserved `docs/snapshot-format.md` as the protocol source of truth.
- Completed V1 Manual Validation Run 001 across DeepSeek, Claude, and Gemini.
- Recorded V1 Manual Validation Run 001 as PASS within its stated scope.
- Completed the release-readiness inventory in `docs/v1-release-readiness-inventory.md`.
- Created `tests/v1-validation-summary.md`.
- Summarized the mixed V0 evidence and the bounded V1 Run 001 result without claiming full product validation.
- Created `RELEASE_CHECKLIST.md`.
- Recorded completed release checks and remaining human-review items.
- Created `docs/v1-release-notes.md`.
- Documented the V0-to-V1 format migration, bounded validation evidence, exclusions, and next review items.
- Created `docs/v1-final-consistency-check.md`.
- Updated current navigation and release-gap status to reflect completion of V1 Run 001.
- Verified that README files and the Snapshot v1 protocol were unchanged during release-candidate preparation.
- Verified that no code, CLI, dependencies, agents, workflows, or automation were added.
- Verified that historical V0 evidence was not deleted.

## In Progress

- Awaiting human release-candidate review.

## Next Action

Review `RELEASE_CHECKLIST.md`, `docs/v1-release-notes.md`, and `docs/v1-final-consistency-check.md` together.

## Boundaries

- OCH is a context handoff protocol.
- Do not rewrite README.md or alter its philosophical narrative.
- Do not add code, CLI, dependencies, automation, agent logic, workflow systems, memory systems, or multi-agent execution.
- Do not redesign the project.
- Do not delete existing files.
- Keep V1 release work documentation-first and manual.

## Stop Conditions

- Stop after the V1 release-candidate consistency check is created and verified.
- Stop before any CLI, code, dependency, automation, agent, workflow, or protocol redesign work.
- Stop and request human review if a change would alter historical evidence or project positioning.

## V1 Release Candidate Preparation

### Phase 0 — Preflight

- Worktree was clean.
- V1 Manual Validation Run 001 was already committed.
- Local `main` matched `origin/main`.

### Phase 1 — Release readiness inventory

- Read the narrative, protocol, prompt, example, validation, historical, and goal layers.
- Created `docs/v1-release-readiness-inventory.md`.
- Identified stale release-status references and README-era V0 terminology as human-review risks.
- Preserved all historical V0 evidence without rewriting it as V1.

### Phase 2 — Validation summary

- Created `tests/v1-validation-summary.md`.
- Recorded that V0 evidence is useful but incomplete.
- Summarized V1 Run 001 across DeepSeek, Claude, and Gemini.
- Limited the conclusion to the bounded manual scenario actually tested.

### Phase 3 — Release checklist

- Created `RELEASE_CHECKLIST.md`.
- Confirmed protocol, prompt, example, historical-evidence, and validation readiness checks.
- Kept README terminology and incomplete V0 evidence as explicit human-review decisions.
- Reconfirmed that implementation work remains outside the release scope.

### Phase 4 — Release notes draft

- Created `docs/v1-release-notes.md`.
- Described the five-section V0 to six-field V1 migration.
- Recorded only the validation evidence actually present.
- Kept implementation, automation, agents, workflows, and protocol expansion out of scope.

### Phase 5 — Final consistency check

- Verified that both README files were untouched during release-candidate preparation.
- Verified that `docs/snapshot-format.md` remained stable and defines the six official V1 fields.
- Verified alignment across active prompts, examples, and V1 tests.
- Verified that no code, dependencies, CLI, agents, workflows, or automation were added.
- Verified that historical V0 evidence was preserved.
- Created `docs/v1-final-consistency-check.md`.
- Stopped before release creation, implementation work, or README changes.

## V1 Alignment Inventory

### Findings before alignment

- `prompts/snapshot_generator_prompt.md` — generates the old five-section format.
- `prompts/receiver_prompt.md` — instructs receivers using old field names.
- `prompts/quick-snapshot-template.md` — templates the old five-section format.
- `prompts/quick-receiver-prompt.md` — refers to `HARD DECISIONS` instead of `DECISIONS` and `CONSTRAINTS`.
- `examples/minimal-snapshot.md` — demonstrates the old five-section format.
- `examples/bad-vs-good-snapshot.md` — both examples and commentary use old field names.
- `tests/test-template.md` — generic validation template evaluates `HARD DECISIONS` rather than V1 decisions and constraints separately.
- `docs/quickstart.md` — active manual instructions evaluate old field names and identify themselves only as V0.
- `docs/repo-map.md` — navigation is V0-only and omits V1 validation and release-readiness documents.

### V1-aligned materials

- `docs/snapshot-format.md`
- `tests/v1-spec-conformance-test.md`
- `tests/v1-validation-run-001.md`

### Historical V0 materials to preserve

- `snapshots/001-chatgpt-to-claude.md`
- `tests/001-chatgpt-to-claude-result.md`
- `tests/002-chatgpt-to-claude-result.md`
- `tests/7-run-validation-log.md`
- `docs/v0-scope.md`
- `docs/v0-validation-plan.md`
- `docs/audit-notes.md`
- `docs/v1-friction-notes.md`
- `docs/future-direction.md`

These files are evidence or historical planning records. Their old terminology should not be rewritten as if it had been V1 at the time; ambiguous artifacts may receive a short legacy label.

## V1 Minimal Alignment Plan

| File | Issue | Minimal fix | Human review needed |
| --- | --- | --- | --- |
| `prompts/snapshot_generator_prompt.md` | Old fields and sentence rules | Replace structure and rules with the exact six-field V1 contract | No |
| `prompts/receiver_prompt.md` | Old receiver semantics | Preserve `DECISIONS` and `CONSTRAINTS`; continue only from `NEXT ACTION` | No |
| `prompts/quick-snapshot-template.md` | Old template | Replace with six V1 fields and valid empty-list markers | No |
| `prompts/quick-receiver-prompt.md` | Old field names | Use V1 receiver language | No |
| `examples/minimal-snapshot.md` | Invalid V1 example | Preserve scenario while mapping content into six fields | No |
| `examples/bad-vs-good-snapshot.md` | Comparison teaches old format | Convert both examples and explanations to V1 | No |
| `tests/test-template.md` | Generic template checks old decisions field | Split evaluation into V1 decisions and constraints | No |
| `docs/quickstart.md` | Active flow uses V0 terminology | Make the manual flow version-neutral/V1-aligned without changing product positioning | No |
| `docs/repo-map.md` | V0-only navigation | Update navigation to distinguish active V1 materials from preserved V0 evidence | No |
| Historical V0 artifacts | Old terminology may look canonical | Preserve content; add a concise legacy label only where ambiguity matters | No |
| `docs/v1-release-gap.md` | Describes gaps before alignment | Mark resolved items and retain remaining gaps | No |

No planned change alters the protocol, narrative, or historical test outcomes. No risky change requiring another pre-edit review was identified.

## Repository Map

### Narrative layer

- `README.md` — canonical English project narrative and philosophy; protected from rewrite.
- `README_CN.md` — Chinese project narrative; still contains a V0-format block and V0 status language.

### Protocol layer

- `docs/snapshot-format.md` — canonical strict OCH Snapshot v1 specification.

### Prompt layer

- `prompts/snapshot_generator_prompt.md` — full generator prompt for the strict six-field V1 format.
- `prompts/receiver_prompt.md` — full V1 receiver prompt preserving decisions and constraints.
- `prompts/quick-snapshot-template.md` — compact six-field V1 template.
- `prompts/quick-receiver-prompt.md` — compact V1 receiver instruction.

### Example layer

- `examples/minimal-snapshot.md` — compact valid V1 example.
- `examples/bad-vs-good-snapshot.md` — V1-specific bad-vs-good comparison.

### Validation layer

- `tests/7-run-validation-log.md` — V0 cross-system validation evidence; four runs have recorded outcomes and three remain blank.
- `tests/002-chatgpt-to-claude-result.md` — completed V0 manual handoff result.
- `tests/001-chatgpt-to-claude-result.md` — V0 result template that remains unfilled.
- `tests/test-template.md` — reusable V1 manual result template.
- `snapshots/001-chatgpt-to-claude.md` — V0 Snapshot artifact used by test 001.
- `tests/v1-spec-conformance-test.md` — V1 manual conformance design using the strict six-field format.
- `tests/v1-validation-run-001.md` — completed first V1 cross-AI validation run.
- `tests/v1-validation-summary.md` — factual summary of V0 evidence and V1 Run 001.

### Legacy / unclear

- `docs/quickstart.md` — active V1-aligned manual flow.
- `docs/repo-map.md` — current layer-based navigation map distinguishing V1 materials from V0 evidence.
- `docs/v0-scope.md` — historical V0 boundary record.
- `docs/v0-validation-plan.md` — historical V0 three-test plan.
- `docs/audit-notes.md` — historical V0 documentation audit.
- `docs/v1-friction-notes.md` — early V1 planning notes focused on access/toolization rather than the current strict-format release.
- `docs/v1-release-gap.md` — current release-readiness analysis and human-review decision point.
- `docs/v1-alignment-report.md` — completed V1 alignment record.
- `docs/v1-release-readiness-inventory.md` — release-candidate layer and risk inventory.
- `docs/v1-release-notes.md` — factual V1 release-notes draft.
- `docs/v1-final-consistency-check.md` — final release-candidate consistency results.
- `RELEASE_CHECKLIST.md` — human release-candidate review checklist.
- `docs/future-direction.md` — deferred research ideas; several ideas intentionally exceed the current product boundary.
- `GOAL.md` — long-running release-readiness state, not a public protocol layer.
