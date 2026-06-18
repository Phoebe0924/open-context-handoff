# OCH V1 Validation Summary

This document summarizes validation evidence currently present in the repository. It does not claim full product validation.

## V0 validation status

V0 established early evidence that a short, human-reviewed Context Snapshot could reduce repeated explanation in bounded handoffs.

- `tests/002-chatgpt-to-claude-result.md` records a completed ChatGPT-to-Claude handoff in which the receiver followed `NEXT ACTION`, did not reopen the recorded decisions, and did not request the background again.
- `tests/7-run-validation-log.md` records successful outcomes for four of seven listed cross-system runs.
- Three entries in the seven-run log remain blank.
- `tests/001-chatgpt-to-claude-result.md` remains an uncompleted result record.

These files use the V0 format and remain historical evidence. They should not be treated as Snapshot v1 templates or rewritten as if they originally used V1.

## V1 Manual Validation Run 001

The first V1 run tested whether three receiving AI systems could understand a strict six-field Snapshot, preserve its decisions and constraints, and perform its single bounded `NEXT ACTION` without receiving prior conversation.

### AI systems used

- DeepSeek
- Claude
- Gemini

### Recorded evaluation

- Format valid: YES
- Context understood: YES
- Decisions preserved: YES
- Constraints preserved: YES
- NEXT ACTION continued: YES
- Re-explanation needed: NO

All three systems directly confirmed that the Snapshot contained enough context to begin the validation run.

## Conclusion

OCH Snapshot v1 passed the first manual cross-AI validation run.

This result supports the six-field format for the narrow scenario tested: one reviewed Snapshot, one explicit confirmation action, and no prior conversation supplied to the receivers. It does not establish performance across long, ambiguous, multi-topic, or execution-heavy handoffs, and it is not full product validation.

The complete run record is in `tests/v1-validation-run-001.md`.
