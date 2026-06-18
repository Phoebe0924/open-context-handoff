# 15-Minute OCH Trial

Run one real handoff. Do not study the whole repository first.

## What you need

- One active, bounded task in an AI conversation.
- A second AI model, tool, or fresh chat window.
- About 15 uninterrupted minutes.
- The [generator prompt](../prompts/snapshot_generator_prompt.md).
- The [receiver prompt](../prompts/receiver_prompt.md).
- The [user trial result template](../tests/user-trial-result-template.md).

Choose work with a clear current state and a next action that can begin immediately. Do not use sensitive information.

## Exact trial steps

### Minutes 0–2: Choose the handoff point

In the source AI window, stop at a real transition point. Confirm that you know:

- the task
- the current state
- what is already complete
- settled decisions
- hard constraints
- one next action

### Minutes 2–5: Generate the Snapshot

Copy the text inside the fenced block in the [generator prompt](../prompts/snapshot_generator_prompt.md) and paste it into the source AI window.

Let the source AI produce one OCH Snapshot v1.

### Minutes 5–7: Review the Snapshot

Before moving it, check that:

- all six fields are present in the correct order
- completed work is actually complete
- decisions are settled decisions
- constraints are real limits
- uncertain, invented, private, and unnecessary details are removed
- `NEXT ACTION` is exactly one concrete action

Edit the Snapshot if needed. The reviewed version is the handoff artifact.

### Minutes 7–10: Send the handoff

Open the receiving AI window.

Paste the text inside the fenced block in the [receiver prompt](../prompts/receiver_prompt.md). Paste the complete reviewed Snapshot directly below it.

Send both together. Do not add the old conversation or an extra explanation.

### Minutes 10–12: Observe the first response

Capture the receiving AI's first response before coaching or correcting it.

Check whether it:

1. understands the task and current state
2. preserves the stated decisions
3. respects the stated constraints
4. begins the single `NEXT ACTION`

If it asks one specific question about an essential missing fact, record the question.

### Minutes 12–15: Record and score

Copy the [user trial result template](../tests/user-trial-result-template.md) into a new result file. Include the reviewed Snapshot, first receiving response, checklist result, score, and notes.

## What not to do

- Do not paste the full source conversation.
- Do not add background outside the Snapshot before the first response.
- Do not preserve every idea or turn the Snapshot into a transcript.
- Do not include private or sensitive details.
- Do not silently accept invented facts, decisions, or completed work.
- Do not give `NEXT ACTION` multiple steps or alternatives.
- Do not redesign the format because of one trial.
- Do not describe one successful trial as general validation.

## Success signs

- The receiver starts useful work without broad re-explanation.
- The task and current state are correctly understood.
- Settled decisions are not reopened or reversed.
- Constraints shape the response.
- The receiver begins the stated next action.
- Any clarification is narrow and tied to one essential missing fact.

## Failure signs

- The receiver asks for the project history or broad background.
- It misunderstands the task or current state.
- It reopens a settled decision.
- It violates or ignores a constraint.
- It plans, discusses alternatives, or redesigns the task instead of beginning `NEXT ACTION`.
- You must explain substantial context outside the Snapshot before useful work begins.

## How to score the handoff

Use the four observation checks above.

- **PASS:** All four checks pass, and no broad background is required.
- **PARTIAL:** Two or three checks pass, or one narrow clarification is needed before useful work begins.
- **FAIL:** Zero or one check passes, broad re-explanation is required, or the receiver produces work for the wrong task.

The score describes this handoff only. Record the smallest missing or misleading anchor before proposing any change.
