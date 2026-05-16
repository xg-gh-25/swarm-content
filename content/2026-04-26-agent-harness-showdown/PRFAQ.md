# PRESS RELEASE

**Headline:** Agent Harness 五大玩家对比 — 99% 的人在比错东西

**Problem:** Agent Harness 市场爆炸式增长（AWS AgentCore、Claude Managed Agents、Hermes、OpenClaw、SwarmAI…），开发者面对一堆功能列表和 Star 数无从选择。更糟的是，大多数对比文只看表面（模型支持、工具数量），完全忽视了最关键的维度。

**Solution:** 一篇基于实际构建和深度研究的全景对比，按三层分类（L1 Product / L2 Framework / L3 Platform）定位 5 家玩家，从 Memory 所有权这个真正决定壁垒的维度切入，帮读者做出清醒的技术选型。

**Real Example:** AgentCore Memory API 故意不提供 export 接口 — session-hour 计费让记忆越深迁移成本越高。Claude Managed Agents 的 Memory 同样被 Anthropic 托管，无法导出。CrewAI 创始人 Moura 直言 "harness is plumbing, moat is proprietary data"。LangChain 创始人 Chase 分享真实案例：邮件助手被误删，同模板重建后体验断崖下降 — 因为记忆丢了。

**Quote:** "模型会换、框架会换，但记忆一旦积累就无法替代。灵魂拷问：你的 Agent 记忆存在哪里？你能带走吗？"

# FAQ

**Q: 这 5 家不在同一个层级，怎么比？**
A: 没错，它们确实分属三层（L3 Platform: AgentCore/Claude Managed, L2 Framework: Hermes, L1 Product: OpenClaw/SwarmAI）。但 Memory ownership 是跨层级的维度 — 无论你在哪层，谁控制记忆谁就控制壁垒。

**Q: Memory 真有那么重要吗？**
A: 两大框架创始人（CrewAI Moura + LangChain Chase）同时独立验证了这个判断。模型可以一行代码切换，但迁移 3 个月的工作记忆？几乎不可能。

**Q: 谁最适合普通开发者？**
A: 看你的需求层级：要快速 POC → OpenClaw/Hermes；要企业级隔离 → AgentCore；要个人 AI 中枢、记忆完全自有 → SwarmAI。
