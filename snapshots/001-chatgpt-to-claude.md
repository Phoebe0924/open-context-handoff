# OCH Context Snapshot Test 001

## Source

ChatGPT current window

## Target

Claude new window

## Scenario

Testing whether an OCH Context Snapshot can reduce repeated explanation when switching from ChatGPT to Claude.

## OCH Snapshot

### WHAT WE'RE DOING

We are defining and manually validating OCH — Open Context Handoff, a lightweight protocol for carrying working context across AI windows and tools.

### WHERE WE ARE

Done:
- Created GitHub repo
- Published English README
- Published Chinese README
- Clarified that V0 should stay minimal
- Defined OCH as user-owned context handoff, not memory system

Current:
- The first ChatGPT-to-Claude handoff has not yet been run.

### HARD DECISIONS

- V0 does not build a browser extension, CLI, MCP server, or automation.
- V0 only validates whether a simple Snapshot reduces repeated explanation.
- README is already published; stop polishing for now.
- OCH is about context ownership and continuity of thought.
- Human confirmation is required before using a Snapshot.

### NEXT ACTION

- Run the ChatGPT-to-Claude handoff with this Snapshot and record the result.

### CONTEXT NOTES

- The core pain is having to reconstruct the same working context in each new AI window.
