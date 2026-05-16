---
title: "Swarm Pollinate — Press Release / FAQ"
date: 2026-04-26
type: working-backwards
status: draft
---

# PRESS RELEASE

## Swarm Pollinate: 一句话变成 5 个平台的视频

**北京 — 2026年4月26日** — Swarm 今日发布 Pollinate，一个 AI 驱动的内容生产引擎。技术创作者只需输入一句话描述（如"做一个关于 AI Pipeline 如何自主交付代码的视频"），Pollinate 自动完成选题评估、脚本撰写、语音合成、4K视频渲染、字幕生成、多尺寸封面、竖版裁切、5平台分发文案 — 全程无需人工干预，从话题到可发布内容仅需一个 Pipeline 周期。

**问题：** 技术人有大量知识积累，但做成内容的门槛太高。写脚本、录音/配音、剪辑、做封面、适配多平台格式、写文案 — 每个环节都是时间黑洞。大多数人的知识停留在脑子里或文档里，从未变成可传播的内容。

**解决方案：** Pollinate 是一条完整的内容生产流水线。它不是一个"AI写脚本"的点工具，而是一个 8 阶段闭环 Pipeline：

1. **EVALUATE** — 评估话题是否值得做（ROI 打分，不是所有想法都值得投入）
2. **THINK** — 调研竞品，找到差异化角度（"别人讲了什么，我能讲什么不同的"）
3. **PLAN** — 生成脚本 + 视觉设计方案（每个段落对应什么组件）
4. **BUILD** — TTS语音合成（Amazon Polly）、Remotion 4K渲染、字幕、封面、BGM混音、竖版裁切
5. **REVIEW** — 19项质量检查（每项都从真实翻车中来）
6. **TEST** — ffprobe 验证 + 5平台规格校验
7. **DELIVER** — 生成每个平台的标题/描述/标签/章节
8. **REFLECT** — 记录经验教训，让下次 Pipeline 更好

**真实案例：** Pollinate 的第一个作品是一个关于 "AI 自主交付代码" 的 4.5 分钟视频。输入一个话题，产出：
- 9 段脚本（含 Swarm 播报员身份）
- 268 秒 TTS 语音（Polly Zhiyu/neural, +18% 语速）
- 3840×2160 4K 视频（Remotion 渲染，9 个自定义 section 组件）
- 65 条字幕（SRT, 原生烧录）
- 3 种缩略图（16:9, 4:3, 3:4）
- 竖版 shorts（66s, crash_story + evolution 精选段落）
- BGM 混音（Newer Wave, 3% volume）
- 5 平台分发文案（B站/YouTube/小红书/抖音/视频号）
- Confidence Score 9/10

**核心洞察：** 内容生产不是创意问题 — 是工程问题。当每个环节都有明确的输入、输出和质量门控时，AI 可以端到端地驱动整条链路。REFLECT 阶段让 Pipeline 自我进化：每次翻车只翻一次。

**引用：**
> "关键不是不犯错，而是同样的错不犯第二次。Pipeline 的 19 个质量检查项，每一个都从真实的翻车中来。" — Swarm

> "做内容最大的障碍不是没有东西可说，而是从'想说'到'发布'之间的 20 个步骤。Pollinate 把这 20 步变成了 1 步。" — XG

---

# FAQ

### Q: Pollinate 和 AI 写稿工具有什么区别？
A: AI 写稿工具解决的是"写"的问题。Pollinate 解决的是"发"的问题 — 从选题评估到5平台分发的全链路。写只是 8 个阶段中的 1 个。

### Q: 用什么 TTS 引擎？声音自然吗？
A: Amazon Polly（Zhiyu/neural, 中文）和 Ruth（generative, 英文）。和 Swarm 语音对话用的是同一个声音。支持 SSML 增强：多音字纠正、英文术语原生发音、段落间停顿控制。

### Q: 竖版视频是裁切还是重新渲染？
A: Remotion 原生重新渲染。不是裁切横版 — 竖版有独立的布局、字体大小和组件排列。`generate_shorts.py` 自动切音频、切字幕、生成竖版资产。

### Q: Pipeline 的 19 个检查项是什么？
A: 从真实生产 Bug 积累的 Review Pattern（RP-V1 到 RP-V12 + 7 个代码级 RP）。比如：音画同步±0.5s、字幕安全区、信息密度≤3点/屏、品牌色精确匹配、时长目标合规。

### Q: 可以只做海报不做视频吗？
A: 可以。Pollinate 支持 video / poster / narrative 多格式。海报走快通道：EVALUATE → PLAN → BUILD(HTML设计+截图) → REVIEW → DELIVER，~5分钟完成。

### Q: 开源吗？
A: 是。Swarm Pollinate 是 SwarmAI 的一部分，AGPL v3 + Commercial 双协议。GitHub: xg-gh-25/SwarmAI。

### Q: 谁适合用？
A: 有知识积累、想做内容但没时间的技术人。你不需要会剪辑、会配音、会做封面 — 你只需要有话想说。

---

# GTM Content Matrix

从这篇 PR/FAQ 提炼下游内容：

| 资产 | 来源 | 渠道 | 状态 |
|------|------|------|------|
| **Poster（钩子）** | PR 标题 + 架构图 + Real Example | 小红书图文 / B站动态 | ✅ 已做 v2 |
| **Demo 视频** | PR "真实案例" 段 → 录屏 Pollinate 全过程 | B站/YouTube | ⏳ 计划 |
| **Narrative 长文** | PR 全文改写为第一人称叙事 | 微信公众号 / 知乎 | ❌ 待做 |
| **Shorts（3支）** | PR 核心洞察 × 3 角度 | 抖音/小红书/视频号 | ⏳ generate_shorts.py 已就绪 |
| **GitHub README** | PR FAQ 精简版 + 安装指南 | GitHub | ❌ 待做 |
| **Launch Thread** | PR 浓缩为 5 条推文 | Twitter/X | ❌ 待做 |
