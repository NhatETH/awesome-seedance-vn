# 📕 Storyboard Grid Method — Save 70% Credits

> **Pipeline thay đổi mọi thứ.** Thay vì generate 9 video riêng lẻ ($9-15), bạn generate **1 grid storyboard** ($0.30) → animate thành 1 video continuous ($1.50-3). Tiết kiệm 60-70% credit, quality cao hơn, consistency tự động.

[← Back to resources](README.md)

---

## 🇻🇳 Tóm tắt

**Phương pháp cũ (text-to-video):** Viết prompt → generate video → kết quả thường drift, character thay đổi, lighting nhảy. Test 5-10 versions = $10-20.

**Phương pháp mới (grid + image-to-video):**
1. Generate 1 ảnh grid 3×3 (hoặc 4×4) — mỗi ô = 1 cảnh story
2. Upload grid làm reference
3. Viết motion prompt mô tả cách animate theo trình tự
4. Seedance generate video continuous theo grid

**Kết quả:** Character consistency tự động (vì grid cố định), cost giảm 60-70%, iteration nhanh hơn.

---

## 🧠 Why this works

Seedance 2.0 có image-to-video mode mạnh hơn text-to-video. Khi bạn cung cấp **ảnh storyboard có tất cả cảnh trong 1 frame**, model:
1. Hiểu được spatial layout (chỗ nào là cảnh nào)
2. Maintain character identity (face đã được lock từ image)
3. Maintain lighting/setting (vì đã có ground truth)
4. Cần generate ít detail hơn → tiết kiệm compute → ít drift

**Insight cốt lõi:** Storyboard không phải "preview" — đây là **constraint** cho video gen.

---

## 📊 Comparison: Cost & Quality

### Old method (text-to-video, 9 separate videos)

| Item | Cost | Time |
|------|:----:|:----:|
| 9 video generations × $1.50 | $13.50 | 5-7 min each = 45-60 min |
| 3 iterations per video (avg) | $40+ total | 2-3 hours |
| Character consistency | ❌ Drifts | — |
| Editing into 1 sequence | Manual cut | 30 min |

**Total:** $40-50, 3-4 hours, inconsistent quality.

### New method (grid storyboard + 1 continuous video)

| Item | Cost | Time |
|------|:----:|:----:|
| 1 grid generation (GPT Image 2) | $0.40 | 1-2 min |
| 1 grid iteration | $0.40 | 1-2 min |
| 1 continuous video generation | $2.50 | 5-7 min |
| 2 video iterations | $5 | 10-15 min |
| Character consistency | ✅ Auto | — |

**Total:** $8-9, 30-45 min, consistent quality.

**Savings: 80% cost, 70% time.**

---

## 🎬 The Pipeline (5 Steps)

### Step 1: Outline scenes (5 phút)

Break your video idea into 9 scenes (or 16 for advanced):

```
Scene 1: Establishing shot — character in setting
Scene 2: Character close-up — emotional anchor
Scene 3: Detail shot — prop or texture
Scene 4: Action begins — first movement
Scene 5: Mid-action — body in motion
Scene 6: Reaction — expression change
Scene 7: Climax — peak moment
Scene 8: Aftermath — settling
Scene 9: Final image — memorable closer
```

### Step 2: Write grid prompt for image gen (5 phút)

Format:

```
A 3×3 grid storyboard (1:1 aspect, 9 cinematic panels with bold black 4px borders 
and 8px white gutters). [Genre/mood description].

ULTRA-CONSISTENT CHARACTER: [Full character bible - face, hair, wardrobe in detail].
The face stays IDENTICAL across all 9 panels.

Setting: [Location and lighting consistency requirements].

Read panels left-to-right, top-to-bottom:

Panel 1: [Scene 1 description]
Panel 2: [Scene 2 description]
...
Panel 9: [Scene 9 description]

STYLE: [Director reference, lens character, color palette]
CONSTRAINTS: [What to avoid - text, glitches, etc.]
```

### Step 3: Generate grid (5 phút)

**Best models for grids:**
- **GPT Image 2** — best at multi-cell layouts, understands "panel" terminology
- **Nano Banana 2** — best for Asian character consistency
- **FLUX 1.1 Pro** — best for hero-shot detail

Generate 2-3 versions, pick best.

### Step 4: Write motion prompt (5 phút)

Use [3-Layer Motion Prompt Structure](03-three-layer-prompt.md):
- **Style & Mood** — overall aesthetic
- **Dynamic Description** — frame-by-frame animation logic
- **Static Description** — what stays consistent

Tell Seedance: "Animate this 9-panel storyboard into a [X]-second continuous sequence."

### Step 5: Generate video (15-30 phút)

1. **480p Fast** test (3 versions) → pick best — costs ~$1.50
2. **1080p Standard** final → costs ~$2.50

Total render time: 15-30 min including iterations.

---

## 📐 Aspect Ratio Strategy

### Grid generation
- **1:1 (square)** — DEFAULT. Cells become roughly square, easy to read
- **4:3** — for cinematic widescreen content within cells
- **NEVER 9:16** — Seedance auto-crops grid and loses 60% content

### Final video (after Seedance generates)
- 16:9 → YouTube, web
- 9:16 → TikTok, Reels (crop in CapCut from 16:9)
- 1:1 → IG feed (crop in CapCut)
- 2.39:1 → Cinema (crop in CapCut)

**Rule:** Generate at 1:1 or 16:9, then crop down. Don't generate at 9:16 directly.

---

## 🎯 Grid Sizes — When to use which

| Grid | Cells | Final video | Best for |
|------|:-----:|:-----------:|----------|
| **3×3 (9-panel)** | 9 | 8-12s | 80% use cases — drama, tutorial, process, ASMR |
| **4×4 (16-panel)** | 16 | 12-24s | K-pop MV, cổ trang, TVC luxury, short film |
| **2×2 (4-panel)** | 4 | 4-6s | Quick TikTok, simple loops |
| **5×3 (15-panel)** | 15 | 15-20s | Rare — when 16 too many but 9 too few |

[👉 9-Panel Workflow](../workflows/01-grid-9-panel.md) · [👉 16-Panel Master Series](../workflows/02-grid-16-panel/)

---

## 🚨 Common Failures

### Failure 1: "Cells don't match each other"
**Cause:** Character bible not strong enough.
**Fix:** Add `ULTRA-CONSISTENT CHARACTER: [face, hair, wardrobe IDENTICAL across all cells]` in prompt.

### Failure 2: "Grid generates as 9 unrelated images"
**Cause:** GPT Image 2 lost context.
**Fix:** Start prompt with `A 3×3 grid storyboard with bold black borders separating cells.`

### Failure 3: "Video animates each cell separately, jumps between scenes"
**Cause:** Motion prompt didn't tell Seedance it's a sequence.
**Fix:** Use phrase: `Animate this storyboard into ONE CONTINUOUS [X]-second cinematic sequence reading left-to-right, top-to-bottom.`

### Failure 4: "Character changes face in some cells"
**Cause:** Cell density too high for face fidelity.
**Fix:** Use Nano Banana 2 to regenerate problem cells, composite back in Photoshop.

### Failure 5: "Lighting jumps between cells"
**Cause:** No lighting anchor specified.
**Fix:** Add `LIGHTING ANCHOR: Single key light from camera-left at 45° in all 9 panels`.

---

## 💎 Pro Techniques

### Multi-engine composite
Instead of using 1 image model for entire grid:
1. **Layout** in GPT Image 2 (best at panel structure)
2. **Character cells** regenerated in Nano Banana 2 (best Asian faces)
3. **Hero shot cells** regenerated in FLUX 1.1 Pro (best material textures)
4. **Composite** in Photoshop using best cells from each
5. **Use composite** as reference for Seedance

This is the technique only documented in this repo. Saves 30-50% iteration time vs single-model approach.

### Color script evolution
For 9-panel: cells 1-3 cool, 4-6 warm, 7-9 climax saturation.
For 16-panel: cells 1-4 cool, 5-8 warming, 9-12 saturated peak, 13-16 muted resolution.

This forces emotional arc into image generation.

### Audio anchors
For each "block" of 3-4 panels, define audio character. Tell Seedance:
```
Panels 1-3: ambient room tone + soft strings entry
Panels 4-6: percussion entering, building tension
Panels 7-9: full score peak, dramatic cymbal at climax
```

Seedance 2.1+ uses these as audio generation anchors.

---

## 🔗 Related

- [9-Panel Workflow](../workflows/01-grid-9-panel.md) — Default workflow
- [16-Panel Master Series](../workflows/02-grid-16-panel/) — Expert tier
- [3-Layer Motion Prompt](03-three-layer-prompt.md) — How to write motion prompt
- [Character Bible System](../workflows/03-character-bible.md) — Lock character identity

---

[← Resources](README.md) · [Main README](../README.md)
