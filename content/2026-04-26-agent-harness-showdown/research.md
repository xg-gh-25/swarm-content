# Research: Agent Harness 五大玩家深度对比

## Core Thesis

Agent Harness 正在加速 commodity 化，真正的壁垒不是技术架构而是 Memory ownership — 谁拥有用户记忆，谁锁定用户。

## Target Audience

AI 开发者、技术决策者、AI 产品经理。使用或评估 Agent 框架的人。对 AI 行业趋势敏感，能理解架构图和对比表。小红书浏览习惯：快速扫读 + 收藏深度内容。

## Differentiation Angle

- **What we know that others don't:** 同时作为 SwarmAI 构建者和 4 家竞品深度研究者，有一手数据 + 架构体验
- **What others get wrong:** 大多数对比文只比功能清单，没有抓住 Memory 才是真战场
- **What angle hasn't been covered:** CrewAI + LangChain 创始人同时验证 Memory = moat，行业共识正在形成

## Internal Asset Manifest

| File | Extract |
|------|---------|
| `Learned/2026-04-25-agent-harnesses-are-dead.md` | Moura 全文分析: harness is plumbing, entangled software is moat |
| `Reports/2026-04-19-agentcore-harness-competitive-landscape.md` | 三层分类 (L1/L2/L3) + Memory 对比矩阵 + 行业演进路线图 |
| `Reports/2026-04-12-swarmai-vs-openclaw-vs-hermes.md` | 详细功能对比数据 (Memory/Self-Evolution/Context Engineering) |
| `Notes/2026-04-22-agentcore-managed-harness-deep-dive.md` | AgentCore 技术架构 + microVM + Memory API (no export) |
| `MEMORY.md LL14` | Harness 层竞争本质是 Memory ownership |
| `MEMORY.md KD07` | Memory sovereignty is a first principle |

## Narrative Arc

Hook → 一句话抛出矛盾: "Agent 框架满天飞，但 99% 的人在比错东西"
Setup → 三层分类让读者瞬间建立框架
Development → 5 家对比 (架构 + Memory + 自进化 + 模型中立 + 适用场景)
Climax → Memory is the moat — 两大创始人同时验证 + AgentCore 故意不做 export
Resolution → 灵魂拷问: 你的 Agent 记忆存在哪里？你能带走吗？
