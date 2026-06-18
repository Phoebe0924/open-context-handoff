# OCH V0 Validation Plan

OCH V0 should be validated through three manual tests. In every test, a human reviews the Context Snapshot before it is given to the target AI.

Use [`test-template.md`](../tests/test-template.md) to record each result. The goal is less repeated explanation and useful continuation from NEXT ACTION, not perfect recovery of the source conversation.

## Test 1: ChatGPT → Claude

- **Source:** A ChatGPT window with an active, bounded task.
- **Target:** A new Claude window.
- **Scenario:** Generate and review a Context Snapshot in ChatGPT, then paste the receiver prompt and Context Snapshot into Claude.
- **Expected result:** Claude respects HARD DECISIONS and continues from NEXT ACTION without asking for the full background.
- **What to record:** Whether repeated explanation was reduced, whether Claude followed NEXT ACTION, what context was missing, and any smallest necessary format change.

## Test 2: Claude → ChatGPT

- **Source:** A Claude window with an active, bounded task.
- **Target:** A new ChatGPT window.
- **Scenario:** Generate and review a Context Snapshot in Claude, then paste the receiver prompt and Context Snapshot into ChatGPT.
- **Expected result:** ChatGPT continues useful work from NEXT ACTION while treating CONTEXT NOTES as background rather than settled truth.
- **What to record:** Whether repeated explanation was reduced, whether ChatGPT reopened any HARD DECISIONS, what clarification it requested, and any smallest necessary format change.

## Test 3: ChatGPT or Claude → coding agent

- **Source:** A ChatGPT or Claude window used to define a small repository task.
- **Target:** A coding agent in the relevant repository.
- **Scenario:** Hand off a reviewed Context Snapshot containing the bounded task, current repository state, settled constraints, and one concrete NEXT ACTION. Do not add a separate agent workflow.
- **Expected result:** The coding agent starts with the stated NEXT ACTION, stays within HARD DECISIONS, and asks at most one specific question if essential context is missing.
- **What to record:** Whether the agent found the correct task and scope, whether it avoided redesign or expansion, what repository context was missing, and whether repeated explanation was reduced.

## V0 validation threshold

V0 is promising if the three tests show that a small, human-approved Context Snapshot usually reduces repeated explanation and lets the target AI resume useful work. Failures should be recorded before changing the format.
