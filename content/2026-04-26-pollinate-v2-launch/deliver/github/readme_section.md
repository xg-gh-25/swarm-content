## 🌸 Pollinate — Media Value Delivery Engine

Pollinate transforms a single message into publish-ready media packages across multiple platforms. Not a "video maker" — a full GTM pipeline.

**Input:** `"Make content about AI Pipeline autonomous code delivery"`

**Output (one pipeline run):**
- 4.5min 4K video (Remotion + Amazon Polly TTS)
- 65 subtitle entries (SRT, native burn-in)
- 3 thumbnail sizes (16:9, 4:3, 3:4)
- Vertical shorts (auto-recut to 9:16)
- Per-platform publish copy (B站, YouTube, 小红书, 抖音, 视频号)

**9-stage pipeline:** INTAKE → EVALUATE → STRATEGIZE → PLAN → BUILD → REVIEW → TEST → DELIVER → REFLECT

The STRATEGIZE stage writes a PR/FAQ (source doc) and generates a channel × format matrix — the AI decides what format works best for each platform. Video for B站, poster for 小红书, narrative for WeChat.

```bash
# Quick start
cd backend/skills/s_pollinate
python scripts/topic_backlog.py add --message "Your topic here" --source user --score 4.0
# Then in Swarm: "Pollinate: [topic]"
```

[→ Design doc](Knowledge/Designs/2026-04-26-pollinate-v2-media-value-engine-design.md) | [→ Brand identity](backend/skills/s_pollinate/brand/identity.yaml)
