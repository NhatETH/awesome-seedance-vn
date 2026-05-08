# Case Study 03: TVC Nước Hoa "Saigon Centre"

[← Back to case studies](../README.md)

> Premium TVC nước hoa với 4-panel cinematic. Hero shot beauty pass technique. Anonymized client (perfume brand VN).

---

## 📝 Brief (Anonymized)

```
Client: Boutique perfume brand VN
Brief tiếng Việt:
"Em cần TVC 30 giây cho dòng nước hoa mới 'Saigon Centre' — 
inspiration từ Saigon những năm 1990, hoài cổ pha hiện đại. 
Mood elegant, không quá trẻ. Target: phụ nữ 30-50 tuổi.
Format: 16:9 (cinema/digital) + 9:16 (Reels) + 1:1 (IG feed).
Ngân sách: 25 triệu cho concept + production."

Deliverable: 1 master 30s + 3 format crops
```

---

## 🎯 Approach

- **Archetype:** PRODUCT (with PORTRAIT character anchor)
- **Workflow:** Custom **4-panel grid** for TVC narrative arc (1 min/panel = 30s total but feels longer)
- **Why 4 panels?** Premium TVC pacing is SLOW. Each panel held 7.5s (long for AI video, but feasible với good motion prompt).
- **Models:** GPT Image 2 + FLUX 1.1 Pro (perfume bottle hero shot)
- **Total time:** 4 hours
- **Production cost:** ~$15

---

## 🎬 The 4-Panel Brand Story

| Panel | Beat | Camera |
|-------|------|--------|
| 1 | Saigon 1990s establish — Catinat Street, soft golden | Wide aerial → push-in |
| 2 | Woman 40s in vintage áo dài, walking past colonial architecture | Medium tracking |
| 3 | She enters boutique, sees bottle on display | CU bottle |
| 4 | She holds bottle, light catches glass, closes eyes inhaling | Macro hero shot |

---

## 🎨 Grid Storyboard Prompt (Excerpt)

```
A 2×2 grid storyboard (16:9 aspect WIDE since this is cinematic TVC, 
4 panels with bold black 4px borders and 8px white gutters). 
Premium Vietnamese perfume brand TVC, Saigon 1990s nostalgic luxury.

ULTRA-CONSISTENT CHARACTER (@subject1): A 42-year-old Vietnamese woman. 
168cm slim elegant. Hair: dark brown shoulder-length with soft waves, 
parted side, polished but with slight 90s romantic feel. 
Face: mature beauty, fine smile lines (NOT anti-aged), warm undertone skin, 
soft makeup with pink-nude lip, slight blush.
Wardrobe: pale yellow silk áo dài with subtle floral motif (lotus pattern), 
matching pale yellow silk pants, nude pointed-toe heels, vintage gold watch, 
small pearl earrings.

PRODUCT (@subject2): Perfume bottle "Saigon Centre" — 
Faceted crystal glass cube design, 50ml capacity, 
amber-gold liquid inside (subtle gradient).
Cap: brushed gold with embossed Saigon skyline silhouette.
Label: minimalist serif font, gold foil "Saigon Centre" centered.

Setting: Saigon 1990s aesthetic — restored colonial street (Đồng Khởi/Catinat), 
warm afternoon light, French architectural details.

Read panels left-to-right, top-to-bottom:

Panel 1 (top-left): WIDE AERIAL of Saigon Catinat Street 1990s aesthetic. 
French colonial buildings, warm afternoon golden hour, faint mist of nostalgia.

Panel 2 (top-right): MEDIUM TRACKING. Character walks past colonial architecture, 
yellow áo dài flowing in soft breeze. Bicycle bell rings in background. 
Light filters through trees, dappled shadows.

Panel 3 (bottom-left): MEDIUM CU. Character inside boutique (warm wood interior, 
brass fixtures, soft music implied). She sees the perfume bottle on display, 
soft smile of recognition.

Panel 4 (bottom-right): MACRO HERO SHOT. She holds bottle, light catches the crystal 
facets creating prismatic refractions. Eyes closed, slight smile, gentle inhale. 
This is THE iconic image of the TVC.

STYLE REQUIREMENTS:
- Premium luxury TVC, Wong Kar-wai meets Hermès commercial aesthetic
- Anamorphic 2.35:1 framing within each cell
- Color palette: warm amber gold + pale yellow silk + brass + crystal refractions
- Soft natural light + motivated practical light only
- AVOID: harsh studio strobe, busy backgrounds, generic luxury

PRODUCT FIDELITY ABSOLUTE: Perfume bottle must look IDENTICAL in panels 3 and 4.
Same crystal cut, same amber liquid level, same gold cap with skyline detail.

BEAUTY PASS (panel 4):
- Crystal: micro-scratches NONE, refractive caustic light visible
- Gold cap: brushed surface with anisotropic reflection
- Liquid: amber gradient with internal viscosity hint
- Skin (her hand): subsurface scattering at fingertip edge
```

---

## 📊 Result

- Master: 30.0s @ 1080p 24fps anamorphic 2.39:1
- Crops: 9:16 vertical (15s cut) + 1:1 square (10s cut)
- Music: Licensed library track (Vietnamese 90s nostalgic style)
- Client used in: Cinema chains (Galaxy/CGV pre-roll), digital (YouTube/IG)

---

## 💰 ROI Breakdown

| Item | Cost |
|------|:----:|
| GPT Image 2 grid (3 iterations) | $1.20 |
| FLUX 1.1 Pro hero shot bottle (4 versions) | $4.00 |
| Seedance 480p tests (5 versions) | $2.50 |
| Seedance 1080p master | $3.50 |
| 2 additional 1080p crops generation | $5.00 |
| Audio licensing | $20 (royalty-free library) |
| Editing time CapCut + DaVinci color grade | (your time, 2 hrs) |
| **Total cost** | **~$36** |
| **Client paid** | **25,000,000 VND (~$1,000)** |
| **Margin** | **96%** |

**Time invested:** 4 hours
**Effective hourly rate:** ~$240/hr

---

## 📝 Lessons Learned

### What worked
✅ **4-panel structure for premium pacing** — gave each beat space to breathe (TVC luxury rule: less is more)
✅ **FLUX 1.1 Pro for hero bottle shot** — material physics on crystal/gold no other model nailed
✅ **Multi-format from one master** — 1 generation, 3 crops, 3x deliverables

### What didn't work first try
❌ **Character looked too 30s in V1** — strengthened "fine smile lines visible" + "mature beauty NOT anti-aged"
❌ **Bottle had wrong proportions** — added explicit dimensions "50ml cube" + reference image
❌ **Setting felt too modern** — added "1990s aesthetic, French colonial restoration, no smartphones, no modern signage"

### Key insight
Premium TVC clients pay for **restraint**, not flash. 4-panel forces patience. AI naturally wants to over-generate detail — fight that with explicit "minimalist" constraints.

---

## 🔗 Related

- [16-Panel TVC Luxury Master Template](../../workflows/02-grid-16-panel/03-tvc-luxury.md)
- [3-Layer Motion Prompt](../../resources/03-three-layer-prompt.md)

---

[← Case Studies](../README.md) · [Main README](../../README.md)
