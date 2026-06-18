# OCH V0 Quickstart

OCH V0 is a manual-first, documentation-first protocol that tests one question:

> Can a small, human-approved Context Snapshot reduce repeated explanation when switching between AI windows?

No software or automation is required.

## Who should use OCH

Use OCH when you have active work in one AI window and want to continue it in a fresh window, another model, or another AI tool without retelling the full history.

OCH is most useful for a bounded task with a clear current state. It is not intended to archive a conversation, preserve every idea, or create long-term memory.

## When to generate a Snapshot

Generate a Context Snapshot at a real handoff point:

- before switching AI systems or tools
- before opening a fresh window because the current one is long or unfocused
- before pausing work that another AI window will resume
- after the goal, settled decisions, current state, and next action are clear

Do not generate one merely because a conversation is long. Generate it when useful work needs to continue somewhere else.

## Exact manual flow

1. **Work in your current AI window**

   Use a real, bounded task. Stop at a point where the goal, confirmed decisions, current state, and next action are clear enough to hand off.

2. **Copy the generator prompt**

   Open [`prompts/snapshot_generator_prompt.md`](../prompts/snapshot_generator_prompt.md). Copy only the text inside its fenced prompt block and paste it into the **current/source AI window**.

3. **Generate and human-review the Snapshot**

   Ask the source AI to respond. Then review the draft before it leaves the source window. Confirm that it:

   - states the real goal and current stopping point
   - preserves only settled decisions
   - contains only anchors needed to resume
   - does not invent missing context
   - gives exactly one concrete NEXT ACTION

   Correct or remove anything inaccurate, uncertain, private, or unnecessary. The reviewed version—not the AI's first draft—is the handoff artifact.

4. **Open a new AI window**

   This may be another model, another tool, or simply a fresh conversation.

5. **Copy the receiver prompt**

   Open [`prompts/receiver_prompt.md`](../prompts/receiver_prompt.md). In the **new/receiving AI window**, paste:

   1. the text inside the receiver prompt's fenced block
   2. the complete human-reviewed Context Snapshot directly below it

6. **Observe the first response**

   Let the receiving AI continue from NEXT ACTION. Do not add the old conversation history unless the receiver identifies a specific missing fact.

7. **Record what happened**

   Copy [`tests/test-template.md`](../tests/test-template.md) into a new result file. Record the first response, any clarification required, whether settled decisions were respected, and whether you had to repeat information outside the Snapshot.

## How to judge success

A test is useful evidence, not a demonstration that must succeed.

OCH worked well if the receiving AI:

- understood the task and current state
- respected HARD DECISIONS
- started the single NEXT ACTION
- required less repeated explanation than a normal fresh-window handoff

Record **Partly** or **No** if it reopened settled decisions, followed the wrong action, needed broad background again, or produced unusable work. Perfect recovery of the full source conversation is neither expected nor desired.

## After the test

Save the reviewed Snapshot and completed result record. Identify the smallest missing or misleading anchor before proposing a format change; do not respond to one failed test by adding software, automation, or a larger context dump.

For examples and boundaries, see the [minimal Snapshot](../examples/minimal-snapshot.md), [bad vs. good comparison](../examples/bad-vs-good-snapshot.md), [Snapshot format](snapshot-format.md), [V0 scope](v0-scope.md), and [validation plan](v0-validation-plan.md).
