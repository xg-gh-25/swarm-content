---
title: "小红书发布包 — Agent Harness 五大玩家深度对比"
run_id: run_p_a8h3f92c
platform: xiaohongshu
created: 2026-04-26T23:20:00+08:00
status: ready-to-publish
---

# 小红书发布包

---

## 1. 发帖文本

### Title
Agent Harness 五大玩家深度对比 — 99%的人在比错东西

### Briefing Summary (正文区)
```
你以为 Agent 竞争是比谁工具多、谁模型强？错了。

我花两个月深度研究了 AgentCore / Claude Managed / Hermes / OpenClaw / SwarmAI 五大 Agent Harness，读了源码、跑了 benchmark、翻了论文。

发现一个被 99% 的人忽略的事实：

👉 市场分三层 L1产品/L2框架/L3平台，大部分对比文章混在一起比——这是最大的误导
👉 功能表格人人都做，但 Memory 那一行才是关键
👉 AgentCore 和 Claude Managed 的 Memory 都无法导出——这不是技术限制，是战略选择
👉 CrewAI + LangChain 两大创始人同一周说了同一句话："Memory is the moat"

模型可以换（改个 endpoint），工具可以换（MCP 是标准协议），编排可以换（都是 prompt loop）。

但记忆——工作习惯、项目上下文、历史决策——是时间的结晶，不可重建。

选框架前先问：我的 Agent 记忆存在哪里？我能带走吗？

详细对比看图 👇 滑到最后有完整分析

数据来源：源码实测 + 官方文档 + ICLR 2026 论文
```

### Tags
```
#Agent #AIAgent #AgentCore #Claude #Hermes #OpenClaw #SwarmAI #记忆主权 #AI深度对比 #Agent框架 #AI工具 #大模型应用 #AI开发 #Memory #技术分析
```

---

## 2. Posters (3 张独立海报)

按顺序发布，每张可独立传播：

| # | 文件名 | 内容 | 用途 |
|---|--------|------|------|
| P1 | `poster-xiaohongshu-3x4.png` | 总览：三层分类 + 六维矩阵 + Memory 特写 + CTA | **封面图** — 信息密度高，引发保存 |
| P2 | `poster-matrix.png` | 完整对标矩阵：9 维度 × 5 玩家 + 各家最强维度 | **数据图** — 横向对比一目了然 |
| P3 | `poster-memory.png` | Memory 所有权深度：锁定/自由对比 + 行业 quotes + 锁定循环 | **观点图** — 核心论点视觉化 |

**路径：** `tracks/poster/`

---

## 3. 深度文章轮播 (8 张图片)

按顺序组成完整长文阅读体验：

| # | 文件名 | 内容 |
|---|--------|------|
| C1 | `card-1.png` | 封面：标题 + hook + "真正的战场不是功能，是记忆" |
| C2 | `card-2.png` | 三层分类 L1/L2/L3 — 认知校准 |
| C3 | `card-3.png` | L3 速评：AgentCore + Claude Managed |
| C4 | `card-4.png` | L2+L1 速评：Hermes + OpenClaw + SwarmAI |
| C5 | `card-5.png` | 六维对标矩阵 — "表格给你，但不是重点" |
| C6 | `card-6.png` | 核心观点：Memory 所有权真相 + 五家对比 |
| C7 | `card-7.png` | 行业信号：CrewAI + LangChain 创始人 quotes + 锁定循环 |
| C8 | `card-8.png` | CTA：选框架前先问这个问题 |

**路径：** `tracks/narrative/`

---

## 发布建议

### 方案 A：单笔记发布（推荐）
发 1 条笔记，图片排列：
1. P1 (封面) → P2 (矩阵) → P3 (Memory) → C1-C8 (深度轮播)
- 总计 **11 张图**，小红书上限 18 张，完全够

### 方案 B：拆分两条笔记
- **笔记 1 (海报版)：** P1 + P2 + P3，配简短文案，适合快速传播
- **笔记 2 (深度版)：** C1-C8，配完整文案，适合深度阅读+收藏

### 发布时间
- **最佳：** 周一-周三 8:00-9:00 或 20:00-22:00（技术内容读者活跃时段）
- **避开：** 周末下午（技术类内容低谷）

---

## 文件清单

```
tracks/poster/
  poster-xiaohongshu-3x4.png   (818KB)  ← P1 封面
  poster-matrix.png             (432KB)  ← P2 矩阵
  poster-memory.png             (645KB)  ← P3 Memory

tracks/narrative/
  card-1.png                    (403KB)  ← C1 封面
  card-2.png                    (433KB)  ← C2 三层分类
  card-3.png                    (433KB)  ← C3 L3 速评
  card-4.png                    (456KB)  ← C4 L2+L1 速评
  card-5.png                    (387KB)  ← C5 对标矩阵
  card-6.png                    (427KB)  ← C6 Memory 真相
  card-7.png                    (414KB)  ← C7 行业信号
  card-8.png                    (291KB)  ← C8 CTA

  cards.html                           ← 源文件（可调整后重新渲染）
  xiaohongshu.md                       ← 纯文本版本

content_package.md                     ← 内容包（核心论点+证据）
```

---

_Produced by Pollinate (run_p_a8h3f92c) · Swarm Intelligence · 2026-04-26_
