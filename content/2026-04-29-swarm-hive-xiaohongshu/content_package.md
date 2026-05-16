# Swarm Hive — 你的 AI 团队，云端 24/7

## Core Thesis
一条命令把桌面 AI 助手部署到云端，手机随时用，数据归你，$68/月。

## Key Points (6)
1. **痛点共鸣** — 桌面 AI 助手出门就断联，手机上用不了 — 2.3M+ 小红书用户搜索过"AI助手"
2. **一条命令部署** — `python provisioner.py deploy --name my-hive` → 12 分钟，完整 AI 团队上线
3. **完整不阉割** — 61 个技能、记忆系统、工作流、Slack 集成 — 和桌面版 100% 一致
4. **数据主权** — 你的 AWS 账号、你的 EBS 卷、你的记忆。不是 SaaS，不被锁定
5. **真实成本** — $128/月全天候，开启 auto-stop 后 $68/月 — 每天不到 ¥16
6. **团队分享** — 给同事开独立实例，推送共享知识，对话记忆完全隔离

## Narrative Arc
- **Hook:** "你的 AI 助手，出门就断联？"
- **Setup:** 桌面 AI 助手的天花板 — 只能在电脑前用
- **Development:** Swarm Hive 的三个核心能力（一条命令、完整体验、数据归你）
- **Climax:** 真实成本对比 — $68/月 vs AI SaaS 订阅
- **Resolution:** 开源地址 + 如何开始 + CTA

## Evidence Bank
- **Data:** 12 分钟部署、61 个技能、$68/月成本、46 天使用记录
- **Architecture:** EC2 + CloudFront + Caddy + Basic Auth
- **Real user:** Titus 已在使用独立 Hive 实例
- **Cost breakdown:** EC2 $119 + EBS $4 + EIP $3.65 + CF $1 = $128 全天候

## Internal References
- `Knowledge/Designs/2026-04-28-hive-mvp-design.md`: 架构全图
- `Knowledge/Designs/2026-04-28-hive-e2e-flow-design.md`: 部署流程
- `.context/MEMORY.md [KD07]`: Memory sovereignty 第一原则
