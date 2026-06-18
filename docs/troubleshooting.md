# OCH Troubleshooting

Use this after a trial produces a weak handoff. Fix the smallest observed problem, then run another bounded trial.

## Receiving AI asks for more background

**Symptom**

The receiving AI asks for the project history, prior conversation, or a broad explanation before doing useful work.

**Likely cause**

One essential anchor is missing, the task is too broad, or the receiver prompt was not sent with the reviewed Snapshot.

**Fix**

Ask which single fact is essential. Add that fact to the appropriate Snapshot field only if it is necessary and verifiable. Do not paste the full conversation. If the question is broad, narrow the task and make `NEXT ACTION` more specific before retrying.

## Snapshot is too vague

**Symptom**

The receiver gives generic advice, guesses the current state, or cannot tell what concrete work is underway.

**Likely cause**

`WHAT WE ARE DOING` names a topic instead of a task, `CURRENT STATE` lacks a real status, or the fields use abstractions that are not observable.

**Fix**

Replace generic language with task-specific nouns and current facts. State what artifact or outcome is being worked on, where it stands now, and only the anchors needed for the next action. Keep the Snapshot concise; specificity does not require more history.

## NEXT ACTION is not executable

**Symptom**

The receiver discusses plans, offers options, asks what to do next, or performs several unrelated steps.

**Likely cause**

`NEXT ACTION` contains abstract planning, multiple actions, alternatives, or no observable output.

**Fix**

Rewrite it as one action with a clear verb and object. Name an observable result, such as “Draft a 100-word opening paragraph” or “Review `START_HERE.md` for broken links.” Remove “and,” optional branches, and later steps.

## Decisions and constraints are mixed

**Symptom**

The receiver treats a preference as a hard rule, silently reverses a settled choice, or cannot tell what is negotiable.

**Likely cause**

`DECISIONS` and `CONSTRAINTS` contain the same kind of information or combine several claims in one bullet.

**Fix**

Put settled choices in `DECISIONS`: choices that should not be silently reopened. Put hard limits and rules in `CONSTRAINTS`: boundaries the work must obey. Split mixed bullets and remove anything that is only a suggestion.

## AI redesigns the task

**Symptom**

The receiving AI proposes a new architecture, redefines the goal, reopens settled choices, or produces a plan instead of continuing the handoff.

**Likely cause**

The receiver prompt was omitted, the decisions or constraints are incomplete, or `NEXT ACTION` leaves room for strategy work instead of execution.

**Fix**

Send the receiver prompt and Snapshot together. Confirm that settled direction is explicit in `DECISIONS`, boundaries are explicit in `CONSTRAINTS`, and `NEXT ACTION` requests execution rather than ideation. Record any redesign as a failed checklist item.

## User explains too much outside the Snapshot

**Symptom**

The user adds a long introduction, old conversation excerpts, or corrective context before observing the receiver's first response.

**Likely cause**

The user does not trust the Snapshot yet, is trying to guarantee success, or has not chosen a bounded task.

**Fix**

Run the trial again with a smaller task. Send only the receiver prompt and reviewed Snapshot, then wait for the first response. Add outside context only when the receiver asks one specific essential question, and record exactly what was added.

## After a weak result

Score the run using the [15-minute trial](15-minute-trial.md) and record it with the [user trial result template](../tests/user-trial-result-template.md). One weak result is evidence about that handoff, not proof that the protocol or format must expand.
