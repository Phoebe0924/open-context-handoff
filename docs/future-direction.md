# OCH Future Directions

These are observations for later research, not V0 commitments. They should not change the current manual validation protocol.

## 1. In-session topic drift detection

A long AI session can move away from its active task without either participant noticing. A future OCH direction could examine how to make that drift visible while preserving the user's right to change direction intentionally.

## 2. Unlanded commitment tracking

Conversations often contain promises, decisions, or intended actions that never become completed work. It may be useful to distinguish these open commitments from settled decisions and general discussion.

## 3. Active interruption when topic drifts from open todos

Some users may benefit from an explicit interruption when a new topic displaces an unfinished action. Any such interruption would need to remain supportive and overridable rather than treating every change of attention as an error.

## 4. Multi-Snapshot per conversation

A single conversation may contain several independent workstreams that should not share one overloaded Snapshot. Multiple small Snapshots could preserve cleaner boundaries, but they would also require clear human choices about which one is active.

## 5. Cross-model Brief format

Not every handoff asks another model to continue the same work. A Cross-model Brief could invite a different perspective, critique, or independent judgment while preserving the minimum shared facts.

## 6. Agent Work Order format

Coding agents such as Claude Code or Codex may need a more execution-specific handoff than a general Context Snapshot. An Agent Work Order could emphasize repository scope, constraints, evidence, and a bounded deliverable without turning OCH V0 into an agent workflow.

## 7. Context translator concept

The same source context may need different packaging for a strategist, editor, coding agent, or fresh chat model. A context translator could explore receiver-aware selection of anchors while keeping the human in control of what is sent.
