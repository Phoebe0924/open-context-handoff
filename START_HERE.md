# Start Here

OCH helps you continue real work in another AI window without retelling the full conversation.

Use it when you are switching models, tools, or chat windows and already know the task, current state, settled decisions, constraints, and next action.

In 15 minutes, you will create one human-reviewed Snapshot, send it to another AI, and record whether the handoff worked.

## Step 1: Generate a Snapshot

In your current AI window, use the [Snapshot generator prompt](prompts/snapshot_generator_prompt.md) on a real, bounded task.

## Step 2: Review the Snapshot

Check that it is accurate, contains no sensitive or invented details, and gives exactly one executable `NEXT ACTION`. You—not the AI—approve the handoff.

## Step 3: Send it to another AI

Open a fresh AI window. Paste the [receiver prompt](prompts/receiver_prompt.md), then paste the reviewed Snapshot directly below it.

## Step 4: Check whether it worked

Observe the receiving AI's first response before adding more background. Record whether it understood the task, preserved decisions and constraints, and began the next action.

Follow the exact procedure and scoring rules in the [15-minute OCH trial](docs/15-minute-trial.md).
