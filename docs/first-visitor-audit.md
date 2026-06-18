# OCH First-Visitor Audit

## Audit question

Can a first-time GitHub visitor understand OCH quickly and complete one real cross-AI handoff without reconstructing the repository's history?

## Can a new visitor understand OCH in 30 seconds?

Mostly.

The top of `README.md` clearly names the problem: switching AI systems breaks continuity of thought. It also explains the narrow solution—a small, human-readable Context Snapshot—and distinguishes OCH from memory, agents, and automation.

The likely gap is practical confidence. A visitor can understand the idea, but the first screen does not immediately show the shortest current path, the 15-minute commitment, or the concrete evidence they will produce. The philosophical reason to care is strong; the reason to star and return to the repository is less explicit.

## Can they find where to start?

Partly.

`README.md` has a visible **Start here** section, but it presents five separate links and calls the first one a “V0 quickstart” even though the linked document is the current V1 quickstart. A new visitor must decide whether to read the quickstart, protocol specification, prompts, examples, or test template first.

The repository has the required materials, but not yet one obvious entry point that says: start here, spend 15 minutes, perform these four actions, and record this result.

## Can they complete a first handoff without reading the whole repo?

Yes, with avoidable navigation work.

`docs/quickstart.md`, the generator prompt, the receiver prompt, and the result template contain enough information to run a manual handoff. The user does not need the release documents or historical V0 records.

However, the current path requires opening several files and translating general guidance into a trial procedure. There is no single time-boxed checklist, explicit PASS / PARTIAL / FAIL scoring rule, or troubleshooting page for a failed first attempt.

## Where does the user journey break?

1. **Entry-point ambiguity:** the README links to a “V0 quickstart” that is now titled V1.
2. **Too many first choices:** the visitor is offered a guide, two prompts, examples, a protocol specification, scope history, and a result template before being told the minimum path.
3. **No time-boxed trial:** the manual flow is accurate but does not frame one bounded 15-minute test.
4. **No preparation boundary:** a new user may choose a vague task, paste too much history, or edit the Snapshot until it becomes a transcript.
5. **No simple score:** the existing template is useful but does not reduce the first result to PASS, PARTIAL, or FAIL.
6. **No recovery path:** common failures are not mapped to likely causes and small fixes.
7. **Version noise:** V0 language in the narrative layer can make a first-time visitor uncertain about which format is current.

## What should remain untouched because it carries the project soul?

- The opening narrative in `README.md`, especially the distinction between losing context and losing continuity of thought.
- The framing of “restart thinkers” and “continuity thinkers.”
- The narrow product boundary: OCH is not memory, automation, an agent, or a knowledge base.
- The core principle: AI drafts, humans decide, and context belongs to the user.
- The closing philosophy that context belongs to the person thinking.
- `README_CN.md` as the existing Chinese narrative record unless a separate human-approved alignment task is created.
- `docs/snapshot-format.md` as the canonical V1 protocol contract.
- Historical V0 artifacts and test evidence as records of what was actually tried.

## Minimal readiness direction

Add a short root-level start guide, one exact 15-minute trial, one result template with a clear score, and one troubleshooting guide. Then connect the README to that path with a single link while preserving its narrative.
