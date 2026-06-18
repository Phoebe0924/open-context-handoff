# OCH V1 Release Checklist

This checklist is for human release-candidate review. It verifies the documentation-only OCH Snapshot v1 release scope.

## Required checks

- [x] README narrative preserved
  - `README.md` and `README_CN.md` remain the human narrative layer.
  - Neither file was rewritten during V1 alignment or release-candidate preparation.

- [x] Snapshot v1 protocol defined
  - `docs/snapshot-format.md` is the official protocol source.
  - It defines exactly six fields in the required order.

- [x] Prompts aligned with V1
  - Generator and receiver prompts use the official field names and receiver behavior.
  - `NEXT ACTION` remains one concrete executable action.

- [x] Examples aligned with V1
  - The minimal example follows the six-field protocol.
  - The bad-vs-good example explains V1-specific conformance failures.

- [x] V0 validation preserved
  - Original V0 Snapshot and test records remain in the repository.
  - Historical terminology has not been rewritten as if it were V1.

- [x] V1 validation recorded
  - `tests/v1-validation-run-001.md` records results from DeepSeek, Claude, and Gemini.
  - `tests/v1-validation-summary.md` limits its conclusion to the scenario actually tested.

- [x] No CLI added

- [x] No agent system added

- [x] No automation added

- [x] No code, workflow system, or dependencies added

## Remaining human review items

- [ ] Decide whether the protected README navigation should continue to say V0 for the V1 release candidate.
- [ ] Decide whether the old five-section example in `README_CN.md` is acceptable as preserved narrative or requires a separately approved terminology-only update.
- [ ] Confirm that incomplete V0 records remain intentionally incomplete historical evidence.
- [ ] Review `docs/v1-release-notes.md` for factual accuracy after it is drafted.
- [ ] Review the final consistency report and decide whether to designate the repository as an OCH V1 release candidate.

## Release boundary

This checklist does not authorize a GitHub release, CLI, agent design, automation, workflow system, implementation code, dependency addition, protocol redesign, or README rewrite.
