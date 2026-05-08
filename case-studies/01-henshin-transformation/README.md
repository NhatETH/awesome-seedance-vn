# Case Study 01: Henshin Saigon → Samurai

[← Back to case studies](../README.md)

> Format viral nhất Q2/2026 — biến hình anime/warrior từ ảnh người thật. View potential 500K-2M+ TikTok.

---

## 📝 Brief (Anonymized)

```
Client: Indie creator Saigon, mục tiêu launch personal brand
Brief tiếng Việt:
"Em muốn 1 video henshin biến hình từ phong cách Saigon hiện đại 
sang samurai Nhật Bản. Khuôn mặt giữ nguyên. 8s cho TikTok, ratio 9:16.
Ngân sách: 3 triệu."

Deliverable: 1 video 8 giây MP4, format dọc 9:16, 1080p
```

---

## 🎯 Approach

- **Archetype:** ACTION (with PORTRAIT character anchor)
- **Workflow:** [9-Panel Grid](../../workflows/01-grid-9-panel.md) — sweet spot for 8s henshin
- **Models used:**
  - GPT Image 2 → grid layout
  - Nano Banana 2 → face consistency (Asian face strength)
  - FLUX 1.1 Pro → samurai armor texture detail
  - Seedance 2.0 → motion + audio
- **Total time:** 1.5 hours (including iterations)
- **Production cost:** ~$5

---

## 🎨 Grid Storyboard Prompt

```
A 3×3 grid storyboard (1:1 aspect, 9 cinematic panels with bold black 4px borders 
and 8px white gutters). Henshin transformation sequence — modern Saigon to feudal samurai.

ULTRA-CONSISTENT CHARACTER (@subject1): A 28-year-old Vietnamese man, 175cm slim athletic build.
Hair: black short undercut with longer top swept side, well-styled.
Face: oval, double-lid eyes natural, defined jaw with light stubble, 
medium tan skin matte natural finish.
THE FACE STAYS IDENTICAL ACROSS ALL 9 PANELS — this is critical.

Panel 1: Modern Saigon street, golden hour. Subject in white linen shirt, 
black slim trousers, walking confidently toward camera. Medium shot.

Panel 2: Close-up subject's eyes. Determined expression. 
Background blur shows Saigon traffic.

Panel 3: ECU on hand reaching to chest, white shirt slightly disturbed by wind.

Panel 4: Wide shot. Color shifts cool. Saigon fades to twilight blue mist. 
Subject midway transformation, white shirt morphing into white silk.

Panel 5: Medium shot. Particle effects swirling. Half white linen / half white silk yukata visible. 
Hair lengthens, ties back into samurai topknot.

Panel 6: Close-up. Face same identity. Steam/mist obscures lower half. 
Eyes fierce now. A glint of katana hilt visible at hip.

Panel 7: Wide shot. Setting fully transformed — feudal Japan, wooden temple, 
cherry blossoms. Subject in full samurai outfit: white silk kimono, dark hakama, 
katana at hip, hair in topknot.

Panel 8: Medium 3/4. Hand on katana hilt. Slight bow stance. 
Cherry blossom petals drifting.

Panel 9: HERO POSE. Wide shot. Katana drawn vertical in front of face. 
Cherry blossoms suspended in slow motion. Confident warrior stance.

STYLE REQUIREMENTS:
- Cinematic transformation reference: anime intro sequences meets Akira Kurosawa
- Color script: panels 1-3 warm Saigon golden, panels 4-6 cool transition mist, 
  panels 7-9 saturated samurai golden hour
- Particle effects subtle, not over-stylized
- Anamorphic lens character
- AVOID: melted faces, multiple arms, broken katana physics

CHARACTER FIDELITY: Same face all 9 panels. Same facial structure throughout transformation.
```

---

## 🎬 Motion Prompt (Seedance)

```
STYLE & MOOD:
8-second henshin transformation video, 9:16 vertical for TikTok. 
Cinematic anime intro meets live-action samurai film. 24fps.

DYNAMIC DESCRIPTION:
Animate this 9-panel grid into 8-second continuous transformation:

0-2s (panels 1-3): Modern Saigon establishing. Subject walks to camera, 
close-ups on eyes and hand. Color: warm golden hour.

2-4s (panels 4-6): Transformation phase. Color shifts cool. Particle effects swirl. 
Clothing morphs from white linen to white silk. Hair lengthens. 
Setting blurs and shifts. THE FACE STAYS LOCKED throughout.

4-6s (panels 7-8): Reveal phase. Setting now feudal Japan. 
Subject in samurai outfit, walks toward camera, hand reaches katana.

6-8s (panel 9): HERO POSE. Slow-motion katana draw, cherry blossoms suspended, 
final warrior stance. Hold last frame for emphasis.

Audio: 
- 0-2s: Saigon street ambient (traffic, voices)
- 2-4s: Mystical chimes, swelling string section
- 4-6s: Wind, distant temple bell
- 6-8s: Katana ring, dramatic taiko drum hit on hero pose

STATIC DESCRIPTION:
Subject's face IDENTICAL throughout entire 8 seconds. NO morphing.
Same eye shape, same nose, same jaw structure. 
Only clothing/hair/setting changes.

HARD CONSTRAINTS:
- Face stays locked — same person before, during, after transformation
- Katana must be physically realistic (not glitchy, no clipping)
- Cherry blossoms move with realistic gravity/drift
- No extra arms, fingers, or appendages during transformation
- Vertical 9:16 aspect (will crop from 16:9 generation in CapCut)
```

---

## 📊 Result

**Final video specs:**
- Duration: 8.0s
- Resolution: 1080p (cropped to 1080×1920 for TikTok)
- Frame rate: 24fps
- File size: ~12MB MP4
- Audio: AI-generated, mixed in CapCut

**Quality benchmarks:**
- Face consistency: 9.5/10 (one slight wobble in panel 5)
- Transformation smoothness: 9/10
- Cultural authenticity: 9/10 (consulted Japanese friend for samurai accuracy)
- Overall client satisfaction: 10/10

---

## 💰 ROI Breakdown

| Item | Cost |
|------|:----:|
| GPT Image 2 grid (2 iterations) | $0.80 |
| Nano Banana 2 face cells (3 cells) | $0.40 |
| FLUX 1.1 Pro samurai armor (1 cell) | $0.50 |
| Seedance 480p tests (3 versions) | $1.50 |
| Seedance 1080p final | $2.50 |
| Audio generation | $0.30 |
| **Total cost** | **$6.00** |
| **Client paid** | **3,000,000 VND (~$120)** |
| **Margin** | **95%** |

**Time invested:** 1.5 hours
**Effective hourly rate:** ~$76/hr

---

## 📝 Lessons Learned

### What worked
✅ **Multi-engine composite for face consistency** — Nano Banana 2 made face stronger than GPT Image 2 alone could
✅ **Slow-mo on hero pose (panel 9)** — created the iconic "thumbnail moment"
✅ **Cherry blossoms as visual anchor** — gave viewer something to track during transformation

### What didn't work first try
❌ **First grid had Western-looking face** — fixed by emphasizing "Vietnamese" + reference image
❌ **Initial katana looked like plastic toy** — fixed by specifying "lacquered scabbard with mother-of-pearl inlay"
❌ **Cherry blossoms too sparse** — added "dense cascade of at least 30 petals visible"

### Key insight
Henshin format works best when **transformation has emotional weight**, not just visual flash. The "before" must feel grounded so the "after" feels meaningful.

---

## 🔗 Related

- [Henshin Prompt Template](../../prompts/02-drama/21-henshin-samurai.md)
- [9-Panel Workflow](../../workflows/01-grid-9-panel.md)
- [Character Bible System](../../workflows/03-character-bible.md)

---

[← Case Studies](../README.md) · [Main README](../../README.md)
