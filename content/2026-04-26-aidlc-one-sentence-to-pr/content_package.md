# 一句话需求到PR — AI 如何自主交付代码

## Core Thesis
AI 写代码不难，难的是让 AI 的代码能上线。8 阶段 Pipeline 是从玩具到生产的桥。

## Key Points
1. AI 写代码已经很强了 — 但"能写"≠"能上线"，中间差一个 Pipeline
2. 8 阶段闭环：EVALUATE→THINK→PLAN→BUILD(TDD)→REVIEW→TEST→DELIVER→REFLECT
3. 每个阶段解决一个具体问题：该不该做？怎么做？做对了吗？学到什么？
4. TDD 不是可选的 — 先写测试后写代码，AI 也不能跳过
5. 真实案例：Pipeline 给自己打了 10/10 分，但功能 100% 不能用 — 翻车教训
6. 决策分类：mechanical（自动做）、taste（攒着一起问）、judgment（立刻停）
7. REFLECT 是闭环关键 — 每次 Pipeline 运行都让下次更好

## Narrative Arc
- **Hook:** "给 AI 一句话：'加一个语音输入功能'，3 小时后你收到一个 PR。这不是 demo，这是我每天在用的工具。"
- **Setup:** 现状 — AI 写代码很容易，但从代码到上线的路上全是坑
- **Development:**
  - EVALUATE: 先问该不该做（ROI 评分，不是所有需求都值得投入）
  - THINK→PLAN: 调研→设计→3 个方案选 1 个
  - BUILD(TDD): 红灯→绿灯→验证，AI 也必须先写测试
  - REVIEW: 19 个检查项 — 从安全到性能到 UX
  - TEST: 不是跑一遍测试，是修 bug 直到全绿
- **Climax:** 翻车故事 — Voice Input: 14 个测试全绿、8 阶段全过、信心 10/10，但 Content-Type 一个 header 写错了，功能 100% 不能用。一个真实 HTTP 请求就能发现的 bug，14 个测试没抓到。这就是为什么 Pipeline 要不断进化。
- **Resolution:** REFLECT — 翻车不可怕，可怕的是翻了同一辆车。Pipeline 每次翻车都加新检查项（RP1→RP19），下次不会翻同一辆车。现在 Pipeline 已经翻了 5 次车，攒了 19 个检查项。

## Evidence Bank

### Data
- 1247 行 INSTRUCTIONS.md 驱动整个 Pipeline
- 5 次完整 Pipeline 运行数据（Slack adapter, Voice Input, Token Usage, Pollinate, etc.）
- 19 个 Review Pattern（每个都从真实 bug 中来）
- Pipeline 10/10 confidence → 12 个 bug（LL10 原始数据）
- Pollinate 本身：73 个文件、一次 Pipeline 运行、ROI 4.60

### Quotes
- "Pipeline dog-fooding validates architecture" — IMPROVEMENT.md
- "Pipeline confidence 10/10 是假的 — scoring 验'做了没有'不验'做得对不对'" — LL10
- "最致命的 bug 最容易被一个真实请求发现" — LL12

### Visuals
- 8 阶段 Pipeline 流程图（FlowChart 组件）
- TDD 红绿灯循环图（Timeline 组件）
- REVIEW 19 检查项 → 5 次翻车 → 自我进化的 Timeline
- 10/10 信心 vs 12 个 bug 的对比（ComparisonCard）
- 决策分类表（mechanical/taste/judgment）（DataTable / FeatureGrid）
