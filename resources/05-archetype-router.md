# 🧪 Scene Archetype Router

> **5 scene archetypes** map mọi video idea bạn có vào 1 trong 5 patterns. Pick archetype → apply template → save 80% prompt-writing time.

[← Back to resources](README.md)

---

## 🎯 Why Archetypes?

99% video ideas có thể classify thành 5 archetypes. Mỗi archetype có:
- Camera grammar đặc trưng
- Pacing template
- Lighting default
- Aspect ratio recommendation
- Common mistakes

Thay vì viết prompt từ đầu mỗi lần, **router** input idea → recommend archetype → suggest base template.

---

## 📋 The 5 Archetypes

### 1. 🎭 PORTRAIT / Beauty
**Definition:** Subject hero, minimal action, beauty/identity focus.

**Examples:**
- Beauty product TVC
- Fashion editorial
- Influencer talking-head
- Henshin transformation
- ASMR macro skincare

**Camera grammar:**
- Static or slow push-in (rarely tracking)
- Medium → Close-up → ECU progression
- Shallow depth of field
- Eye-level or slight low-angle (flatters subject)

**Pacing:** Slow, contemplative. Hold each shot 2-4 seconds.

**Lighting:** Soft key + fill, often beauty dish or softbox aesthetic.

**Aspect:** 9:16 (TikTok/Reels) or 4:3 (editorial).

**Default duration:** 5-10s.

---

### 2. 🚶 WALK / Tracking
**Definition:** Subject moving through space, camera follows.

**Examples:**
- Real estate walkthrough
- Fashion lookbook walking shot
- Travel B-roll character moving
- Music video performer walking
- Pháp sư entering a haunted location

**Camera grammar:**
- Tracking shot (dolly or steady-cam)
- Side profile or behind-shoulder
- Depth-of-field shifts as subject moves
- Reveal moments at end (location reveal)

**Pacing:** Sustained shot, can be 8-15s continuous.

**Lighting:** Natural environment, motivated practical lights.

**Aspect:** 16:9 (cinematic) or 2.39:1 (anamorphic feel).

**Default duration:** 8-15s.

---

### 3. ⚔️ ACTION / Dynamic
**Definition:** Energy peak, fast movement, climactic moment.

**Examples:**
- Dance MV chorus drop
- Fight sequence
- Sports highlight
- Henshin transformation moment
- Slow-mo product reveal
- Pháp sư đánh bật linh hồn (exorcism climax)

**Camera grammar:**
- Mix of angles within sequence
- Whip pans, crash zooms, low-angle dramatic
- Slow-motion peak moments
- Multiple cuts (rapid editing)

**Pacing:** Fast cuts (0.3-0.8s each) with 1-2 second slow-mo peaks.

**Lighting:** Dramatic, often high-contrast, can include strobing.

**Aspect:** 16:9 or 9:16 depending on platform.

**Default duration:** 8-15s.

---

### 4. 🧘 CONTEMPLATIVE / Atmosphere
**Definition:** Mood-driven, character-light, environment-heavy.

**Examples:**
- Travel documentary B-roll
- Brand mood film
- Nature footage
- Cinematic establishing shots
- Cổ trang opening scene
- Memory / dream sequence

**Camera grammar:**
- Long static shots OR very slow movement
- Wide compositions, landscape ratios
- Drones, cranes for elevated perspective
- Time-lapse possibilities

**Pacing:** Very slow. Each shot 3-6 seconds.

**Lighting:** Natural — golden hour, blue hour, fog, mist.

**Aspect:** 16:9 or 2.39:1 (cinematic).

**Default duration:** 10-20s.

---

### 5. 🎁 PRODUCT / Object Hero
**Definition:** Inanimate object is hero. Beauty pass on materials.

**Examples:**
- Watch / jewelry TVC
- Tech gadget reveal
- Food / beverage closeup
- Liquid / cosmetic macro
- Architectural detail

**Camera grammar:**
- Macro / extreme close-up dominant
- Slow rotation OR static beauty pass
- Rack focus shifts
- Specific reflection / refraction work

**Pacing:** Slow, sensual. Each detail held 1.5-3s.

**Lighting:** Multi-light setup — key + rim + accent. Often studio.

**Aspect:** 1:1 (IG feed) or 16:9 (TVC).

**Default duration:** 6-12s.

---

## 🎯 The Router Decision Tree

```
What's the SUBJECT of your video?
│
├─ Person / character (subject hero) ───▶  Is there significant motion?
│                                          ├─ NO  ───▶  PORTRAIT
│                                          ├─ YES, walking ───▶  WALK
│                                          └─ YES, peak action ───▶  ACTION
│
├─ Environment / mood (subject is "world") ───▶  CONTEMPLATIVE
│
└─ Object / product (subject is inanimate) ───▶  PRODUCT
```

---

## 🔥 Hybrid Archetypes

Real videos often blend 2-3 archetypes. Examples:

### **WALK + ACTION**
Fashion model walks → stops → strikes pose dramatic.
Use: WALK as base, ACTION beats inserted at climax.

### **PORTRAIT + PRODUCT**
Beauty influencer applies skincare, macro on product.
Use: PORTRAIT for face cells, PRODUCT for product cells, alternate.

### **CONTEMPLATIVE + WALK**
Travel documentary character walks through landscape.
Use: CONTEMPLATIVE establishing shots, WALK transitions.

### **ACTION + PORTRAIT**
Henshin transformation — character + transformation effect.
Use: PORTRAIT before/after, ACTION middle.

---

## 📊 Quick Reference Cheatsheet

| Archetype | Pacing | Cuts | Lighting | Aspect | Duration |
|-----------|:------:|:----:|:--------:|:------:|:--------:|
| Portrait | Slow | Few | Soft beauty | 9:16 / 4:3 | 5-10s |
| Walk | Sustained | None to 1 | Natural motivated | 16:9 / 2.39 | 8-15s |
| Action | Fast | Many | Dramatic high-contrast | 16:9 / 9:16 | 8-15s |
| Contemplative | Very slow | Few | Natural ambient | 16:9 / 2.39 | 10-20s |
| Product | Slow sensual | Medium | Multi-light studio | 1:1 / 16:9 | 6-12s |

---

## 🛠️ Application — Router → Workflow

After identifying archetype:

1. **Pick base prompt template** in [prompts/](../prompts/) folder by archetype
2. **Customize subject + setting** for your specific case
3. **Apply** [6-Step Formula](02-six-step-formula.md) or [3-Layer Motion Prompt](03-three-layer-prompt.md)
4. **Use grid method** if duration > 8s (see [Grid Method](04-grid-method.md))

---

## 🎓 Practice — Classify These

Try classifying these video ideas:

1. "Vietnamese pháp sư casting out spirit, dramatic shaman ritual" → ACTION (with PORTRAIT character anchor)
2. "Áo dài model walking through Hội An old town golden hour" → WALK + CONTEMPLATIVE
3. "Macro shot of perfume bottle, light catching glass, slow rotation" → PRODUCT
4. "Influencer applying lipstick mirror reflection" → PORTRAIT
5. "Drone over Saigon at dawn, mist rising over rooftops" → CONTEMPLATIVE
6. "K-pop dance chorus with multi-angle coverage" → ACTION (16-panel master)
7. "Cổ trang princess in palace, slow contemplative scene" → CONTEMPLATIVE + PORTRAIT

---

## 📚 Related

- [6-Step Prompt Formula](02-six-step-formula.md) — Foundation
- [3-Layer Motion Prompt](03-three-layer-prompt.md) — Advanced structure
- [Grid Method](04-grid-method.md) — Multi-shot pipeline
- [Prompts Library](../prompts/) — Templates by archetype

---

[← Resources](README.md) · [Main README](../README.md)
