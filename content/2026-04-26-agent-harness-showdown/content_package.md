---
title: "Agent Harness 五大玩家深度对比"
run_id: run_p_a8h3f92c
domain: ai-agents
platform: xiaohongshu
formats: [poster, narrative]
created: 2026-04-26T23:10:00+08:00
---

# Content Package

## Core Thesis

99% 的人在比 Agent 框架的功能列表，但真正决定胜负的是 Memory ownership — 谁拥有你的记忆，谁锁定你。

## Key Points

1. Agent 市场分三层：L1 产品 / L2 框架 / L3 平台 — 大部分人在同层内卷，跨层才是降维打击
2. 五大玩家各占生态位：AgentCore (L3) / Claude Managed (L3) / Hermes (L2) / OpenClaw (L1) / SwarmAI (L1)
3. Memory 架构是最被忽视的维度 — AgentCore 和 Claude Managed 都无法导出记忆
4. AgentCore session-hour 计费本质：时间越长→记忆越深→迁移成本越高→lock-in 越强
5. Hermes GEPA (ICLR 2026 oral) 是唯一学术验证的 prompt 自进化算法
6. Context Engineering 才是真护城河 — 11 文件优先级链 vs 塞进 system prompt
7. CrewAI + LangChain 创始人同时说："Memory is the moat"

## Narrative Arc

- **Hook:** "你以为 Agent 竞争是比谁工具多？错了。"
- **Setup:** 三层市场分类 — 让读者知道自己在看哪层
- **Development:** 五大玩家逐个拆解，每家一句话定位 + 核心优劣
- **Climax:** Memory 对标矩阵 — 揭示 "无法导出" 的真相
- **Resolution:** 选择框架前先问："我的记忆存在哪？我能带走吗？"

## Evidence Bank

- CrewAI João Moura (2026-04-14): "Harness is plumbing, moat is proprietary data"
- Harrison Chase (LangChain): 邮件助手被删→重建→体验断崖 = 记忆是唯一专有资产
- AgentCore Memory API 无 export — 官方文档验证
- Hermes GEPA: ICLR 2026 oral paper
- SwarmAI: 11-file context + MEMORY.md git-tracked = 完全可迁移

## Internal References

- Knowledge/Reports/2026-04-19-agentcore-harness-competitive-landscape.md
- Knowledge/Reports/2026-04-12-swarmai-vs-openclaw-vs-hermes.md
- Knowledge/Notes/2026-04-22-agentcore-managed-harness-deep-dive.md
- Knowledge/Notes/2026-04-23-agentcore-managed-harness-launched.md
- Knowledge/Library/2026-04-13-hermes-agent-orange-book-notes.md
- Knowledge/Learned/2026-04-25-agent-harnesses-are-dead.md
