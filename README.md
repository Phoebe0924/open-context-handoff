# OCH — Open Context Handoff

New here? Start with [START_HERE.md](START_HERE.md).

> You are not losing context.  
> You are losing continuity of thought.

OCH is a small, human-readable Snapshot format for carrying working context from one AI system to another.

---

## The shift

We no longer work with a single AI system.

We constantly move between:

ChatGPT · Claude · Gemini · Cursor · Claude Code · Agents

But something breaks every time we switch:

> Our thinking does not carry over.

Only fragments do.

---

## The invisible problem

Every switch forces you to:

- re-explain what you're doing
- rebuild your decisions
- re-establish what is true
- reconstruct the same narrative

Meanwhile:

AI quietly rewrites your story in its own way.

Sometimes correct.  
Sometimes confidently wrong.

You are no longer continuing your work.

You are restarting your thinking.

---

## The real divide

There are two types of AI users:

### 1. Restart thinkers

They treat every new AI window as a blank slate.

### 2. Continuity thinkers

They preserve context across systems and continue from where they stopped.

---

## OCH is built for the second group

Not to store memory.  
Not to automate workflows.  
Not to build agents.

But to solve one thing:

> Make thinking portable across AI systems.

---

## What OCH does

OCH generates a **Context Snapshot**:

A small, human-readable artifact containing:

- what you are working on
- what you have decided
- what you explicitly rejected
- what you should do next

You can carry it across:

- AI chat windows
- different models
- coding agents (Cursor / Claude Code)
- personal notes

And continue instantly.

No re-explaining.

---

## Start here

For the current V1 first-user path:

1. [Start with the practical guide](START_HERE.md)
2. [Review the Snapshot v1 format](docs/snapshot-format.md)
3. [Copy the Snapshot generator prompt](prompts/snapshot_generator_prompt.md)
4. [Copy the receiver prompt](prompts/receiver_prompt.md)
5. [Record the trial result](tests/user-trial-result-template.md)

---

## Quick manual testing

- [Quick receiver prompt](prompts/quick-receiver-prompt.md)
- [Quick Snapshot template](prompts/quick-snapshot-template.md)
- [7-run validation log](tests/7-run-validation-log.md)

---

## How it works (V0)

1. End a session while thinking is still coherent  
2. Generate a Context Snapshot  
3. Review and approve it
4. Paste into another AI system  
5. Continue from NEXT ACTION  

---

## Core principle

> AI drafts.  
> Humans decide.  
> Context belongs to the user.

---

## Why this matters

AI systems are becoming more powerful.

But human thinking is becoming more fragmented.

We optimize models.

But we lose continuity.

OCH is a small attempt to fix one thing:

> Keep thinking alive across system boundaries.

---

## Not trying to solve

OCH is intentionally narrow.

It is NOT:

- a memory system
- an AI agent
- an automation tool
- a knowledge base

---

## It only solves this

> How do you continue thinking without restarting yourself every time you switch systems?

---

## Philosophy

Context does not belong to platforms.

It belongs to the person thinking.
