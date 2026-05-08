# Case Study 04: ASMR Macro Korean Skincare

[← Back to case studies](../README.md)

> Format viral cho beauty community. Macro extreme close-up + tactile sound design. View potential 100K-500K mỗi clip.

---

## 📝 Brief (Anonymized)

```
Client: K-beauty brand reseller VN, dòng skincare gel
Brief tiếng Việt:
"Em cần 12s ASMR macro shot dòng gel skincare. Cận cảnh kết cấu gel, 
tay người Korean (tone trắng-hồng), cảm giác cool và clean. 
Posted lên TikTok beauty + IG Reels.
Ngân sách: 2 triệu cho 1 video, em cần 5 video set."

Deliverable: 5 × 12s ASMR macro videos, 9:16 vertical
```

---

## 🎯 Approach

- **Archetype:** PRODUCT (extreme macro, no character face)
- **Workflow:** [9-Panel Grid](../../workflows/01-grid-9-panel.md) but rendered at macro scale
- **Key insight:** ASMR macro = audio is 50% of the experience. Sound design as important as visuals.
- **Models:** FLUX 1.1 Pro (best material macro detail) + GPT Image 2 (layout)
- **Total time per video:** 1.5 hours (template-able after first)
- **Production cost per video:** ~$4

---

## 🎨 Grid Storyboard Prompt (Sample — Gel Texture Hero)

```
A 3×3 grid storyboard (1:1 aspect, 9 macro extreme close-up panels with bold black 
4px borders and 8px white gutters). K-beauty ASMR macro skincare gel showcase.

NO character face visible — only hands and product.

HANDS: Korean female hands, fair-pale skin with healthy pink undertone, 
short natural nails with clear topcoat (no color polish), 
no rings or accessories. Slim long fingers.

PRODUCT: Frosted glass jar of skincare gel, 50g size. 
Translucent jade-green gel inside (like aloe vera + green tea blend). 
Brushed silver lid with subtle embossed brand mark (anonymized — generic minimalist mark).

SETTING: Soft white backdrop, marble vanity surface, 
single large softbox key light from above creating gentle gradient shadows.
Slight blue-cool color temperature (clinical clean K-beauty aesthetic).

Read panels left-to-right, top-to-bottom:

Panel 1: ECU. Closed jar on marble surface, fingers approaching from frame edge.

Panel 2: ECU. Fingers grasp lid, slight pressure visible in fingertip.

Panel 3: MACRO. Lid being twisted off, satisfying mechanical detail, 
slight glass-against-glass sound implied.

Panel 4: MACRO. Lid lifted away, gel surface revealed. 
Gel surface is glossy, slight meniscus at edge.

Panel 5: EXTREME MACRO. Fingertip touching gel surface — 
moment of contact, gel deforms slightly, surface tension visible.

Panel 6: EXTREME MACRO. Finger pulls back, single thread of gel briefly stretches 
then breaks in beautiful surface tension reveal.

Panel 7: MACRO. Gel on fingertip, semi-translucent, jade-green color, 
small bubble visible inside.

Panel 8: ECU. Fingertip approaching back of opposite hand, 
gel about to make contact with skin.

Panel 9: EXTREME MACRO. Gel applied to skin, beginning to spread, 
glossy sheen on skin, water-like texture revealing pore detail of skin.

STYLE REQUIREMENTS:
- K-beauty editorial aesthetic, clinical clean meets sensual tactile
- Reference: Mario Sorrenti macro work + Sephora hero shots
- Anamorphic macro lens character
- Color: pale jade green gel, fair Korean skin, white-cool background
- AVOID: yellow tints, harsh shadows, plastic look, over-saturation

MATERIAL PHYSICS (critical for ASMR):
- Gel: viscous translucent, surface tension visible at edges, 
  slow-mo deformation when touched, glossy reflective surface
- Skin: subsurface scattering visible, pore structure preserved at macro, 
  no plastic-doll smoothing, fine vellus hair visible at extreme close-up
- Glass jar: frosted texture, light refraction visible, 
  micro-scratches if any are absent (new product feel)
```

---

## 🎬 Motion Prompt (Seedance) — Sound Design Critical

```
STYLE & MOOD:
12-second ASMR macro skincare video. K-beauty clean clinical luxury. 
9:16 vertical for TikTok. 24fps. Soft cool palette.

DYNAMIC DESCRIPTION:
Animate this 9-panel macro grid into 12-second satisfying ASMR sequence:

0-3s (panels 1-2): Hand approaches and grasps jar. Slow deliberate movement.
Audio: silence then soft glass-tap when finger contacts jar.

3-5s (panel 3-4): Lid twisted off, opens.
Audio: subtle glass-on-glass twist, pop of seal release.

5-7s (panels 5-6): THE MONEY SHOT — finger touches gel, surface tension stretch.
Audio: satisfying squelch + brief stretch sound on the gel pull.
Slow-motion x 0.5 speed for these 2 seconds.

7-9s (panels 7-8): Gel on finger, finger moves to back of opposite hand.
Audio: silence (anticipation), then soft gel-against-skin sound.

9-12s (panel 9): Gel spreads on skin, glossy finish reveal.
Audio: gentle smoothing sound, ambient room tone, soft exhale at end.

STATIC DESCRIPTION:
Hand identity stays consistent (same skin tone, same nail finish).
Product stays consistent (same jar, same gel color, same jade-green opacity).
Lighting consistent throughout (soft top key, gentle gradient).
Macro lens character consistent (same depth of field, same focus distance).

HARD CONSTRAINTS:
- Hands clearly anatomically correct, 5 fingers always visible
- Gel physics realistic (surface tension, viscous flow, no glitches)
- No motion blur on extreme macro shots (clarity is the appeal)
- Sound design: ASMR-quality (clean, isolated, satisfying)
```

---

## 📊 Result Set (5 Videos)

| Video # | Product | Duration | View count week 1 |
|:-------:|---------|:--------:|:-----------------:|
| 1 | Gel cleanser | 12s | 320K |
| 2 | Toner pad | 12s | 180K |
| 3 | Serum dropper | 12s | 580K (top performer) |
| 4 | Cream jar | 12s | 240K |
| 5 | Sheet mask | 12s | 150K |

**Total views first week: 1.47M**

---

## 💰 ROI Breakdown (5-video set)

| Item | Cost |
|------|:----:|
| GPT Image 2 grids (5 × 2 iterations) | $4.00 |
| FLUX 1.1 Pro material macro (5 × 3 cells) | $6.00 |
| Seedance 480p tests (5 × 3 versions) | $7.50 |
| Seedance 1080p finals (5 videos) | $12.50 |
| Audio generation + ASMR sound design | $5.00 |
| **Total cost** | **~$35** |
| **Client paid** | **5 × 2,000,000 = 10,000,000 VND (~$400)** |
| **Margin** | **91%** |

**Time invested:** 7.5 hours total (1.5/video, template reused)
**Effective hourly rate:** ~$48/hr

---

## 📝 Lessons Learned

### What worked
✅ **FLUX 1.1 Pro for material physics** — gel viscosity + surface tension only FLUX nails
✅ **Slow-motion at money shot** — 2-second slow-mo is the "ASMR moment" everyone screenshots
✅ **Template reuse** — first video took 3 hours, others 1 hour each

### What didn't work first try
❌ **Initial gel looked too plastic-like** — added "subsurface scattering, internal viscosity hint, slight bubbles"
❌ **Hands looked too generic Western** — added "Korean female hands, fair-pale with healthy pink undertone"
❌ **Audio felt artificial** — switched to recording real gel sounds, layered with AI-generated ambient

### Key insight
ASMR macro is **5% video, 95% sound design**. The visual is the trigger, but audio is what makes viewers stay 12 seconds. Plan your audio FIRST, then build video to match.

---

## 🔗 Related

- [Beauty Pass Technique](../../workflows/02-grid-16-panel/03-tvc-luxury.md#beauty-pass-technique-the-real-secret)
- [9-Panel Workflow](../../workflows/01-grid-9-panel.md)

---

[← Case Studies](../README.md) · [Main README](../../README.md)
