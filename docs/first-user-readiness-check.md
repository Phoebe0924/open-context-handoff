# OCH First-User Readiness Check

## Can a first-time visitor understand OCH in 30 seconds?

Yes, at the documentation level.

The README opening states the continuity problem, identifies the Context Snapshot as the solution, and keeps the protocol's narrow boundary clear. The new link near the title gives a visitor one immediate route into practical use.

This is a readiness assessment, not an observed first-time-user result.

## Can they start in 2 minutes?

Likely yes, if they already have a bounded task and access to two AI windows.

`START_HERE.md` explains the outcome and links directly to the generator prompt, receiver prompt, and exact trial. The user no longer needs to understand the repository layers before beginning.

The two-minute start has not yet been timed with an uncoached first-time visitor.

## Can they complete the 15-minute trial?

The complete path now exists:

1. choose a real handoff point
2. generate and review a Snapshot
3. send it to another AI
4. observe the first response
5. score and record the result

The trial guide supplies time boxes, preparation boundaries, observable checks, failure signs, and scoring. The result template captures the evidence.

Whether a true first-time user can finish within 15 minutes still requires a manual usability test.

## What remains weak?

- The new first-user path has not been tested by an uncoached visitor.
- The README's existing deeper **Start here** section still contains V0 wording, although the new top link bypasses that ambiguity.
- `README_CN.md` does not point to the new first-user path and still records V0 language; it was intentionally left untouched.
- The repository does not yet contain a completed result produced through this exact 15-minute guide.
- The practical reason to star the repository remains implicit: reuse the protocol, prompts, examples, and future evidence.
- Current evidence is bounded and does not establish broad effectiveness across users, task types, or AI systems.

## What should the human manually test next?

Give the repository URL to one person who has not used OCH.

Ask them to begin from the README, use a real bounded task, and complete the trial without coaching or reading release-history documents. Start a timer when they open the repository.

Have them save a copy of `tests/user-trial-result-template.md` containing:

- the reviewed Snapshot
- the receiving AI's first response
- the PASS / PARTIAL / FAIL score
- any background added outside the Snapshot
- where they hesitated or opened an unnecessary file
- total time to the recorded result

The key readiness observations are whether they can explain OCH after 30 seconds, begin the trial within 2 minutes, and save a scored result within 15 minutes.

## What is intentionally out of scope?

- CLI, code, plugins, dependencies, and package files
- agents, automation, memory, and workflow systems
- release creation
- redesigning or expanding the Snapshot v1 protocol
- rewriting the README narrative
- aligning or rewriting `README_CN.md`
- rewriting historical V0 evidence
- claiming broad validation from one or a few manual trials

## Readiness conclusion

OCH now has a direct first-time-user path from README entry to a recorded cross-AI handoff result. The next decision should come from one uncoached manual trial, not from adding more framework or implementation.
