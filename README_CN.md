# OCH — Open Context Handoff

## 1. 问题

我们不断在 ChatGPT、Claude、Gemini、Cursor、Claude Code 等 AI 系统之间切换。每次切换都会打断连续性：用户必须重新解释任务、当前状态、决定、约束和下一步。

OCH 的目标是让工作继续，而不是重建整段对话。

## 2. 核心理念

即使上下文在不同 AI 系统之间断裂，思考也应该可以携带。

OCH 把继续工作所需的最少上下文整理为一份 **Context Snapshot**。用户在交接给另一个 AI 前拥有并审核这份 Snapshot。

## 3. OCH Snapshot 规范（严格）

### OCH Snapshot v1

```markdown
## OCH Snapshot v1

WHAT WE ARE DOING:
[只写一句。]

CURRENT STATE:
[当前阶段或状态。]

COMPLETED:
- [已完成事项。]

DECISIONS:
- [不可重新讨论的决定。]

CONSTRAINTS:
- [必须遵守的硬约束。]

NEXT ACTION:
- [唯一、具体、可执行的步骤。]
```

规则：

- 每个字段只出现一次，并严格保持以上顺序。
- 不得增加字段。
- `WHAT WE ARE DOING` 只能写一句。
- `COMPLETED`、`DECISIONS` 和 `CONSTRAINTS` 只能使用项目符号；没有内容时写 `- None.`。
- `NEXT ACTION` 必须只有一个可执行步骤，并产生可观察结果。
- `NEXT ACTION` 不得包含规划、多步骤、备选方案或抽象思考。
- 交接前必须由人类审核并确认 Snapshot。

## 4. 示例

ChatGPT 生成：

```markdown
## OCH Snapshot v1

WHAT WE ARE DOING:
准备一份单页社区花园提案。

CURRENT STATE:
提纲已经完成，但开头段落尚未撰写。

COMPLETED:
- 已确认受众和单页限制。

DECISIONS:
- 聚焦社区食物获取问题。

CONSTRAINTS:
- 不包含活动策划。

NEXT ACTION:
- 根据提纲起草一段 100 字的开头。
```

Claude 收到经人工审核的 Snapshot 后，直接起草开头，无需询问之前的完整对话。

## 5. 状态

- V0 已验证
- V1 正在细化
