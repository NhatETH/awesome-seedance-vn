# 🧬 Workflow #3: Character Bible System

> **Foundation cho mọi multi-shot project.** Character Bible = 1 document mô tả nhân vật chi tiết đến mức AI generation cross-shot consistency. Pro creators không bao giờ skip step này.

[← Back to workflows](README.md)

---

## 🇻🇳 Tại sao Character Bible quan trọng?

Drift là vấn đề lớn nhất của AI video. Cùng character, prompt khác → face/outfit/age/style nhảy lung tung.

Character Bible giải quyết bằng cách:
1. **Lock identity** — face/body/age/ethnicity được định nghĩa chính xác
2. **Lock wardrobe** — mỗi piece được mô tả chi tiết (color/material/cut)
3. **Lock styling** — hair/makeup/accessories
4. **Lock posture/gesture** — physical signature
5. **Lock voice/personality** — for emotional consistency

Khi bạn copy-paste Character Bible vào mỗi prompt, AI có ground truth. Drift giảm 70-80%.

---

## 📋 The Template

```
=== CHARACTER BIBLE: [Character Name] ===

ROLE / BACKSTORY:
[1-2 sentences about who they are, what they want]

DEMOGRAPHICS:
- Age: [exact number, not range]
- Ethnicity: [Vietnamese Kinh / Korean / Vietnamese-Korean mixed / etc.]
- Build: [height + body type — "168cm slim athletic" not "tall and fit"]

HAIR:
- Color: [exact — "jet black" / "platinum silver-white" / "dark brown with subtle highlights"]
- Length: [exact — "shoulder-length" / "waist-length" / "buzz cut"]
- Texture: [straight / wavy / curly + thickness]
- Style: [parted side / bangs / ponytail / specific style]
- Finish: [glossy / matte / windblown]

FACE:
- Shape: [oval / round / heart / square]
- Skin: [tone + undertone + texture — "fair-medium with warm undertone, matte natural"]
- Eyes: [shape + color + lash detail]
- Nose: [shape + bridge type]
- Lips: [shape + natural color + finish]
- Distinguishing features: [moles, scars, freckles, dimples — be specific]

WARDROBE (each piece detailed):
- Top: [garment + material + color + cut + accents]
- Bottom: [same level of detail]
- Outerwear: [if any]
- Footwear: [exact type, color, brand-feel without naming brands]

ACCESSORIES:
- Jewelry: [each piece described]
- Hat / headwear: [if any]
- Bag: [if visible]
- Watch: [if visible]
- Glasses: [if any]

MAKEUP / GROOMING (for portrait shots):
- Base: [foundation level / glow / matte]
- Eyes: [eyeshadow / liner / lashes]
- Cheeks: [blush color + placement]
- Lips: [lipstick color + finish]
- Brows: [shape + filling]

POSTURE / GESTURE (signature traits):
- Default stance: [how they stand — "always slightly tilted head up"]
- Hand habits: [where their hands rest]
- Walking style: [pace + footfall character]
- Eye behavior: [direct gaze / averted / scanning]

VOICE / PERSONALITY (for emotion cues):
- Energy level: [high / measured / contemplative]
- Speech pattern: [if relevant for VO]
- Emotional default: [warm / aloof / intense / playful]

REFERENCE IMAGES (recommended):
- [Front view full body]
- [3/4 view medium]
- [Profile close-up of distinguishing feature]
```

---

## 🎯 Real Example (from 16-Panel Cổ Trang Template)

```
=== CHARACTER BIBLE: Trần Thị Nguyệt ===

ROLE: Daughter of Trần dynasty nobility, 22 tuổi, sắp xuất chinh chống Mông Cổ.

DEMOGRAPHICS:
- Age: 22
- Ethnicity: Vietnamese (Kinh), Northern Vietnam
- Build: 158cm, slim athletic (period-appropriate, not gym-built)

HAIR:
- Color: Jet black
- Length: Waist-length
- Texture: Slightly wavy, thick
- Style: Parted center, half-up with ngọc bích jade hairpin (chrysanthemum carved)

FACE:
- Shape: Oval
- Skin: Fair-medium, matte natural with slight luminosity at cheekbones
- Eyes: Natural double-lid, almond, dark brown
- Nose: Small straight
- Lips: Full natural rose
- Distinguishing: High cheekbones (period beauty marker)

WARDROBE:
- Underlayer: Áo yếm trắng lụa (white silk underbodice with breast-binding strap)
- Mid-layer: Áo giao lĩnh tay rộng, lụa lĩnh tía (deep purple-red), 
  trim viền lan can (geometric pattern in gold thread)
- Outer: Áo tứ điên formal robe, navy-black silk with phoenix embroidery silver
- Belt: Lụa hoàng kim sash, tied left side
- Bottom: Váy lĩnh xếp pli, same purple as áo giao lĩnh
- Footwear: Hài cong tip-curved, brocade with phoenix motif

ACCESSORIES:
- Trâm cài: Ngọc bích jade hairpin carved chrysanthemum
- Vòng cổ: Bạc đeo cốt ngọc lục bảo (silver chain with emerald pendant)
- Kiếm: Longsword Đông A style, dragon-engraved hilt, lacquer scabbard with mother-of-pearl

POSTURE:
- Default: Head slightly tilted up, never bowed (warrior pride)
- Hands: When still, left hand always on sword hilt
- Walking: Straight back, deliberate steps

PERSONALITY:
- Energy: Quietly determined, not loud
- Eyes: Lock onto subject and don't waver
- Default emotion: Composed, slight underlying intensity
```

---

## 🛠️ How to Use Character Bible

### Method 1: Direct paste in every prompt
**Pros:** Maximum consistency.
**Cons:** Eats tokens, prompts get long.

```
[Your scene-specific prompt]

CHARACTER REFERENCE:
[Paste full character bible here]
```

### Method 2: Reference image + abbreviated bible
**Pros:** Token-efficient.
**Cons:** Requires reference image.

```
[Your scene-specific prompt]

@subject1: 22-year-old Vietnamese noblewoman, 158cm slim athletic, jet-black waist-length wavy hair parted center with jade hairpin, fair-medium matte skin, oval face, áo giao lĩnh deep purple-red silk with gold trim. (See reference image for full detail.)
```

### Method 3: System prompt for LLM workflow
Define character once in [Claude Director V2](04-system-prompts/claude-director-v2.md) system prompt. LLM auto-applies to every generation.

---

## 🎨 Generating Reference Images

**Best practice:** Create 1-3 reference images BEFORE generating any video.

### Setup: 3-image reference pack

**Image 1: Full body front view**
- Subject standing facing camera
- Full body in frame
- Neutral pose, arms at sides
- Plain background (white or gray)
- Even lighting

**Image 2: 3/4 view medium shot**
- Subject from waist up
- 3/4 angle
- Slight expression (neutral or subtle smile)
- Same lighting as image 1

**Image 3: Profile or detail close-up**
- Profile shot OR close-up of distinguishing feature
- Shows hair texture, skin texture
- Jewelry/accessories visible if relevant

### Best image models for reference

| Character type | Best model |
|----------------|-----------|
| Asian face (Vietnamese, Korean, Japanese) | Nano Banana 2 |
| Western face (European, American) | FLUX 1.1 Pro |
| Period costume | GPT Image 2 |
| Highly stylized (anime, fantasy) | FLUX 1.1 Pro |
| Mixed ethnicity | FLUX 1.1 Pro |

### Iteration tip
Generate 4-6 versions of each reference image. Pick the one with cleanest face/best identity match.

---

## 🚨 Common Mistakes

### ❌ Mistake 1: Character bible vague
"Beautiful Vietnamese woman with long hair" is not a bible. Be obsessive about detail.

### ❌ Mistake 2: Forgetting accessories
Watch, jewelry, glasses get dropped between prompts. Always list every accessory.

### ❌ Mistake 3: Not specifying age clearly
"Young woman" → AI guesses 18-30. Specify exact age (24 vs 36 changes face significantly).

### ❌ Mistake 4: Wardrobe described as "elegant"
"Elegant" tells AI nothing. "Ivory silk áo dài with mandarin collar" tells AI everything.

### ❌ Mistake 5: Missing posture/gesture
Without posture cues, AI defaults to generic poses. Specify how character holds themselves.

### ❌ Mistake 6: No reference image for complex characters
For 16-panel projects with 2+ characters, reference images are mandatory. Trying to describe in prompt alone leads to drift.

---

## 💎 Advanced: Multi-Character Bible

For projects với 2-4 characters (cổ trang, drama):

```
=== PROJECT: [Name] ===

CHARACTER A: [Bible 1]
CHARACTER B: [Bible 2]

RELATIONSHIPS:
- A and B: [their dynamic]
- Visual contrast: [how they're visually distinct]

SCENE INTERACTIONS:
- A always stands camera-left, B camera-right (180° rule)
- A speaks first, B reacts
- Color contrast: A wears warm tones, B wears cool tones
```

This level of detail prevents character confusion in scenes where both appear.

---

## 🔗 Related

- [16-Panel Master Series](02-grid-16-panel/) — Where character bible matters most
- [9-Panel Workflow](01-grid-9-panel.md) — Simpler use case
- [System Prompts](04-system-prompts/) — Automate character bible application

---

[← Workflows](README.md) · [Main README](../README.md)
