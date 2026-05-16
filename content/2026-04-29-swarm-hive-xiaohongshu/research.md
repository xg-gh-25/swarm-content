# THINK: Swarm Hive 小红书宣传 Research

## Core Thesis
一条命令，把你的 AI 团队从桌面搬到云端 — 手机、平板、任何设备随时用，记忆不丢，数据归你。

## Target Audience Profile
- **Primary:** 25-35 岁技术人（后端/全栈/DevOps），对 AI 工具有热情，愿意折腾
- **Secondary:** AI 产品经理、独立开发者、技术 leader
- **Pain points:** 想要 7×24 AI 助手但被绑在电脑前；想分享给同事但不想用 SaaS；关心数据安全
- **小红书行为:** 收藏实用工具贴、关注 AI 工具测评、喜欢"手把手教程"和"真实体验"

## Differentiation Angle

### "What do we know that others don't?"
我们自己造了这个产品并真实使用：
- 完整的 provisioner 代码，一条命令部署
- 真实成本：$68/月（12hr auto-stop），不是猜的
- Memory sovereignty — 你的记忆在你的 EBS，不在别人的 SaaS
- 从 Desktop 到 Cloud 是同一份代码，不是阉割版
- CloudFront CDN 加速 + 安全隔离（Security Group 只允许 CloudFront）

### "What did others get wrong or oversimplify?"
小红书现有 AI 部署类内容的问题：
1. **大部分是 ChatGPT API wrapper** — 只有聊天，没有记忆、技能、工作流
2. **开源 LLM 部署教程** — 关注模型本身，不关注"AI 助手"的完整体验
3. **SaaS 推荐贴** — "推荐 10 个 AI 工具" 但完全不讨论数据所有权
4. **Claude Code 教程** — 聚焦写代码，不涉及"个人 AI 团队"概念
5. **缺乏真实成本分析** — 要么说"免费"（因为用的开源），要么完全不提钱

### "What angle hasn't been covered?"
**"从桌面到云端，你的 AI 助手进化之路"** — 没人讲过"先在桌面上培养你的 AI 助手，然后无缝搬到云端"这个故事。因为没人有这个产品。

## Internal Asset Manifest
- `Knowledge/Designs/2026-04-28-hive-mvp-design.md` — 完整架构、成本模型、安全设计
- `Knowledge/Designs/2026-04-28-hive-e2e-flow-design.md` — 部署全流程、API 设计
- `Knowledge/Designs/2026-04-28-desktop-update-gaps-design.md` — Desktop↔Hive 兼容性
- `.context/MEMORY.md` — Memory sovereignty 是第一原则 (KD07)
- DailyActivity 2026-04-28, 2026-04-29 — 真实部署记录

## Competitive Content Analysis (小红书)

| # | Content Type | Typical Title | Weakness |
|---|-------------|---------------|----------|
| 1 | ChatGPT API 部署 | "手把手教你部署私有 ChatGPT" | 只有聊天，无记忆/技能/工作流 |
| 2 | 开源 LLM 教程 | "本地部署 Llama3，比 GPT 还强" | 关注模型不关注助手体验 |
| 3 | AI 工具推荐 | "2026 最强 AI 工具合集" | 表面罗列，不深入 |
| 4 | Claude Code | "Claude Code 使用体验分享" | 写代码工具，不是个人助手 |
| 5 | AI Agent 概念 | "什么是 AI Agent？一文搞懂" | 概念科普，无实际产品 |

## Recommended Narrative Arc
1. **Hook:** "你的 AI 助手，能不能随时随地用？" — 戳中痛点
2. **Problem:** 桌面 AI 助手的局限 — 绑在电脑前，出门就断联
3. **Solution reveal:** Swarm Hive — 一条命令，桌面搬到云端
4. **Proof:** 真实架构 + 真实成本 + 真实截图
5. **Differentiator:** 数据归你，记忆归你，不是 SaaS
6. **CTA:** 开源地址 + 关注后续教程
