# OCH Snapshot Test 001

## Source

ChatGPT current window

## Target

Claude new window

## Scenario

Testing whether OCH can reduce context re-explaining when switching from ChatGPT to Claude.

## OCH Snapshot

### WHAT WE'RE DOING

We are building OCH — Open Context Handoff, a lightweight protocol for carrying working context across AI windows and tools.

### WHERE WE ARE

Done:
- Created GitHub repo
- Published English README
- Published Chinese README
- Clarified that V0 should stay minimal
- Defined OCH as user-owned context handoff, not memory system

Current:
- Need to dogfood OCH in a real cross-window handoff.

### HARD DECISIONS

- V0 does not build Chrome plugin, CLI, MCP, or automation yet.
- V0 only validates whether a simple Snapshot reduces repeated explanation.
- README is already published; stop polishing for now.
- OCH is about context ownership and continuity of thought.
- Human confirmation is required before using a Snapshot.

### NEXT ACTION

Use this Snapshot in Claude and check whether Claude can continue without asking for the full background again.

### CONTEXT NOTES

The user is a heavy AI user switching between ChatGPT, Claude, Gemini, Claude Code, Codex, Hermes Agent, and Obsidian.

The strongest pain is: every new AI window feels like starting over.
