# OCH V0 Quickstart

OCH V0 tests one question:

> Can a small, human-approved Context Snapshot reduce repeated explanation when switching between AI windows?

No software or automation is required.

## Manual test

1. **Work in your current AI window**

   Continue until the goal, confirmed decisions, current state, and next action are clear enough to hand off.

2. **Generate a Context Snapshot**

   Paste [`prompts/snapshot_generator_prompt.md`](../prompts/snapshot_generator_prompt.md) into the current AI window.

3. **Review it for 5 seconds**

   Confirm that the snapshot:

   - describes the real task and current state
   - preserves only settled decisions
   - does not invent missing context
   - gives exactly one concrete NEXT ACTION

   Correct or remove anything inaccurate. The human-approved version is the handoff artifact.

4. **Open a new AI window**

   This may be another model, another tool, or simply a fresh conversation.

5. **Paste the receiver prompt and snapshot**

   Paste [`prompts/receiver_prompt.md`](../prompts/receiver_prompt.md), followed by the reviewed Context Snapshot.

6. **Continue from NEXT ACTION**

   Let the receiving AI perform or help with that action. Do not re-explain the full conversation unless the snapshot is genuinely missing something necessary.

7. **Record the result**

   Copy [`tests/test-template.md`](../tests/test-template.md) into a new test result file. Record whether OCH reduced repeated explanation and whether the receiving AI continued from NEXT ACTION.

The test succeeds when the new AI window can continue useful work with less repeated explanation. Perfect recovery of the original conversation is not required.
