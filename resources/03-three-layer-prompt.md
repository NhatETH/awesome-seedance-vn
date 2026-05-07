# 📙 3-Layer Motion Prompt Structure / Cấu trúc Motion Prompt 3 lớp

> **🆕 NEW STANDARD May 2026** — Replaces the old 6-step formula for MOTION prompts (the 6-step formula is still correct for IMAGE prompts).

[← Back to resources](README.md) · [← Main README](../README.md)

---

## 🇻🇳 Tóm tắt

Cộng đồng AI video toàn cầu (Atlas Cloud, EvoLinkAI, Higgsfield) đã hội tụ vào tháng 5/2026 về 1 cấu trúc CHUẨN cho motion prompt: **Style & Mood → Dynamic Description → Static Description**. Tỷ lệ thành công tăng từ **40-50% lên 80-90%**.

## 🇬🇧 TL;DR

The global AI video community converged in May 2026 on a STANDARD structure for motion prompts: **Style & Mood → Dynamic Description → Static Description**. Success rate jumped from 40-50% to 80-90%.

---

## ❌ Why the old 6-step formula falls short for motion prompts

The classic 6-step formula (`Subject + Action + Setting + Camera + Lighting + Style`) was designed for **image prompts** (single frame). When applied to **motion prompts** (animating images into video), it has these issues:

1. **No timeline awareness** — Seedance doesn't know when each action happens
2. **Conflicting instructions** — Style words mixed with motion words confuse the model
3. **Drift over duration** — Without explicit "static" anchors, identity drifts in long shots
4. **Cinematic quality vague** — "cinematic style" alone doesn't tell the model HOW to be cinematic

---

## ✅ The 3-Layer Structure

### 📐 Layer 1 — STYLE & MOOD (10-15% of prompt, 1-2 sentences)

Defines the visual identity of the video as a whole. This layer is the "DNA" the model should preserve from frame 1 to frame N.

**Include:**
- Genre (`cinematic` / `documentary` / `commercial` / `anime`)
- Color palette (`midnight blues with amber highlights`)
- Lighting baseline (`soft natural window light` / `dramatic chiaroscuro`)
- Aspect & resolution (`16:9, 8K hyperrealistic`)
- Reference (optional: `Wong Kar-wai inspired` / `Netflix production quality`)

**Example:**
```
STYLE & MOOD:
Photorealistic cinematic realism, Netflix production quality, IMAX-grade detail.
Midnight palette — cold blues with warm amber highlights from emergency flares.
Anamorphic lens flare. 16:9, 8K hyperrealistic textures.
```

---

### 🎬 Layer 2 — DYNAMIC DESCRIPTION (60-80% of prompt, the bulk)

Describes EXACTLY what happens, second by second. This is the longest layer. Use:
- **Active verbs** (not adjectives)
- **Timeline notation** (`At 0-3s:`, `At 3-6s:`)
- **One main shot per beat** (not stacked descriptions)
- **Specific actions** (not abstract concepts)

**Bad example (avoid):**
```
A dramatic scene unfolds with intense emotions and beautiful cinematography.
```

**Good example:**
```
DYNAMIC DESCRIPTION:
Opens extreme wide aerial drone — Panama Canal at midnight.

At 0-3s: Filaments stretched taut across water, catching faint moonlight.
At 3-6s: Cruise ship arrives, hull contacts filaments.
At 6-10s: Metal slabs shear, water columns erupt.
At 10-15s: Camera pulls back, revealing full devastation.
```

---

### 🔒 Layer 3 — STATIC DESCRIPTION (10-15% of prompt, 1-2 sentences)

Describes what does NOT change throughout the video. This locks the model's drift over duration.

**Include:**
- Character identity (face, clothing)
- Setting consistency (location, props)
- Color grade lock
- Mood baseline

**Example:**
```
STATIC DESCRIPTION:
ULTRA-CONSISTENT character identity (face, wardrobe).
Midnight setting unchanged. Lens flare persists.
Color grade locked: cold blue + amber accent throughout.
```

---

## 📋 Full Template

```markdown
STYLE & MOOD:
[1-2 sentences — genre, palette, lighting baseline, aspect/resolution]

DYNAMIC DESCRIPTION:
[Opening shot description.]
At 0-3s: [action 1].
At 3-6s: [action 2 — escalate].
At 6-10s: [action 3 — climax].
At 10-12s: [action 4 — resolution].

STATIC DESCRIPTION:
[1-2 sentences — what doesn't change]
ULTRA-CONSISTENT [character/wardrobe/setting].
[Color grade lock.] [Mood baseline.]

[Optional] HARD CONSTRAINTS:
[Engine-specific limits, see Archetype Router]
```

---

## 📏 Length Rule: 60-100 words

Sweet spot for Seedance 2.0:

- **< 60 words:** Missing detail → output drifts, blurry
- **60-100 words:** Optimal — clear instructions without conflict
- **> 100 words:** Conflicting instructions → blur, artifacts

**Pro tip:** Count after writing. If over 100, cut filler adjectives (`beautiful`, `amazing`, `stunning`).

---

## 🆚 Side-by-Side Comparison

### ❌ Old 6-step (suboptimal for motion)
```
A 28-year-old Vietnamese woman in red áo dài walks through Saigon villa party at night, 
guests turn to admire her, she meets her twin sister, they confront each other, slow push-in
camera, warm tungsten lighting, K-drama cinematic style.
```
**Problems:** No timeline. No static anchor. Camera mixed with action. ~85% drift in tests.

### ✅ New 3-layer (optimal)
```
STYLE & MOOD:
K-drama short cinematic, warm tungsten + cool moonlight blue, shallow DoF, 
Lưu Diệc Phi reference, 16:9 4K.

DYNAMIC DESCRIPTION:
Opens medium shot — Character A holds champagne, smiles confidently.
At 0-3s: side door opens, Character B enters quietly.
At 3-6s: Character A spots her, smile freezes mid-sip.
At 6-9s: slow tilt up reveals identical faces, contrasting outfits.
At 9-12s: champagne glass slips, slow-motion shatter — A's tear forms.

STATIC DESCRIPTION:
ULTRA-CONSISTENT twin features (face structure, age 22).
Saigon villa hall — chandelier, marble floor unchanged.
Color grade locked: tungsten warm + moonlight cool.
```
**Result:** Clear timeline. Static anchors prevent drift. ~85% success rate in tests.

---

## 🎯 When to use each layer most heavily

| Use Case | Layer 1 | Layer 2 | Layer 3 |
|----------|---------|---------|---------|
| Single emotional shot | Light | Medium | Heavy |
| Multi-action drama | Medium | Heavy | Medium |
| Product TVC | Heavy | Medium | Medium |
| Documentary B-roll | Heavy | Light | Light |
| K-pop dance MV | Medium | Heavy | Heavy |
| Henshin transformation | Medium | Heavy | Heavy |
| Satisfying loop | Heavy | Medium | Heavy (loop anchor) |

---

## 🧪 Quick Quality Test

After writing your motion prompt, ask yourself:

- [ ] Can I count exact seconds for each action? (Layer 2 timeline)
- [ ] Is character/setting identity locked? (Layer 3)
- [ ] Is genre/palette clear in 1 sentence? (Layer 1)
- [ ] Is total word count 60-100? (Length rule)
- [ ] Have I used active verbs (not adjectives)? (Verb test)
- [ ] Is each "At X-Ys:" line ONE main action? (No stacking)

If 5/6 passed → 80%+ chance of success on first generation.

---

## 🔗 Related

- [Scene Archetype Router](05-archetype-router.md) — choose archetype BEFORE writing prompt
- [4-Step Iteration Loop](../workflows/05-iteration-loop.md) — refine with structured tests
- [System Prompts for LLMs](../workflows/04-system-prompts/) — Claude/ChatGPT will write 3-layer prompts for you

---

## 📚 Sources

- [Atlas Cloud — Drama Workflow Guide (April 2026)](https://www.atlascloud.ai/blog/guides/ultimate-drama-workflow-gpt-image-2-seedance-2-0)
- [Higgsfield — Seedance Prompting Guide](https://higgsfield.ai/blog/seedance-prompting-guide)
- [@deredleritt3r on X](https://x.com/) — Motion prompt mental model pioneer
- [Seedance 2.0 Official Prompt Guide (APIYI)](https://help.apiyi.com/en/seedance-2-0-prompt-guide-video-generation-camera-style-tips-en.html)

---

[← Resources](README.md) · [← Main README](../README.md)
