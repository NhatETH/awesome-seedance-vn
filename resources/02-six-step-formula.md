# 📗 The 6-Step Prompt Formula

> **Công thức cơ bản** để viết Seedance 2.0 prompt. Master công thức này = master 60% prompting. Còn lại là [3-Layer Motion Prompt Structure](03-three-layer-prompt.md) cho advanced.

[← Back to resources](README.md)

---

## 🎯 The Formula

Mọi Seedance prompt tốt đều follow 6-step structure này:

```
[1. SUBJECT] + [2. ACTION] + [3. CAMERA] + [4. SETTING] + [5. STYLE] + [6. CONSTRAINTS]
```

**Quan trọng:** Order matters. Seedance attention weights heavily về front của prompt → put SUBJECT first, CONSTRAINTS last.

---

## 📋 Step-by-Step Breakdown

### Step 1: SUBJECT — Cụ thể, không chung chung

❌ Không tốt: "a woman"
✅ Tốt: "A 28-year-old Vietnamese woman with shoulder-length black wavy hair, wearing a white linen dress"

**Quy tắc:**
- Tuổi cụ thể (28, không "young")
- Dân tộc cụ thể (Vietnamese, Korean — không "Asian")
- Đặc điểm vật lý nổi bật (3-5 features)
- Wardrobe specific (color + material + cut)

### Step 2: ACTION — Verb mạnh, không adjective

❌ Không tốt: "She is beautiful and walking"
✅ Tốt: "She walks slowly across the wooden bridge, hand trailing along the railing"

**Quy tắc:**
- 1 main verb chính (walks, stands, reaches, turns)
- 1-2 sub-actions để add depth (hand trailing, looking up)
- KHÔNG dùng "is + adjective" (waste tokens)
- Speed/quality verbs: slowly, deliberately, hesitantly, sharply

### Step 3: CAMERA — Cinematic, không "iPhone"

❌ Không tốt: "shot on iPhone"
✅ Tốt: "Medium tracking shot, camera dollies left following her, anamorphic lens"

**Quy tắc:**
- Shot type: Wide / Medium / Close-up / ECU / Macro
- Movement: Static / Pan / Tilt / Dolly / Crane / Handheld
- Lens character: Anamorphic / 35mm prime / 75mm portrait / Wide-angle
- Distance: 1m / 3m / 10m (helps Seedance compute depth)

**Cinematic camera vocabulary cheatsheet:**
| Term | Meaning |
|------|---------|
| Push-in | Camera moves toward subject |
| Pull-out | Camera moves away from subject |
| Dolly | Camera on rails moving sideways |
| Crane / jib | Camera moving vertically |
| Whip pan | Fast horizontal pan |
| Rack focus | Focus shift between depths |
| Dutch tilt | Tilted angle for unease |

### Step 4: SETTING — Time + Place + Light

❌ Không tốt: "in a forest"
✅ Tốt: "In a misty pine forest at dawn, soft golden light filtering through trees, cold blue shadows"

**Quy tắc:**
- Place specific (pine forest > forest)
- Time of day (dawn / golden hour / blue hour / midday / dusk / night)
- Light direction & quality (front / side / back / top / soft / harsh)
- Color temperature hint (golden / cool blue / warm amber)

### Step 5: STYLE — Reference cụ thể

❌ Không tốt: "cinematic"
✅ Tốt: "Wong Kar-wai aesthetic, anamorphic lens, soft grain, painterly color"

**Quy tắc:**
- 1 director / DP reference (Wong Kar-wai, Roger Deakins, Trần Anh Hùng)
- 1 visual style (painterly / documentary / commercial / editorial)
- 1 lens character (anamorphic / spherical / vintage / clinical)
- Optional: 1 film stock or LUT (Kodak Vision3 / Fuji 8553)

### Step 6: CONSTRAINTS — Tell what NOT to do

❌ Không tốt: (omit constraints)
✅ Tốt: "No camera shake. No text in frame. No motion blur on face. Hands clearly show 5 fingers."

**Quy tắc:**
- Anti-glitch constraints (no morphing, no extra fingers, no warping)
- Aesthetic constraints (no over-saturation, no plastic skin)
- Composition constraints (no crowd in background, no logos visible)

---

## 🎬 Full Example (Affiliate Video)

Concept: Woman holding skincare product, ASMR macro vibe.

```
[SUBJECT] A 24-year-old Korean woman with porcelain skin, slick low ponytail, 
wearing minimalist beige knit sweater, holding a frosted glass skincare bottle.

[ACTION] She slowly turns the bottle in her hand, light catching the glass surface, 
her thumb gently pressing the dropper top.

[CAMERA] Macro close-up, 100mm lens, shallow depth of field. 
Camera holds steady at chest level, subject's face just out of focus in background.

[SETTING] Soft morning light in a minimalist white studio space, 
single key light from camera-left at 45 degrees, gentle shadows.

[STYLE] K-beauty editorial aesthetic, glass skin finish, slight grain, 
Mario Sorrenti reference, tactile and sensual.

[CONSTRAINTS] Hands clearly show 5 fingers, fingernails natural with clear polish only,
no harsh studio strobe, no text on bottle, no motion blur on the bottle.
```

---

## 🚨 Common Mistakes

### ❌ Mistake 1: Adjective overload
"Beautiful, stunning, gorgeous, amazing woman" wastes tokens. Pick 1 specific descriptor.

### ❌ Mistake 2: Vague camera
"Cinematic shot" tells Seedance nothing. Specify shot type + movement.

### ❌ Mistake 3: Missing constraints
Without constraints, AI defaults to common failure modes. Always add 2-3 negatives.

### ❌ Mistake 4: Lighting unmentioned
If you don't specify, you get default flat lighting. Always specify light source + direction.

### ❌ Mistake 5: No reference style
"Looks good" ≠ specific aesthetic. Reference 1 director or genre.

---

## 🎓 Practice Exercises

### Exercise 1: Cafe scene
Write a 6-step prompt for: Woman 30s reading a book in cafe, Saigon afternoon.

### Exercise 2: Product reveal
Write a 6-step prompt for: Watch on velvet display, slowly rotating.

### Exercise 3: Action moment
Write a 6-step prompt for: Skater landing a kickflip in slow motion, urban setting.

Compare your prompts against examples in [prompts/](../prompts/) folder.

---

## 📚 Next Reading

- [03 — 3-Layer Motion Prompt Structure](03-three-layer-prompt.md) — Advanced structure for complex motion
- [04 — Storyboard Grid Method](04-grid-method.md) — Multi-shot from single grid
- [05 — Scene Archetype Router](05-archetype-router.md) — 5 archetypes mapped to formula

---

[← Resources](README.md) · [Main README](../README.md)
