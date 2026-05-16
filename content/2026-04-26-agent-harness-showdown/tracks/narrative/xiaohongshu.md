---
track: narrative
platform: xiaohongshu
run_id: run_p_a8h3f92c
word_count: ~1400
language: zh-CN
---

# Agent Harness 五大玩家深度对比 — 99%的人在比错东西

你以为 Agent 竞争是比谁工具多、谁模型强？错了。

我花了两个月深度研究了市场上五个最有代表性的 Agent 平台/框架/产品，读了源码、跑了 benchmark、翻了论文。结论只有一句话：**真正的战场不是功能，是记忆。**

---

## 先搞清楚：你看的是哪一层？

市场上叫 "Agent" 的东西分属三个完全不同的层级，大部分对比文章把它们混在一起比，这是最大的误导：

**L3 平台层** — 你定义 agent，我管 infra + runtime + memory + observability
→ AgentCore Harness, Claude Managed Agents

**L2 框架层** — 你管 infra，我给编排 + memory + tool 抽象
→ Hermes, LangGraph, CrewAI, DeerFlow 2.0

**L1 产品层** — 开箱即用，终端用户直接交互
→ Claude Code, OpenClaw, SwarmAI, Operator

同层竞争是内卷，跨层是降维打击。L3 的客户是 L2 和 L1。

---

## 五家速评：一句话定位

**AgentCore (AWS, L3)** — "Any model, any framework, your VPC." 最开放的平台层，microVM 隔离，支持 Bedrock + OpenAI + Gemini。杀手锏是企业级安全 (VPC 部署 + X-Ray 审计)。

**Claude Managed Agents (Anthropic, L3)** — "Best Claude experience, zero ops." 最流畅的开发体验，但只能用 Claude。Notion 和 Rakuten 已在用。

**Hermes (MIT, L2)** — 唯一有学术验证的自进化框架。GEPA 算法发了 ICLR 2026 oral，用遗传算法在 Pareto front 上优化 prompt。17 个 channel (Telegram/Discord/WhatsApp...)，agentskills.io 生态。

**OpenClaw (L1)** — 社区驱动的通用 Agent，MCP 生态 + 54 denied-command 安全模式。优势在社区活跃度和政策推动。

**SwarmAI (L1)** — 个人 AI command center。11 文件 context engineering + 61 skills + memory sovereignty。设计哲学：记忆属于用户，不属于平台。

---

## 功能对比？表格给你，但不是重点

| 维度 | AgentCore | Claude Managed | Hermes | OpenClaw | SwarmAI |
|------|-----------|---------------|--------|----------|---------|
| 自进化 | ❌ | ❌ | GEPA (ICLR) | ❌ | 4-phase pipeline |
| Memory 分层 | 托管 API | Append log | 3 层 (2.2K cap) | Vector | 4 层 + 蒸馏 |
| Context 管理 | 基础 | 基础 | 2 文件 | 配置 | 11 文件 P0-P10 |
| Skills 数量 | N/A | N/A | Marketplace | 54+ | 61 |
| 多平台 | API | API | 17 个 | Desktop | Desktop+Slack |
| 安全 | VPC+X-Ray | Sandbox | 6 后端隔离 | OS sandbox | 3-tier+MemoryGuard |

好了，表格看完了。现在说重点。

---

## 真正的战场：你的记忆存在哪？

翻到上面的表格，看 Memory 那一行。注意一个细节：

- AgentCore Memory API → **无法导出**
- Claude Managed → **无法导出**
- Hermes → 本地，可迁移，但 2.2K chars 上限
- OpenClaw → 本地 vector，可迁移
- SwarmAI → 本地 git，完全可迁移

为什么这很重要？

**记忆是 Agent 唯一不可替代的资产。** 模型可以换（改个 endpoint），工具可以换（MCP 是标准协议），编排可以换（都是 prompt loop）。但记忆——你和 Agent 积累的工作习惯、项目上下文、个人偏好、历史决策——这些是时间的结晶，不可重建。

Harrison Chase (LangChain 创始人) 讲了一个真实案例：他的邮件助手被意外删除，用同样的模板重建，体验断崖式下降。不是模型变差了，是记忆没了。

João Moura (CrewAI 创始人) 同一周写了篇博客："Harness is plumbing, moat is proprietary data." 翻译：管道谁都能建，数据才是护城河。

两大框架创始人同时说同一件事 = 行业共识正在形成。

---

## AgentCore 的计费逻辑：一个精妙的锁定循环

AgentCore 按 session-hour 计费。看起来很合理对吧？

但想想底层逻辑：时间越长 → 记忆越深 → Agent 越好用 → 你越离不开 → 迁移成本越高 → lock-in 越强。

而且 Memory API 故意不提供 export。这不是技术限制，是战略选择。

Claude Managed 也一样——Append-only session log，没有导出。

---

## 所以选框架之前，先问自己一个问题

不是 "谁工具多"，不是 "谁模型强"，不是 "谁星标高"。

**"我的 Agent 记忆存在哪里？我能带走吗？"**

如果答案是 "在云端，不能导出" — 你在用别人的记忆。
如果答案是 "在本地，git 管理" — 记忆属于你。

模型会迭代，框架会洗牌，只有记忆是真正的复利。

---

#Agent #AI #AgentCore #Claude #Hermes #OpenClaw #SwarmAI #记忆主权 #AIAgent #深度对比
