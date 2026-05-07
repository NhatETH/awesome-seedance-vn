# 🔧 Workflows / Quy trình thực chiến

[← Back to main](../README.md)

5 production-ready workflows. Mỗi workflow là pipeline + template để bạn copy-customize cho dự án.

---

## 📂 Workflows

| # | Workflow | Best For | Difficulty |
|---|----------|----------|-----------|
| 01 | [9-Panel Grid](01-grid-9-panel.md) | **80% use cases** — drama, tutorial, process | Beginner |
| 02 | [16-Panel Dance Grid](02-grid-16-panel.md) | K-pop/V-pop MV | Intermediate |
| 03 | [Character Bible System](03-character-bible.md) | Multi-shot consistency, drama series | Intermediate |
| 04 | [System Prompts for LLMs](04-system-prompts/) | Automate prompt writing | Advanced |
| 05 | [4-Step Iteration Loop](05-iteration-loop.md) | Save 75% credits, ensure quality | Beginner |

---

## 🎯 Which workflow to use?

### Start here:
1. **Just experimenting?** → [4-Step Iteration Loop](05-iteration-loop.md)
2. **Making a drama / tutorial / process video?** → [9-Panel Grid](01-grid-9-panel.md)
3. **Making a K-pop MV?** → [16-Panel Dance Grid](02-grid-16-panel.md)
4. **Series with same character?** → [Character Bible](03-character-bible.md)
5. **Want LLM to write prompts for you?** → [System Prompts](04-system-prompts/)

---

## 🔥 Pipeline Overview / Tổng quan Pipeline

```
┌─────────────┐
│   BRIEF     │  Client/idea (Vietnamese OK)
│  (5 phút)   │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   ChatGPT   │  Break into scenes (use Claude/ChatGPT system prompt)
│  / Claude   │
│  (3 phút)   │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ GPT Image 2 │  Generate storyboard grid (3×3 default, 4×4 for dance)
│  (5 phút)   │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   Claude    │  Write motion prompt (3-layer + archetype + constraints)
│  (3 phút)   │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│  Seedance   │  Test 3 versions @ 480p Fast → pick best → 1080p final
│ (15 phút)   │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   CapCut    │  Edit, music, voice-over, captions
│ (10 phút)   │
└──────┬──────┘
       │
       ▼
   ┌──────┐
   │ DONE │  Total time: ~45 phút for production-ready video
   └──────┘
```

---

[← Main README](../README.md)
