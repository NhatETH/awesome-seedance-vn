# 🎯 Workflow #1: 9-Panel Grid (Sweet Spot)

> **The 80/20 workflow.** 80% of use cases work best with 9-panel grid. Master this before exploring others.

[← Back to workflows](README.md)

---

## 🇻🇳 Tóm tắt

9-panel grid (3×3) là sweet spot cho 80% use case AI video. Cộng đồng tháng 5/2026 đã hội tụ về kết luận này. Lý do: vừa đủ thông tin (9 beats kể được story arc 4 hồi), vừa đủ chi tiết (mỗi panel còn sắc nét), aspect 1:1 linh hoạt cho mọi platform sau.

## 🇬🇧 TL;DR

9-panel grid (3×3) is the sweet spot for 80% of AI video use cases. The May 2026 community consensus: balanced information density (9 beats = full 4-act dramatic arc), readable detail per panel, and 1:1 aspect ratio that crops well to all platforms.

---

## 🎬 Use Cases for 9-Panel

✅ **Best for:**
- Drama short 9-12s (full dramatic arc)
- Tutorial / process (9 steps)
- Brand storytelling (problem→solution arc)
- Travel / documentary B-roll (9 establishing shots)
- Character introduction (9 expressions/poses)
- Product demo (9 angles)

❌ **NOT best for:**
- Casting test → use 4-panel
- K-pop dance MV → use 16-panel
- Single-action shot → use single image (no grid)
- Comic book adaptation with title → use 12-panel + title

---

## 📋 Full Workflow Step-by-Step

### 🟦 STEP 1 — Brief tiếng Việt → 9 cảnh

**Time:** 3-5 phút
**Tool:** Claude / ChatGPT (with [Director V2 system prompt](04-system-prompts/claude-director-v2.md))

#### Input format
```
Brief: [Mô tả tiếng Việt 2-4 câu]

Yêu cầu:
- Format: short drama / tutorial / brand story
- Duration: 9-12 giây
- Aspect output: 16:9 / 9:16 / 1:1
- Mood: [vui / buồn / hồi hộp / hoành tráng]

Hãy chia thành 9 cảnh theo 4 hồi:
- Setup (panels 1-2)
- Rising (panels 3-4)
- Turn (panels 5-6)
- Resolution (panels 7-9)
```

#### Example Brief
```
Brief: Cô gái 28t mở thư của bố, phát hiện bố có gia đình thứ 2.
Format: Drama short
Duration: 9s
Aspect output: 16:9
Mood: Buồn / drama tâm lý
```

#### Output (Claude returns)
```
9 cảnh chia theo 4 hồi:

SETUP:
1. Cô gái về căn hộ trống, cởi áo khoác chậm rãi
2. Thấy lá thư chưa mở trên bàn, ngần ngại

RISING:
3. Cầm thư, tay run nhẹ
4. Mở thư — bức ảnh đen trắng rơi ra

TURN:
5. Close-up: ảnh bố cô bên người phụ nữ lạ
6. Mặt cô đông cứng — bối rối, rồi nhận ra

RESOLUTION:
7. Cô ngồi xuống sàn, ảnh trong tay, nước mắt
8. Wide: cô ngồi một mình, đèn duy nhất
9. Mặt cô từ từ giãn ra — quyết tâm mới
```

---

### 🟦 STEP 2 — Generate Grid trong GPT Image 2

**Time:** 3-5 phút
**Tool:** ChatGPT (Plus/Pro) với GPT Image 2

#### Prompt template
```
A 3×3 grid storyboard (1:1 aspect), 9 cinematic panels with bold black 4px borders and 8px white gutters.

ULTRA-CONSISTENT main character: [character description from brief]

Panels read left-to-right, top-to-bottom:
1: [scene 1 from step 1]
2: [scene 2]
3: [scene 3]
...
9: [scene 9]

Style: [genre cinematic, palette, lighting reference]
```

#### Example (filled)
```
A 3×3 grid storyboard (1:1 aspect), 9 cinematic panels with bold black 4px borders and 8px white gutters.

ULTRA-CONSISTENT main character: a 28-year-old Vietnamese woman, shoulder-length black bob, beige wool coat, calm pensive expression. SAME face, SAME hair, SAME outfit across all 9 panels.

Panels read left-to-right, top-to-bottom:
1: She enters her empty Hà Nội apartment at dusk, removes coat slowly.
2: She sees an unopened letter on the table, hesitates.
3: She picks up the letter, hand trembles slightly.
4: She opens it — a black-and-white photo falls out.
5: Close-up: photo shows her father with an unknown woman.
6: Her expression freezes — confusion, then dawning realization.
7: She sits down on the floor, photo in hand, tears form.
8: Wide shot: she sits alone in dim apartment, single lamp on.
9: Her face slowly resolves — no more tears. A new resolve appears.

Style: melancholic K-drama, cool blue dim tungsten light, shallow depth of field, Lưu Diệc Phi reference.
```

#### Iteration tip
- If GPT Image 2 misses 1-2 panels, edit only those panels (not regenerate whole)
- If face inconsistent across panels, add: `EVERY panel must show the EXACT same face — same eyes, same nose, same mouth shape, same skin tone.`
- If style varies, add specific reference: `same lens (50mm equivalent), same color grade (cool blue tungsten LUT)`

---

### 🟦 STEP 3 — Write Motion Prompt (3-Layer)

**Time:** 3 phút
**Tool:** Claude (with system prompt)

#### Output format (Claude returns)
```
=== MOTION PROMPT — SEEDANCE ===

STYLE & MOOD:
Melancholic K-drama short, cool blue dim tungsten light with shallow DoF, Lưu Diệc Phi cinematography reference. 16:9 final, 24fps.

DYNAMIC DESCRIPTION:
Animate this 9-panel character study into a continuous 9-second melancholic drama. Camera moves naturally through her emotional journey:

At 0-1s: she enters apartment, removes coat (panel 1).
At 1-2s: notices letter, hesitation (panel 2-3).
At 2-3s: opens letter, photo falls (panel 4).
At 3-5s: close-up reveal of photo, expression freezes (panels 5-6).
At 5-7s: sits on floor, tears form (panel 7).
At 7-9s: alone in dim room → final resolve (panels 8-9).

STATIC DESCRIPTION:
ULTRA-CONSISTENT character identity — face, hair, beige coat unchanged. Hà Nội apartment dim tungsten lighting locked. Color grade cool blue + warm lamp accent throughout.
```

---

### 🟦 STEP 4 — Generate in Seedance

**Time:** 5-15 phút
**Platform:** 0ai.vn (rẻ, không cần VPN, support 4K) hoặc Jimeng (cần VPN, nhiều quota free)

#### Settings
- Upload grid image as reference (`@subject1`)
- Paste motion prompt
- Aspect: **1:1 or 16:9** (NOT 9:16 — auto-crop)
- Duration: 8-12s
- Resolution: 480p Fast for testing
- FPS: 24

#### Generate 3 versions at 480p
- ~1-2 credits each
- **Cost: $0.30-0.60 total**
- Pick best version

#### Final at 1080p
- 1 generation: ~48 credits
- **Cost: ~$2.40**

#### Total cost: ~$3 per 9-panel video

---

### 🟦 STEP 5 — Edit in CapCut

**Time:** 10-15 phút

1. Import generated 1080p MP4
2. Add Vietnamese voice-over (use ElevenLabs or 11labs.io)
3. Add background music (royalty-free từ Epidemic Sound / Artlist)
4. Add captions (Vietnamese auto-generate)
5. Add brand logo intro/outro (5s + 5s)
6. Export 1080p H.264

#### Multi-format export
- **YouTube/Web:** 16:9 1080p
- **TikTok/Reels:** 9:16 1080p (crop in CapCut)
- **Instagram feed:** 1:1 1080p (center crop)

---

## ⏱️ Total Time & Cost

| Phase | Time | Cost |
|-------|------|------|
| Step 1: Brief → 9 scenes | 3-5 min | Free (Claude) |
| Step 2: GPT Image 2 grid | 3-5 min | $0.20-0.40 |
| Step 3: Motion prompt | 3 min | Free (Claude) |
| Step 4: Seedance generate | 5-15 min | $3 |
| Step 5: CapCut edit | 10-15 min | Free |
| **Total** | **~30 min** | **~$3-3.50** |

**Compared to old "single shot" T2V workflow:** ~3x faster, ~5x cheaper, much higher quality.

---

## 📊 Success Rate Reference

Internal benchmarks across 50+ test runs:

| Metric | 9-panel grid | T2V single-shot |
|--------|-------------|----------------|
| First-gen success | 65% | 25% |
| With 1 iteration | 85% | 50% |
| With 3 iterations | 95% | 70% |
| Character consistency | 95% | 60% |
| Cost per finished video | $3 | $12-15 |

---

## 🎓 Common Pitfalls

### 1. Trying to fit too many actions in 9 panels
**Fix:** 9 panels = 9 BEATS. Each beat = ONE main action. Don't stack multiple actions in 1 panel.

### 2. Using 9:16 grid (vertical)
**Fix:** ALWAYS use 1:1 or 16:9 for grids. Seedance auto-crops 9:16. Use CapCut to crop later.

### 3. Forgetting "ULTRA-CONSISTENT" keyword
**Fix:** This is non-optional. Every prompt MUST have it.

### 4. Motion prompt over-explains the grid
**Fix:** Don't say "pan over comic page". Say "animate into continuous video". Grid is visual DNA, not subject.

### 5. Not using iteration loop
**Fix:** Always test 3 versions at 480p Fast first. Pick best. Then 1080p final.

---

## 🚀 Next Steps

After mastering 9-panel:
- Try [16-Panel Dance Grid](02-grid-16-panel/01-dance-mv.md) for K-pop MV
- Try [Character Bible](03-character-bible.md) for series with same character
- Try [Iteration Loop](05-iteration-loop.md) for production-tier quality

---

[← Workflows](README.md) · [← Main](../README.md)
